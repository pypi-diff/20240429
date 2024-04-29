# Comparing `tmp/trytond_quality-7.0.0.tar.gz` & `tmp/trytond_quality-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_quality-7.0.0.tar", last modified: Mon Oct 30 17:36:33 2023, max compression
+gzip compressed data, was "trytond_quality-7.2.0.tar", last modified: Mon Apr 29 15:46:45 2024, max compression
```

## Comparing `trytond_quality-7.0.0.tar` & `trytond_quality-7.2.0.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.730690 trytond_quality-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-22 17:23:15.000000 trytond_quality-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:11:14.000000 trytond_quality-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:11:14.000000 trytond_quality-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2780 2023-10-30 17:36:33.730690 trytond_quality-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      979 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.727357 trytond_quality-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-22 17:23:15.000000 trytond_quality-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:15.000000 trytond_quality-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.727357 trytond_quality-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/icons/tryton-quality.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.720690 trytond_quality-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12415 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13164 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12448 2023-10-30 16:47:45.000000 trytond_quality-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12579 2023-10-30 16:47:45.000000 trytond_quality-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12405 2023-10-30 16:47:45.000000 trytond_quality-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10564 2023-10-30 16:47:45.000000 trytond_quality-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2023-10-28 12:11:25.000000 trytond_quality-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1624 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28138 2023-10-24 08:23:41.000000 trytond_quality-7.0.0/quality.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20577 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/quality.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:36:33.730690 trytond_quality-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4606 2023-10-27 17:38:49.000000 trytond_quality-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2682 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6352 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.724024 trytond_quality-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2481 2023-09-24 21:55:45.000000 trytond_quality-7.0.0/tests/scenario_quality_control_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2607 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/tests/scenario_quality_inspection.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_quality-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      181 2023-10-30 17:11:10.000000 trytond_quality-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.727357 trytond_quality-7.0.0/trytond_quality.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2780 2023-10-30 17:36:33.000000 trytond_quality-7.0.0/trytond_quality.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2368 2023-10-30 17:36:33.000000 trytond_quality-7.0.0/trytond_quality.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:36:33.000000 trytond_quality-7.0.0/trytond_quality.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-10-30 17:36:33.000000 trytond_quality-7.0.0/trytond_quality.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-08 12:43:26.000000 trytond_quality-7.0.0/trytond_quality.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-10-30 17:36:33.000000 trytond_quality-7.0.0/trytond_quality.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:36:33.000000 trytond_quality-7.0.0/trytond_quality.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:33.724024 trytond_quality-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1177 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_alert_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_alert_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      816 2023-10-07 15:40:36.000000 trytond_quality-7.0.0/view/quality_control_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_control_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      709 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_control_point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_control_point_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1281 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_inspection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-08-13 15:26:13.000000 trytond_quality-7.0.0/view/quality_inspection_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.956164 trytond_quality-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-29 15:24:26.000000 trytond_quality-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:24:26.000000 trytond_quality-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2771 2024-04-29 15:46:45.956164 trytond_quality-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      979 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.949497 trytond_quality-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_quality-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.949497 trytond_quality-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/icons/tryton-quality.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12416 2024-04-29 13:17:17.000000 trytond_quality-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13164 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12447 2024-04-29 13:17:17.000000 trytond_quality-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12579 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12405 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10564 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1624 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    29183 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/quality.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20163 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/quality.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:45.956164 trytond_quality-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4597 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6334 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2444 2024-04-22 12:14:36.000000 trytond_quality-7.2.0/tests/scenario_quality_control_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2570 2024-04-22 12:14:36.000000 trytond_quality-7.2.0/tests/scenario_quality_inspection.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_quality-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-04-29 15:24:22.000000 trytond_quality-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/trytond_quality.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2771 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2350 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-08 12:43:26.000000 trytond_quality-7.2.0/trytond_quality.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1177 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_alert_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_alert_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      816 2024-02-04 18:51:26.000000 trytond_quality-7.2.0/view/quality_control_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_control_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      709 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_control_point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_control_point_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1281 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_inspection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_inspection_list.xml
```

### Comparing `trytond_quality-7.0.0/COPYRIGHT` & `trytond_quality-7.2.0/COPYRIGHT`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2023 B2CK
-Copyright (C) 2023 Cédric Krier
-Copyright (C) 2021-2023 Sergi Almacellas Abellana
+Copyright (C) 2023-2024 B2CK
+Copyright (C) 2023-2024 Cédric Krier
+Copyright (C) 2021-2024 Sergi Almacellas Abellana
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_quality-7.0.0/LICENSE` & `trytond_quality-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/PKG-INFO` & `trytond_quality-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_quality
-Version: 7.0.0
+Version: 7.2.0
 Summary: Quality Management
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-quality
+Project-URL: Documentation, https://docs.tryton.org/modules-quality
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton quality QMS inspection
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 ##############
 Quality Module
 ##############
 
 The *Quality Module* enables quality to be controlled by configuring control
 points and inspecting against these when certain operations are performed.
```

