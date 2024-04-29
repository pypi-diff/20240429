# Comparing `tmp/trytond_sale_invoice_grouping-7.0.0.tar.gz` & `tmp/trytond_sale_invoice_grouping-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_invoice_grouping-7.0.0.tar", last modified: Mon Oct 30 17:38:20 2023, max compression
+gzip compressed data, was "trytond_sale_invoice_grouping-7.2.0.tar", last modified: Mon Apr 29 15:48:15 2024, max compression
```

## Comparing `trytond_sale_invoice_grouping-7.0.0.tar` & `trytond_sale_invoice_grouping-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:20.061197 trytond_sale_invoice_grouping-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:23:18.000000 trytond_sale_invoice_grouping-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1887 2023-10-30 17:12:14.000000 trytond_sale_invoice_grouping-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      689 2023-10-30 17:12:13.000000 trytond_sale_invoice_grouping-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3149 2023-10-30 17:38:20.061197 trytond_sale_invoice_grouping-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      479 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1378 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:20.057864 trytond_sale_invoice_grouping-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:23:18.000000 trytond_sale_invoice_grouping-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:18.000000 trytond_sale_invoice_grouping-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:20.057864 trytond_sale_invoice_grouping-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1425 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1830 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1792 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1723 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1950 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1862 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1892 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1840 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1792 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1384 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1441 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1663 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-10-28 12:11:25.000000 trytond_sale_invoice_grouping-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1552 2023-08-13 15:26:13.000000 trytond_sale_invoice_grouping-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-08-13 15:26:13.000000 trytond_sale_invoice_grouping-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:38:20.061197 trytond_sale_invoice_grouping-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4477 2023-10-27 17:38:49.000000 trytond_sale_invoice_grouping-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:20.057864 trytond_sale_invoice_grouping-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5882 2023-06-10 11:39:56.000000 trytond_sale_invoice_grouping-7.0.0/tests/scenario_sale_invoice_grouping.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/tests/scenario_sale_invoice_grouping_multiple.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_invoice_grouping-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-10-30 17:12:10.000000 trytond_sale_invoice_grouping-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:20.061197 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3149 2023-10-30 17:38:19.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-10-30 17:38:20.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:38:19.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:38:19.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      125 2023-10-30 17:38:19.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:38:19.000000 trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:20.057864 trytond_sale_invoice_grouping-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:15.617152 trytond_sale_invoice_grouping-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1988 2024-04-29 15:25:27.000000 trytond_sale_invoice_grouping-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      689 2024-04-29 15:25:27.000000 trytond_sale_invoice_grouping-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3149 2024-04-29 15:48:15.617152 trytond_sale_invoice_grouping-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      479 2024-04-26 08:56:10.000000 trytond_sale_invoice_grouping-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1378 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:15.613819 trytond_sale_invoice_grouping-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_sale_invoice_grouping-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:26.000000 trytond_sale_invoice_grouping-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:15.613819 trytond_sale_invoice_grouping-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1425 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1830 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1792 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1723 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1950 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1862 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1393 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1892 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1840 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1792 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1384 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1441 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1663 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2024-04-27 16:43:26.000000 trytond_sale_invoice_grouping-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-01-27 09:58:52.000000 trytond_sale_invoice_grouping-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2024-04-27 16:30:39.000000 trytond_sale_invoice_grouping-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:15.617152 trytond_sale_invoice_grouping-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4477 2024-03-17 11:01:36.000000 trytond_sale_invoice_grouping-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:15.617152 trytond_sale_invoice_grouping-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5823 2024-04-22 12:14:36.000000 trytond_sale_invoice_grouping-7.2.0/tests/scenario_sale_invoice_grouping.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2813 2024-04-22 12:14:36.000000 trytond_sale_invoice_grouping-7.2.0/tests/scenario_sale_invoice_grouping_multiple.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:26.000000 trytond_sale_invoice_grouping-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2024-04-29 15:25:23.000000 trytond_sale_invoice_grouping-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:15.617152 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3149 2024-04-29 15:48:15.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1776 2024-04-29 15:48:15.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:15.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:48:15.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      125 2024-04-29 15:48:15.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:15.000000 trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:15.617152 trytond_sale_invoice_grouping-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-7.2.0/view/party_form.xml
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/CHANGELOG` & `trytond_sale_invoice_grouping-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_sale_invoice_grouping-7.0.0/COPYRIGHT` & `trytond_sale_invoice_grouping-7.2.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Copyright (C) 2013-2023 Nicolas Évrard.
-Copyright (C) 2013-2023 B2CK SPRL.
+Copyright (C) 2013-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/LICENSE` & `trytond_sale_invoice_grouping-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/PKG-INFO` & `trytond_sale_invoice_grouping-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_invoice_grouping
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to group sale invoices
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
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Invoice Grouping Module
 ############################
 
 The ``sale_invoice_grouping`` module adds an option to define how invoice lines
 generated from sales will be grouped.
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/README.rst` & `trytond_sale_invoice_grouping-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/configuration.py` & `trytond_sale_invoice_grouping-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/doc/conf.py` & `trytond_sale_invoice_grouping-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_sale_invoice_grouping-7.0.0/doc/index.rst` & `trytond_sale_invoice_grouping-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/bg.po` & `trytond_sale_invoice_grouping-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/ca.po` & `trytond_sale_invoice_grouping-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/cs.po` & `trytond_sale_invoice_grouping-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/de.po` & `trytond_sale_invoice_grouping-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/es.po` & `trytond_sale_invoice_grouping-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/es_419.po` & `trytond_sale_invoice_grouping-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/et.po` & `trytond_sale_invoice_grouping-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/fa.po` & `trytond_sale_invoice_grouping-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/fi.po` & `trytond_sale_invoice_grouping-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/fr.po` & `trytond_sale_invoice_grouping-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/hu.po` & `trytond_sale_invoice_grouping-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/id.po` & `trytond_sale_invoice_grouping-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/it.po` & `trytond_sale_invoice_grouping-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/lo.po` & `trytond_sale_invoice_grouping-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/lt.po` & `trytond_sale_invoice_grouping-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/nl.po` & `trytond_sale_invoice_grouping-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/pl.po` & `trytond_sale_invoice_grouping-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/pt.po` & `trytond_sale_invoice_grouping-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/ro.po` & `trytond_sale_invoice_grouping-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/ru.po` & `trytond_sale_invoice_grouping-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/sl.po` & `trytond_sale_invoice_grouping-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/tr.po` & `trytond_sale_invoice_grouping-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/uk.po` & `trytond_sale_invoice_grouping-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/locale/zh_CN.po` & `trytond_sale_invoice_grouping-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/party.py` & `trytond_sale_invoice_grouping-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/sale.py` & `trytond_sale_invoice_grouping-7.2.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
     @property
     def invoice_grouping_method(self):
         party = self.invoice_party or self.party
         return party.sale_invoice_grouping_method
 
     def _get_invoice_grouping_fields(self, invoice):
