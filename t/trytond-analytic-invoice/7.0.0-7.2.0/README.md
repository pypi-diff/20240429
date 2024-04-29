# Comparing `tmp/trytond_analytic_invoice-7.0.0.tar.gz` & `tmp/trytond_analytic_invoice-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_invoice-7.0.0.tar", last modified: Mon Oct 30 17:26:43 2023, max compression
+gzip compressed data, was "trytond_analytic_invoice-7.2.0.tar", last modified: Mon Apr 29 15:37:51 2024, max compression
```

## Comparing `trytond_analytic_invoice-7.0.0.tar` & `trytond_analytic_invoice-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:43.247874 trytond_analytic_invoice-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:22:59.000000 trytond_analytic_invoice-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2765 2023-10-30 17:04:37.000000 trytond_analytic_invoice-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:04:37.000000 trytond_analytic_invoice-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2802 2023-10-30 17:26:43.247874 trytond_analytic_invoice-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-10-07 15:40:36.000000 trytond_analytic_invoice-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2565 2023-08-13 15:26:13.000000 trytond_analytic_invoice-7.0.0/asset.py
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.0.0/asset.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:43.244541 trytond_analytic_invoice-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:22:59.000000 trytond_analytic_invoice-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:59.000000 trytond_analytic_invoice-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     4189 2023-10-07 15:40:36.000000 trytond_analytic_invoice-7.0.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.0.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:43.241207 trytond_analytic_invoice-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      595 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      600 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      648 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      595 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-10-28 12:11:21.000000 trytond_analytic_invoice-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:26:43.247874 trytond_analytic_invoice-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4572 2023-10-27 17:38:49.000000 trytond_analytic_invoice-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:43.244541 trytond_analytic_invoice-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-06-10 11:39:56.000000 trytond_analytic_invoice-7.0.0/tests/scenario_analytic_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5113 2023-08-13 15:26:13.000000 trytond_analytic_invoice-7.0.0/tests/scenario_analytic_invoice_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3881 2023-10-07 15:40:36.000000 trytond_analytic_invoice-7.0.0/tests/scenario_analytic_invoice_defer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-07 15:40:36.000000 trytond_analytic_invoice-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_analytic_invoice-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-10-30 17:04:32.000000 trytond_analytic_invoice-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:43.244541 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2802 2023-10-30 17:26:42.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1775 2023-10-30 17:26:43.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:26:42.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:26:42.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:26:42.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:26:42.000000 trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:43.244541 trytond_analytic_invoice-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.0.0/view/asset_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.0.0/view/invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:51.310147 trytond_analytic_invoice-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2866 2024-04-29 15:17:44.000000 trytond_analytic_invoice-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:17:44.000000 trytond_analytic_invoice-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2802 2024-04-29 15:37:51.310147 trytond_analytic_invoice-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-02-04 18:51:26.000000 trytond_analytic_invoice-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2565 2024-01-27 09:58:52.000000 trytond_analytic_invoice-7.2.0/asset.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.2.0/asset.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:51.306814 trytond_analytic_invoice-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_analytic_invoice-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:04.000000 trytond_analytic_invoice-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     4189 2024-02-04 18:51:26.000000 trytond_analytic_invoice-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.2.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:51.306814 trytond_analytic_invoice-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      595 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      601 2024-04-29 13:17:17.000000 trytond_analytic_invoice-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      648 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      595 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-27 16:43:22.000000 trytond_analytic_invoice-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:51.310147 trytond_analytic_invoice-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4572 2024-03-17 11:01:36.000000 trytond_analytic_invoice-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:51.310147 trytond_analytic_invoice-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3786 2024-04-22 12:14:36.000000 trytond_analytic_invoice-7.2.0/tests/scenario_analytic_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5028 2024-04-22 12:14:36.000000 trytond_analytic_invoice-7.2.0/tests/scenario_analytic_invoice_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3877 2024-04-22 12:14:36.000000 trytond_analytic_invoice-7.2.0/tests/scenario_analytic_invoice_defer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-02-04 18:51:26.000000 trytond_analytic_invoice-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_invoice-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:04.000000 trytond_analytic_invoice-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-04-29 15:17:40.000000 trytond_analytic_invoice-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:51.310147 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2802 2024-04-29 15:37:50.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1757 2024-04-29 15:37:51.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:50.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:37:50.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-29 15:37:50.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:50.000000 trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:51.310147 trytond_analytic_invoice-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.2.0/view/asset_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_analytic_invoice-7.2.0/view/invoice_line_form.xml
```

### Comparing `trytond_analytic_invoice-7.0.0/CHANGELOG` & `trytond_analytic_invoice-7.2.0/CHANGELOG`

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
 * Fill analytic lines when defer invoice
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_analytic_invoice-7.0.0/COPYRIGHT` & `trytond_analytic_invoice-7.2.0/COPYRIGHT`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2012 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_analytic_invoice-7.0.0/LICENSE` & `trytond_analytic_invoice-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/PKG-INFO` & `trytond_analytic_invoice-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_invoice
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add analytic accounting on invoice
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
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_analytic_account<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_analytic_account<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_asset<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_defer<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_asset<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_defer<7.3,>=7.2; extra == "test"
 
 Analytic Invoice Module
 #######################
 
 The analytic invoice modules allows to set analytic accounts on invoice line.