### Comparing `trytond_quality-7.0.0/__init__.py` & `trytond_quality-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/doc/conf.py` & `trytond_quality-7.2.0/doc/conf.py`

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

### Comparing `trytond_quality-7.0.0/doc/design.rst` & `trytond_quality-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/icons/LICENSE` & `trytond_quality-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/bg.po` & `trytond_quality-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/ca.po` & `trytond_quality-7.2.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
 msgctxt "model:quality.configuration,name:"
 msgid "Quality Configuration"
 msgstr "Configuració qualitat"
 
 msgctxt "model:quality.configuration.sequence,name:"
 msgid "Quality Configuration Sequence"
-msgstr "Seqüencia configuració qualitat"
+msgstr "Configuració Seqüencies qualitat"
 
 msgctxt "model:quality.control,name:"
 msgid "Quality Control"
 msgstr "Control de qualitat"
 
 msgctxt "model:quality.control.point,name:"
 msgid "Quality Control Point"
```

### Comparing `trytond_quality-7.0.0/locale/cs.po` & `trytond_quality-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/de.po` & `trytond_quality-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/es.po` & `trytond_quality-7.2.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 
 msgctxt "field:quality.alert,title:"
 msgid "Title"
 msgstr "Título"
 
 msgctxt "field:quality.configuration,alert_sequence:"
 msgid "Alert Sequence"
-msgstr "Sequència alertas"
+msgstr "Secuencia alertas"
 
 msgctxt "field:quality.configuration,inspection_sequence:"
 msgid "Inspection Sequence"
 msgstr "Secuencia Inspecciones"
 
 msgctxt "field:quality.configuration.sequence,alert_sequence:"
 msgid "Alert Sequence"
-msgstr "Sequencia Alertas"
+msgstr "Secuencia Alertas"
 
 msgctxt "field:quality.configuration.sequence,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:quality.configuration.sequence,inspection_sequence:"
 msgid "Inspection Sequence"
```

### Comparing `trytond_quality-7.0.0/locale/es_419.po` & `trytond_quality-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/et.po` & `trytond_quality-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/fa.po` & `trytond_quality-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/fi.po` & `trytond_quality-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/fr.po` & `trytond_quality-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/hu.po` & `trytond_quality-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/id.po` & `trytond_quality-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/it.po` & `trytond_quality-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/lo.po` & `trytond_quality-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/lt.po` & `trytond_quality-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/nl.po` & `trytond_quality-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/pl.po` & `trytond_quality-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/pt.po` & `trytond_quality-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/ro.po` & `trytond_quality-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/ru.po` & `trytond_quality-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/sl.po` & `trytond_quality-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/tr.po` & `trytond_quality-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/uk.po` & `trytond_quality-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/locale/zh_CN.po` & `trytond_quality-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/message.xml` & `trytond_quality-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/production.py` & `trytond_quality-7.2.0/production.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     __name__ = 'production'
 
     def quality_control_pattern(self, operation):
         pattern = super().quality_control_pattern(operation)
         pattern['company'] = self.company.id
         if operation == 'run':
             pattern['products'] = {m.product.id for m in self.inputs}
