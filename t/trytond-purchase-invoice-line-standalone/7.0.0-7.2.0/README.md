# Comparing `tmp/trytond_purchase_invoice_line_standalone-7.0.0.tar.gz` & `tmp/trytond_purchase_invoice_line_standalone-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_invoice_line_standalone-7.0.0.tar", last modified: Mon Oct 30 17:35:26 2023, max compression
+gzip compressed data, was "trytond_purchase_invoice_line_standalone-7.2.0.tar", last modified: Mon Apr 29 15:45:53 2024, max compression
```

## Comparing `trytond_purchase_invoice_line_standalone-7.0.0.tar` & `trytond_purchase_invoice_line_standalone-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:26.490370 trytond_purchase_invoice_line_standalone-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-22 17:23:14.000000 trytond_purchase_invoice_line_standalone-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3282 2023-10-30 17:10:36.000000 trytond_purchase_invoice_line_standalone-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:10:35.000000 trytond_purchase_invoice_line_standalone-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_invoice_line_standalone-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2789 2023-10-30 17:35:26.490370 trytond_purchase_invoice_line_standalone-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:26.487036 trytond_purchase_invoice_line_standalone-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2833 2023-10-22 17:23:14.000000 trytond_purchase_invoice_line_standalone-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3282 2023-10-30 17:10:36.000000 trytond_purchase_invoice_line_standalone-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:14.000000 trytond_purchase_invoice_line_standalone-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:26.487036 trytond_purchase_invoice_line_standalone-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1707 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1484 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1741 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1507 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1273 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1422 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1466 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1660 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1486 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1537 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1542 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1546 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-28 12:11:24.000000 trytond_purchase_invoice_line_standalone-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1247 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3563 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1311 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:35:26.490370 trytond_purchase_invoice_line_standalone-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4657 2023-10-27 17:38:49.000000 trytond_purchase_invoice_line_standalone-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:26.487036 trytond_purchase_invoice_line_standalone-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2536 2023-10-24 07:56:52.000000 trytond_purchase_invoice_line_standalone-7.0.0/tests/scenario_purchase_invoice_line_not_standalone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5052 2023-10-24 07:56:52.000000 trytond_purchase_invoice_line_standalone-7.0.0/tests/scenario_purchase_invoice_line_standalone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_invoice_line_standalone-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      134 2023-10-30 17:10:32.000000 trytond_purchase_invoice_line_standalone-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:26.490370 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2789 2023-10-30 17:35:25.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1922 2023-10-30 17:35:26.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:35:25.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-10-30 17:35:25.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-10-30 17:35:25.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:35:25.000000 trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:26.487036 trytond_purchase_invoice_line_standalone-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.0.0/view/invoice_line_tree_invoice_type.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-08-13 15:26:13.000000 trytond_purchase_invoice_line_standalone-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:53.770862 trytond_purchase_invoice_line_standalone-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3383 2024-04-29 15:23:44.000000 trytond_purchase_invoice_line_standalone-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:23:44.000000 trytond_purchase_invoice_line_standalone-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_invoice_line_standalone-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2789 2024-04-29 15:45:53.767529 trytond_purchase_invoice_line_standalone-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:53.764196 trytond_purchase_invoice_line_standalone-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-04-27 16:30:39.000000 trytond_purchase_invoice_line_standalone-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3383 2024-04-29 15:23:44.000000 trytond_purchase_invoice_line_standalone-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:21.000000 trytond_purchase_invoice_line_standalone-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:53.767529 trytond_purchase_invoice_line_standalone-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1707 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1484 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1741 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1507 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1273 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1422 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1501 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1466 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1660 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1486 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1537 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1565 2024-04-29 13:17:17.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:26.000000 trytond_purchase_invoice_line_standalone-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1247 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3791 2024-04-27 16:30:39.000000 trytond_purchase_invoice_line_standalone-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-22 12:14:36.000000 trytond_purchase_invoice_line_standalone-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:53.770862 trytond_purchase_invoice_line_standalone-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4657 2024-03-17 11:01:36.000000 trytond_purchase_invoice_line_standalone-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:53.767529 trytond_purchase_invoice_line_standalone-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2522 2024-04-22 12:14:36.000000 trytond_purchase_invoice_line_standalone-7.2.0/tests/scenario_purchase_invoice_line_not_standalone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4981 2024-04-22 12:14:36.000000 trytond_purchase_invoice_line_standalone-7.2.0/tests/scenario_purchase_invoice_line_standalone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:21.000000 trytond_purchase_invoice_line_standalone-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      134 2024-04-29 15:23:40.000000 trytond_purchase_invoice_line_standalone-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:53.767529 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2789 2024-04-29 15:45:53.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1822 2024-04-29 15:45:53.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:53.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-29 15:45:53.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:45:53.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:53.000000 trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:53.767529 trytond_purchase_invoice_line_standalone-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-01-27 09:58:52.000000 trytond_purchase_invoice_line_standalone-7.2.0/view/party_form.xml
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/CHANGELOG` & `trytond_purchase_invoice_line_standalone-7.2.0/CHANGELOG`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/LICENSE` & `trytond_purchase_invoice_line_standalone-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/PKG-INFO` & `trytond_purchase_invoice_line_standalone-7.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_invoice_line_standalone
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for standalone invoice line from purchase
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
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_invoice_line_standalone<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice_line_standalone<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #######################################
 Purchase Invoice Line Standalone Module
 #######################################
 
 The *Purchase Invoice Line Standalone Module* allows purchases to generate
 invoice lines instead of invoices.
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/__init__.py` & `trytond_purchase_invoice_line_standalone-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/doc/conf.py` & `trytond_purchase_invoice_line_standalone-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/doc/releases.rst` & `trytond_purchase_invoice_line_standalone-7.2.0/doc/releases.rst`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/bg.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/ca.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/cs.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/de.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/es.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/es_419.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/et.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/fa.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/fi.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/fr.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/hu.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/id.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/it.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/lo.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/lt.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/nl.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/pl.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/pt.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/ro.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/ro.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:party.party,purchase_invoice_line_standalone:"
 msgid "Purchase Invoice Line Standalone"