-        return ['state', 'company', 'type', 'journal', 'party',
-            'invoice_address', 'currency', 'account', 'payment_term']
+        return {'state', 'company', 'type', 'journal', 'party',
+            'invoice_address', 'currency', 'account', 'payment_term'}
 
     def _get_grouped_invoice_order(self):
         "Returns the order clause used to find invoice that should be grouped"
         return None
 
     def _get_grouped_invoice_domain(self, invoice):
         "Returns a domain that will find invoices that should be grouped"
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/setup.py` & `trytond_sale_invoice_grouping-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/tests/scenario_sale_invoice_grouping.rst` & `trytond_sale_invoice_grouping-7.2.0/tests/scenario_sale_invoice_grouping.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ==============================
 Sale Invoice Grouping Scenario
 ==============================
 
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
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_invoice_grouping')
 
 Create company::
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/tests/scenario_sale_invoice_grouping_multiple.rst` & `trytond_sale_invoice_grouping-7.2.0/tests/scenario_sale_invoice_grouping_multiple.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 Sale Invoice Grouping Multiple Scenario
 =======================================
 
 Imports::
 
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
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale_invoice_grouping')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/tox.ini` & `trytond_sale_invoice_grouping-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO` & `trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-invoice-grouping
-Version: 7.0.0
+Name: trytond_sale_invoice_grouping
+Version: 7.2.0
 Summary: Tryton module to group sale invoices
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
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Invoice Grouping Module
 ############################
 
 The ``sale_invoice_grouping`` module adds an option to define how invoice lines
 generated from sales will be grouped.
```

### Comparing `trytond_sale_invoice_grouping-7.0.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt` & `trytond_sale_invoice_grouping-7.2.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt`

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
 configuration.py
```