-        elif operation == 'done':
+        elif operation == 'do':
             pattern['products'] = {m.product.id for m in self.outputs}
         return pattern
 
     @classmethod
     @ModelView.button
     @ControlledMixin.control('run', 'quality.wizard_production_inspect_run')
     def run(cls, productions):
         return super().run(productions)
 
     @classmethod
     @ModelView.button
-    @ControlledMixin.control('done', 'quality.wizard_production_inspect_done')
-    def done(cls, productions):
-        return super().done(productions)
+    @ControlledMixin.control('do', 'quality.wizard_production_inspect_do')
+    def do(cls, productions):
+        return super().do(productions)
```

### Comparing `trytond_quality-7.0.0/production.xml` & `trytond_quality-7.2.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/quality.py` & `trytond_quality-7.2.0/quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,25 +163,25 @@
     "Quality Control"
     __name__ = 'quality.control'
 
     name = fields.Char("Name", required=True, translate=True)
 
     operations = fields.MultiSelection([
             ('stock.shipment.in:receive', "Supplier Shipment Received"),
-            ('stock.shipment.in:done', "Supplier Shipment Done"),
+            ('stock.shipment.in:do', "Supplier Shipment Done"),
             ('stock.shipment.out:pick', "Customer Shipment Picked"),
             ('stock.shipment.out:pack', "Customer Shipment Packed"),
             ('stock.shipment.out.return:receive',
                 "Customer Shipment Return Received"),
-            ('stock.shipment.out.return:done',
+            ('stock.shipment.out.return:do',
                 "Customer Shipment Return Done"),
             ('stock.shipment.internal:ship', "Internal Shipment Shipped"),
-            ('stock.shipment.internal:done', "Internal Shipment Done"),
+            ('stock.shipment.internal:do', "Internal Shipment Done"),
             ('production:run', "Production Run"),
-            ('production:done', "Production Done"),
+            ('production:do', "Production Done"),
             ], "Operations",
         help="The operations for which the control is performed.")
     frequency = fields.Float(
         "Frequency", digits=(1, 4), required=True,
         domain=[
             ('frequency', '>=', 0),
             ('frequency', '<=', 1),
@@ -200,14 +200,40 @@
             },
         help="The product to which the control applies.")
 
     points = fields.One2Many(
         'quality.control.point', 'control', "Points", required=True)
 
     @classmethod
+    def __register__(cls, module):
+        table = cls.__table__()
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
+        update = transaction.connection.cursor()
+
+        super().__register__(module)
+
+        # Migration from 7.0: rename done button to do
+        for old, new in [
+                ('stock.shipment.in:done', 'stock.shipment.in:do'),
+                ('stock.shipment.out.return:done',
+                    'stock.shipment.out.return:do'),
+                ('stock.shipment.internal:done',
+                    'stock.shipment.internal:do'),
+                ('production:done', 'production:do'),
+                ]:
+            cursor.execute(*table.select(
+                    table.id, table.operations,
+                    where=table.operations.like(f'%{old}%')))
+            for id_, operations in cursor:
+                update.execute(*table.update(
+                        [table.operations],
+                        operations.replace(old, new)))
+
+    @classmethod
     def default_frequency(cls):
         return 1
 
     @classmethod
     def get_inspections(cls, records, operation):
         pool = Pool()
         Inspection = pool.get('quality.inspection')
@@ -260,15 +286,16 @@
         return random.random() <= self.frequency
 
 
 class ControlPoint(DictSchemaMixin, ModelSQL, ModelView):
     "Quality Control Point"
     __name__ = 'quality.control.point'
 
-    control = fields.Many2One('quality.control', "Control", required=True)
+    control = fields.Many2One(
+        'quality.control', "Control", required=True, ondelete='CASCADE')
     tolerance_lower = fields.Float(
         "Tolerance Lower",
         states={
             'invisible': ~Eval('type_').in_(['integer', 'float', 'numeric']),
             })
     tolerance_upper = fields.Float(
         "Tolerance Upper",
```

### Comparing `trytond_quality-7.0.0/quality.xml` & `trytond_quality-7.2.0/quality.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_quality-7.0.0/quality.xml` & `trytond_quality-7.2.0/quality.xml`

```diff
@@ -44,22 +44,22 @@
     <record model="ir.action.act_window.view" id="act_quality_configuration_form_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="quality_configuration_view_form"/>
       <field name="act_window" ref="act_quality_configuration_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_quality_configuration_form" sequence="10" id="menu_quality_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_quality_configuration">
-      <field name="model" search="[('model', '=', 'quality.configuration')]"/>
+      <field name="model">quality.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_quality_configuration_quality_admin">
-      <field name="model" search="[('model', '=', 'quality.configuration')]"/>
+      <field name="model">quality.configuration</field>
       <field name="group" ref="group_quality_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_quality_inspection">
@@ -106,31 +106,31 @@
     <record model="ir.action.act_window.view" id="act_quality_control_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="quality_control_view_form"/>
       <field name="act_window" ref="act_quality_control_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_quality_control_form" sequence="20" id="menu_quality_control"/>
     <record model="ir.model.access" id="access_quality_control">
-      <field name="model" search="[('model', '=', 'quality.control')]"/>
+      <field name="model">quality.control</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_quality_control_quality_admin">
-      <field name="model" search="[('model', '=', 'quality.control')]"/>
+      <field name="model">quality.control</field>
       <field name="group" ref="group_quality_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_quality_control_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'quality.control')]"/>
+      <field name="model">quality.control</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_quality_control_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_quality_control_companies"/>
     </record>
     <record model="ir.rule" id="rule_quality_control_no_company">
@@ -203,60 +203,60 @@
     </record>
     <record model="ir.action.act_window.view" id="act_quality_inspection_form_relate_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="quality_inspection_view_form"/>
       <field name="act_window" ref="act_quality_inspection_form_relate"/>
     </record>
     <record model="ir.model.access" id="access_quality_inspection">
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
+      <field name="model">quality.inspection</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_quality_control_quality">
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
+      <field name="model">quality.inspection</field>
       <field name="group" ref="group_quality"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_quality_inspection_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
+      <field name="model">quality.inspection</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_quality_inspection_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_quality_inspection_companies"/>
     </record>
     <record model="ir.model.button" id="quality_inspection_pending_button">
+      <field name="model">quality.inspection</field>
       <field name="name">pending</field>
       <field name="string">Pending</field>
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
     </record>
     <record model="ir.model.button" id="quality_inspection_process_button">
+      <field name="model">quality.inspection</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
     </record>
     <record model="ir.model.button" id="quality_inspection_pass_button">
+      <field name="model">quality.inspection</field>
       <field name="name">pass_</field>
       <field name="string">Pass</field>
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
     </record>
     <record model="ir.model.button-res.group" id="quality_inspection_pass_button_group_quality">
       <field name="button" ref="quality_inspection_pass_button"/>
       <field name="group" ref="group_quality"/>
     </record>
     <record model="ir.model.button" id="quality_inspection_fail_button">
+      <field name="model">quality.inspection</field>
       <field name="name">fail</field>
       <field name="string">Fail</field>
-      <field name="model" search="[('model', '=', 'quality.inspection')]"/>
     </record>
     <record model="ir.model.button-res.group" id="quality_inspection_fail_button_group_quality">
       <field name="button" ref="quality_inspection_fail_button"/>
       <field name="group" ref="group_quality"/>
     </record>
     <record model="ir.ui.view" id="quality_alert_view_form">
       <field name="model">quality.alert</field>
@@ -307,47 +307,47 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_quality_alert_form"/>
     </record>
     <menuitem parent="menu_quality" action="act_quality_alert_form" sequence="10" id="menu_quality_alert_form"/>
     <record model="ir.model.access" id="access_quality_alert">
-      <field name="model" search="[('model', '=', 'quality.alert')]"/>
+      <field name="model">quality.alert</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_quality_alert_quality">
-      <field name="model" search="[('model', '=', 'quality.alert')]"/>
+      <field name="model">quality.alert</field>
       <field name="group" ref="group_quality"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="quality_alert_open_button">
+      <field name="model">quality.alert</field>
       <field name="name">open</field>
       <field name="string">Open</field>
-      <field name="model" search="[('model', '=', 'quality.alert')]"/>
     </record>
     <record model="ir.model.button" id="quality_alert_process_button">
+      <field name="model">quality.alert</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'quality.alert')]"/>
     </record>
     <record model="ir.model.button" id="quality_alert_defer_button">