-msgstr "Achiziție - Rând Factură Ignorată"
+msgstr "Rând Factură de Achiziție Independentă"
 
 #, fuzzy
 msgctxt "field:party.party,purchase_invoice_lines_standalone:"
 msgid "Purchase Invoice Lines Standalone"
-msgstr "Achiziție - Rând Factură Ignorată"
+msgstr "Rând Facturi de Achiziție Independente"
 
+#, fuzzy
 msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 #, fuzzy
 msgctxt ""
 "field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
 msgid "Invoice Line Standalone"
-msgstr "Rânduri Factura Ignorate"
+msgstr "Rând Factură Independent"
 
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rânduri Factura"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/ru.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/sl.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/tr.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/uk.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/locale/zh_CN.po` & `trytond_purchase_invoice_line_standalone-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/party.py` & `trytond_purchase_invoice_line_standalone-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/purchase.py` & `trytond_purchase_invoice_line_standalone-7.2.0/purchase.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+
+from trytond import backend
 from trytond.model import ModelSQL, fields
 from trytond.pool import Pool, PoolMeta
 
 
 class Purchase(metaclass=PoolMeta):
     __name__ = 'purchase.purchase'
     invoice_lines = fields.Function(fields.Many2Many(
@@ -66,21 +68,27 @@
         default.setdefault('invoice_lines_ignored', None)
         return super(Purchase, cls).copy(purchases, default=default)
 
 
 class PurchaseIgnoredInvoiceLine(ModelSQL):
     'Purchase - Ignored Invoice Line'
     __name__ = 'purchase.purchase-ignored-account.invoice.line'
-    _table = 'purchase_invoice_line_ignored_rel'
     purchase = fields.Many2One(
         'purchase.purchase', "Purchase", ondelete='CASCADE', required=True)
     invoice = fields.Many2One(
         'account.invoice.line', "Invoice Line",
         ondelete='RESTRICT', required=True)
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'purchase_invoice_line_ignored_rel', cls._table)
+        super().__register__(module)
+
 
 class HandleInvoiceException(metaclass=PoolMeta):
     __name__ = 'purchase.handle.invoice.exception'
 
     def transition_handle(self):
         state = super(HandleInvoiceException, self).transition_handle()
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/purchase.xml` & `trytond_purchase_invoice_line_standalone-7.2.0/purchase.xml`

 * *Files 15% similar despite different names*

#### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/purchase.xml` & `trytond_purchase_invoice_line_standalone-7.2.0/purchase.xml`

```diff
@@ -1,18 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data>
-    <record model="ir.ui.view" id="invoice_line_invoice_type">
-      <field name="model">account.invoice.line</field>
-      <field name="type">tree</field>
-      <field name="priority" eval="30"/>
-      <field name="name">invoice_line_tree_invoice_type</field>
-    </record>
     <record model="ir.action.act_window" id="act_purchase_invoice_line_relate">
       <field name="name">Invoice Lines</field>
       <field name="res_model">account.invoice.line</field>
       <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('origin.purchase.id', '=', Eval('active_id'), 'purchase.line'), ('origin.purchase.id', 'in', Eval('active_ids'), 'purchase.line'))]" pyson="1"/>
     </record>
     <record model="ir.action.keyword" id="act_invoice_line_form_keyword1">
       <field name="keyword">form_relate</field>
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/setup.py` & `trytond_purchase_invoice_line_standalone-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/tests/scenario_purchase_invoice_line_not_standalone.rst` & `trytond_purchase_invoice_line_standalone-7.2.0/tests/scenario_purchase_invoice_line_not_standalone.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =============================================
 Purchase Invoice Line Not Standalone Scenario
 =============================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('purchase_invoice_line_standalone')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/tests/scenario_purchase_invoice_line_standalone.rst` & `trytond_purchase_invoice_line_standalone-7.2.0/tests/scenario_purchase_invoice_line_standalone.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 =========================================
 Purchase Invoice Line Standalone Scenario
 =========================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> current_config = activate_modules('purchase_invoice_line_standalone')
 
 Create company::
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/tox.ini` & `trytond_purchase_invoice_line_standalone-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO` & `trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-invoice-line-standalone
-Version: 7.0.0
+Name: trytond_purchase_invoice_line_standalone
+Version: 7.2.0
 Summary: Tryton module for standalone invoice line from purchase
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
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_invoice_line_standalone<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice_line_standalone<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #######################################
 Purchase Invoice Line Standalone Module
 #######################################
 
 The *Purchase Invoice Line Standalone Module* allows purchases to generate
 invoice lines instead of invoices.
```

### Comparing `trytond_purchase_invoice_line_standalone-7.0.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt` & `trytond_purchase_invoice_line_standalone-7.2.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 party.py
@@ -43,15 +42,14 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_purchase_invoice_line_not_standalone.rst
 ./tests/scenario_purchase_invoice_line_standalone.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
-./view/invoice_line_tree_invoice_type.xml
 ./view/party_form.xml
 doc/conf.py
 doc/index.rst
 doc/releases.rst
 doc/requirements-doc.txt
 doc/usage.rst
 locale/bg.po
@@ -86,9 +84,8 @@
 trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO
 trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt
 trytond_purchase_invoice_line_standalone.egg-info/dependency_links.txt
 trytond_purchase_invoice_line_standalone.egg-info/entry_points.txt
 trytond_purchase_invoice_line_standalone.egg-info/not-zip-safe
 trytond_purchase_invoice_line_standalone.egg-info/requires.txt
 trytond_purchase_invoice_line_standalone.egg-info/top_level.txt
-view/invoice_line_tree_invoice_type.xml
 view/party_form.xml
```