```

### Comparing `trytond_analytic_invoice-7.0.0/__init__.py` & `trytond_analytic_invoice-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/asset.py` & `trytond_analytic_invoice-7.2.0/asset.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/doc/conf.py` & `trytond_analytic_invoice-7.2.0/doc/conf.py`

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

### Comparing `trytond_analytic_invoice-7.0.0/invoice.py` & `trytond_analytic_invoice-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/bg.po` & `trytond_analytic_invoice-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/ca.po` & `trytond_analytic_invoice-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/de.po` & `trytond_analytic_invoice-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/es.po` & `trytond_analytic_invoice-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/es_419.po` & `trytond_analytic_invoice-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/et.po` & `trytond_analytic_invoice-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/fa.po` & `trytond_analytic_invoice-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/fr.po` & `trytond_analytic_invoice-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/it.po` & `trytond_analytic_invoice-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/lo.po` & `trytond_analytic_invoice-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/nl.po` & `trytond_analytic_invoice-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/pt.po` & `trytond_analytic_invoice-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/ro.po` & `trytond_analytic_invoice-7.2.0/locale/ro.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 msgctxt "field:account.asset,analytic_accounts:"
 msgid "Analytic Accounts"
 msgstr "Conturi Analitice"
 
 msgctxt "field:account.asset,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr "Conturi Analitice Marime"
+msgstr "Conturi Analitice Mărime"
 
 msgctxt "field:account.invoice.line,analytic_accounts:"
 msgid "Analytic Accounts"
-msgstr "Conturi analitice"
+msgstr "Conturi Analitice"
 
 msgctxt "field:account.invoice.line,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr "Mărimea conturilor analitice"
+msgstr "Mărimea Conturilor Analitice"
 
 msgctxt "view:account.invoice.line:"
 msgid "Analytic"
 msgstr "Analitic"
```

### Comparing `trytond_analytic_invoice-7.0.0/locale/ru.po` & `trytond_analytic_invoice-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/locale/sl.po` & `trytond_analytic_invoice-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/setup.py` & `trytond_analytic_invoice-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/tests/scenario_analytic_invoice.rst` & `trytond_analytic_invoice-7.2.0/tests/scenario_analytic_invoice.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 =========================
 Analytic Invoice Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('analytic_invoice')
 
 Create company::
 
@@ -84,16 +83,15 @@
 
     >>> Invoice = Model.get('account.invoice')
     >>> invoice = Invoice()
     >>> invoice.party = party
     >>> invoice.payment_term = payment_term
     >>> line = invoice.lines.new()
     >>> entry, = line.analytic_accounts
-    >>> entry.root == root
-    True
+    >>> assertEqual(entry.root, root)
     >>> entry.account = analytic_account
     >>> line.product = product
     >>> line.quantity = 5
     >>> line.unit_price = Decimal('40')
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
```

### Comparing `trytond_analytic_invoice-7.0.0/tests/scenario_analytic_invoice_asset.rst` & `trytond_analytic_invoice-7.2.0/tests/scenario_analytic_invoice_asset.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 =====================================
 Analytic Invoice with Assets Scenario
 =====================================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
+
+    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_asset.tests.tools import add_asset_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> from trytond.modules.account_asset.tests.tools \
-    ...     import add_asset_accounts
 
     >>> today = dt.date.today()
     >>> next_month = today + relativedelta(day=1, month=1)
     >>> next_next_month = next_month + relativedelta(months=1)
 
 Activate modules::
```

### Comparing `trytond_analytic_invoice-7.0.0/tests/scenario_analytic_invoice_defer.rst` & `trytond_analytic_invoice-7.2.0/tests/scenario_analytic_invoice_defer.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 ===============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
     >>> from trytond.modules.account_invoice_defer.tests.tools import (
     ...     add_deferred_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['analytic_invoice', 'account_invoice_defer'])
 
@@ -103,22 +102,19 @@
     >>> analytic_account.reload()
     >>> analytic_account.debit, analytic_account.credit
     (Decimal('1000.00'), Decimal('0.00'))
 
 Check invoice deferred and run it::
 
     >>> deferral, = InvoiceDeferred.find([])
-    >>> deferral.invoice_line == invoice_line
-    True
+    >>> assertEqual(deferral.invoice_line, invoice_line)
     >>> deferral.amount
     Decimal('1000.00')
-    >>> deferral.start_date == invoice_line.defer_from
-    True
-    >>> deferral.end_date == invoice_line.defer_to
-    True
+    >>> assertEqual(deferral.start_date, invoice_line.defer_from)
+    >>> assertEqual(deferral.end_date, invoice_line.defer_to)
     >>> deferral.click('run')
     >>> deferral.state
     'running'
     >>> len(deferral.moves)
     13
 
     >>> analytic_account.reload()
```

### Comparing `trytond_analytic_invoice-7.0.0/tox.ini` & `trytond_analytic_invoice-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/PKG-INFO` & `trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-analytic-invoice
-Version: 7.0.0
+Name: trytond_analytic_invoice
+Version: 7.2.0
 Summary: Tryton module to add analytic accounting on invoice
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
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_analytic_account<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_analytic_account<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_asset<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_defer<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_asset<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_defer<7.3,>=7.2; extra == "test"
 
 Analytic Invoice Module
 #######################
 
 The analytic invoice modules allows to set analytic accounts on invoice line.
```

### Comparing `trytond_analytic_invoice-7.0.0/trytond_analytic_invoice.egg-info/SOURCES.txt` & `trytond_analytic_invoice-7.2.0/trytond_analytic_invoice.egg-info/SOURCES.txt`

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
 asset.py
```