+      <field name="model">quality.alert</field>
       <field name="name">defer</field>
       <field name="string">Defer</field>
-      <field name="model" search="[('model', '=', 'quality.alert')]"/>
     </record>
     <record model="ir.model.button" id="quality_alert_resolve_button">
+      <field name="model">quality.alert</field>
       <field name="name">resolve</field>
       <field name="string">Resolve</field>
-      <field name="model" search="[('model', '=', 'quality.alert')]"/>
     </record>
   </data>
   <data noupdate="1">
     <record model="ir.sequence" id="sequence_quality_inspection">
       <field name="name">Quality Inspection</field>
       <field name="sequence_type" ref="sequence_type_quality_inspection"/>
     </record>
```

### Comparing `trytond_quality-7.0.0/setup.py` & `trytond_quality-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-quality',
+        "Documentation": 'https://docs.tryton.org/modules-quality',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton quality QMS inspection',
     package_dir={'trytond.modules.quality': '.'},
     packages=(
         ['trytond.modules.quality']
```

### Comparing `trytond_quality-7.0.0/stock.py` & `trytond_quality-7.2.0/stock.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,17 @@
         'receive', 'quality.wizard_stock_shipment_in_inspect_receive')
     def receive(cls, shipments):
         return super().receive(shipments)
 
     @classmethod
     @ModelView.button
     @ControlledMixin.control(
-        'done', 'quality.wizard_stock_shipment_in_inspect_done')
-    def done(cls, shipments):
-        return super().done(shipments)
+        'do', 'quality.wizard_stock_shipment_in_inspect_do')
+    def do(cls, shipments):
+        return super().do(shipments)
 
 
 class ShipmentOut(ControlledShipmentMixin, metaclass=PoolMeta):
     __name__ = 'stock.shipment.out'
 
     @classmethod
     @ModelView.button
@@ -62,17 +62,17 @@
         'receive', 'quality.wizard_stock_shipment_out_return_inspect_receive')
     def receive(cls, shipments):
         return super().receive(shipments)
 
     @classmethod
     @ModelView.button
     @ControlledMixin.control(
-        'done', 'quality.wizard_stock_shipment_out_return_inspect_done')
-    def done(cls, shipments):
-        return super().done(shipments)
+        'do', 'quality.wizard_stock_shipment_out_return_inspect_do')
+    def do(cls, shipments):
+        return super().do(shipments)
 
 
 class ShipmentInternal(ControlledShipmentMixin, metaclass=PoolMeta):
     __name__ = 'stock.shipment.internal'
 
     @classmethod
     @ModelView.button
@@ -80,10 +80,10 @@
         'ship', 'quality.wizard_stock_shipment_internal_inspect_ship')
     def ship(cls, shipments):
         return super().ship(shipments)
 
     @classmethod
     @ModelView.button
     @ControlledMixin.control(
-        'done', 'quality.wizard_stock_shipment_internal_inspect_done')
-    def done(cls, shipments):
-        return super().done(shipments)
+        'do', 'quality.wizard_stock_shipment_internal_inspect_do')
+    def do(cls, shipments):
+        return super().do(shipments)
```

### Comparing `trytond_quality-7.0.0/stock.xml` & `trytond_quality-7.2.0/stock.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_quality-7.0.0/stock.xml` & `trytond_quality-7.2.0/stock.xml`

```diff
@@ -9,23 +9,23 @@
       <field name="model">stock.shipment.in</field>
     </record>
     <record model="ir.action.keyword" id="wizard_stock_shipment_in_inspect_receive_keyword1">
       <field name="keyword">form_action</field>
       <field name="model">stock.shipment.in,-1</field>
       <field name="action" ref="wizard_stock_shipment_in_inspect_receive"/>
     </record>
-    <record model="ir.action.wizard" id="wizard_stock_shipment_in_inspect_done">
+    <record model="ir.action.wizard" id="wizard_stock_shipment_in_inspect_do">
       <field name="name">Inspect Done</field>
       <field name="wiz_name">quality.inspect</field>
       <field name="model">stock.shipment.in</field>
     </record>
-    <record model="ir.action.keyword" id="wizard_stock_shipment_in_inspect_done_keyword1">
+    <record model="ir.action.keyword" id="wizard_stock_shipment_in_inspect_do_keyword1">
       <field name="keyword">form_action</field>
       <field name="model">stock.shipment.in,-1</field>
-      <field name="action" ref="wizard_stock_shipment_in_inspect_done"/>
+      <field name="action" ref="wizard_stock_shipment_in_inspect_do"/>
     </record>
     <record model="ir.action.keyword" id="act_quality_inspection_form_relate_keyword_stock_shipment_in">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.in,-1</field>
       <field name="action" ref="act_quality_inspection_form_relate"/>
     </record>
     <record model="ir.action.wizard" id="wizard_stock_shipment_out_inspect_pick">
@@ -59,23 +59,23 @@
       <field name="model">stock.shipment.out.return</field>
     </record>
     <record model="ir.action.keyword" id="wizard_stock_shipment_out_return_inspect_receive_keyword1">
       <field name="keyword">form_action</field>
       <field name="model">stock.shipment.out.return,-1</field>
       <field name="action" ref="wizard_stock_shipment_out_return_inspect_receive"/>
     </record>
-    <record model="ir.action.wizard" id="wizard_stock_shipment_out_return_inspect_done">
+    <record model="ir.action.wizard" id="wizard_stock_shipment_out_return_inspect_do">
       <field name="name">Inspect Done</field>
       <field name="wiz_name">quality.inspect</field>
       <field name="model">stock.shipment.out.return</field>
     </record>
-    <record model="ir.action.keyword" id="wizard_stock_shipment_out_return_inspect_done_keyword1">
+    <record model="ir.action.keyword" id="wizard_stock_shipment_out_return_inspect_do_keyword1">
       <field name="keyword">form_action</field>
       <field name="model">stock.shipment.out.return,-1</field>
-      <field name="action" ref="wizard_stock_shipment_out_return_inspect_done"/>
+      <field name="action" ref="wizard_stock_shipment_out_return_inspect_do"/>
     </record>
     <record model="ir.action.keyword" id="act_quality_inspection_form_relate_keyword_stock_shipment_out_return">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.out.return,-1</field>
       <field name="action" ref="act_quality_inspection_form_relate"/>
     </record>
     <record model="ir.action.wizard" id="wizard_stock_shipment_internal_inspect_ship">
@@ -84,23 +84,23 @@
       <field name="model">stock.shipment.internal</field>
     </record>
     <record model="ir.action.keyword" id="wizard_stock_shipment_internal_inspect_ship_keyword1">
       <field name="keyword">form_action</field>
       <field name="model">stock.shipment.internal,-1</field>
       <field name="action" ref="wizard_stock_shipment_internal_inspect_ship"/>
     </record>
-    <record model="ir.action.wizard" id="wizard_stock_shipment_internal_inspect_done">
+    <record model="ir.action.wizard" id="wizard_stock_shipment_internal_inspect_do">
       <field name="name">Inspect Done</field>
       <field name="wiz_name">quality.inspect</field>
       <field name="model">stock.shipment.internal</field>
     </record>
-    <record model="ir.action.keyword" id="wizard_stock_shipment_internal_inspect_done_keyword1">
+    <record model="ir.action.keyword" id="wizard_stock_shipment_internal_inspect_do_keyword1">
       <field name="keyword">form_action</field>
       <field name="model">stock.shipment.internal,-1</field>
-      <field name="action" ref="wizard_stock_shipment_internal_inspect_done"/>
+      <field name="action" ref="wizard_stock_shipment_internal_inspect_do"/>
     </record>
     <record model="ir.action.keyword" id="act_quality_inspection_form_relate_keyword_stock_shipment_internal">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.internal,-1</field>
       <field name="action" ref="act_quality_inspection_form_relate"/>
     </record>
   </data>
```

### Comparing `trytond_quality-7.0.0/tests/scenario_quality_control_shipment.rst` & `trytond_quality-7.2.0/tests/scenario_quality_control_shipment.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 =================================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules(['quality', 'stock'])
 
     >>> Control = Model.get('quality.control')
     >>> Inspection = Model.get('quality.inspection')
@@ -72,15 +72,15 @@
     >>> shipment.state
     'draft'
 
     >>> inspection, = Inspection.find([])
     >>> inspection.state
     'failed'
 
-    >>> shipment.click('receive')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('receive')
     Traceback (most recent call last):
         ...
     InspectionError: ...
 
 Receive a product that passes quantity inspection::
 
     >>> inspection.click('pass_')
```

### Comparing `trytond_quality-7.0.0/tests/scenario_quality_inspection.rst` & `trytond_quality-7.2.0/tests/scenario_quality_inspection.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ===========================
 Quality Inspection Scenario
 ===========================
 
 Imports::
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('quality')
 
     >>> Control = Model.get('quality.control')
     >>> Inspection = Model.get('quality.inspection')
@@ -71,15 +71,15 @@
     'failed'
 
 Create a partial inspection::
 
     >>> inspection = Inspection()
     >>> inspection.control = control
     >>> inspection.points = {'boolean': True}
-    >>> inspection.click('process')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> inspection.click('process')
     Traceback (most recent call last):
         ...
     InspectionValidationError: ...
 
 Pass a failed inspection::
 
     >>> inspection = Inspection()
```

### Comparing `trytond_quality-7.0.0/tox.ini` & `trytond_quality-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/trytond_quality.egg-info/PKG-INFO` & `trytond_quality-7.2.0/trytond_quality.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-quality
-Version: 7.0.0
+Name: trytond_quality
+Version: 7.2.0
 Summary: Quality Management
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-quality
+Project-URL: Documentation, https://docs.tryton.org/modules-quality
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton quality QMS inspection
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 ##############
 Quality Module
 ##############
 
 The *Quality Module* enables quality to be controlled by configuring control
 points and inspecting against these when certain operations are performed.
```

### Comparing `trytond_quality-7.0.0/trytond_quality.egg-info/SOURCES.txt` & `trytond_quality-7.2.0/trytond_quality.egg-info/SOURCES.txt`

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

### Comparing `trytond_quality-7.0.0/view/quality_alert_form.xml` & `trytond_quality-7.2.0/view/quality_alert_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/view/quality_control_form.xml` & `trytond_quality-7.2.0/view/quality_control_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/view/quality_control_list.xml` & `trytond_quality-7.2.0/view/quality_control_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/view/quality_control_point_form.xml` & `trytond_quality-7.2.0/view/quality_control_point_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.0.0/view/quality_inspection_form.xml` & `trytond_quality-7.2.0/view/quality_inspection_form.xml`

 * *Files identical despite different names*

