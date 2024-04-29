# Comparing `tmp/trytond_sale_invoice_date-7.0.1.tar.gz` & `tmp/trytond_sale_invoice_date-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_invoice_date-7.0.1.tar", last modified: Fri Nov 17 18:47:48 2023, max compression
+gzip compressed data, was "trytond_sale_invoice_date-7.2.0.tar", last modified: Mon Apr 29 15:48:09 2024, max compression
```

## Comparing `trytond_sale_invoice_date-7.0.1.tar` & `trytond_sale_invoice_date-7.2.0.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:47:48.729399 trytond_sale_invoice_date-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-11-17 18:47:46.000000 trytond_sale_invoice_date-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-11-17 18:47:45.000000 trytond_sale_invoice_date-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2667 2023-11-17 18:47:48.729399 trytond_sale_invoice_date-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:47:48.729399 trytond_sale_invoice_date-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:47:48.726066 trytond_sale_invoice_date-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2396 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2414 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2457 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1893 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2036 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2330 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1426 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4206 2023-11-15 17:15:53.000000 trytond_sale_invoice_date-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3842 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-11-17 18:47:48.729399 trytond_sale_invoice_date-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4628 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:47:48.726066 trytond_sale_invoice_date-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2892 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/tests/scenario_sale_invoice_date.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2023-10-30 17:55:12.000000 trytond_sale_invoice_date-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:47:48.729399 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2667 2023-11-17 18:47:48.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-11-17 18:47:48.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-11-17 18:47:48.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-11-17 18:47:48.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:06.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      107 2023-11-17 18:47:48.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-11-17 18:47:48.000000 trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:47:48.729399 trytond_sale_invoice_date-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/invoice_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/invoice_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      647 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/invoice_term_relative_delta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/invoice_term_relative_delta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/invoice_term_relative_delta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:38.000000 trytond_sale_invoice_date-7.0.1/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:09.267318 trytond_sale_invoice_date-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:25:22.000000 trytond_sale_invoice_date-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:25:22.000000 trytond_sale_invoice_date-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2730 2024-04-29 15:48:09.267318 trytond_sale_invoice_date-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:09.260652 trytond_sale_invoice_date-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_sale_invoice_date-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:25.000000 trytond_sale_invoice_date-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:09.263985 trytond_sale_invoice_date-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2428 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2396 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2414 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2457 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1893 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2036 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2330 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-27 16:43:26.000000 trytond_sale_invoice_date-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1426 2024-01-27 09:58:52.000000 trytond_sale_invoice_date-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1147 2024-04-27 16:30:39.000000 trytond_sale_invoice_date-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4206 2024-04-27 16:30:39.000000 trytond_sale_invoice_date-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3796 2024-04-27 16:30:39.000000 trytond_sale_invoice_date-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:09.267318 trytond_sale_invoice_date-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4688 2024-04-27 16:30:39.000000 trytond_sale_invoice_date-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:09.263985 trytond_sale_invoice_date-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2886 2024-04-22 12:14:36.000000 trytond_sale_invoice_date-7.2.0/tests/scenario_sale_invoice_date.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      901 2024-04-27 16:30:39.000000 trytond_sale_invoice_date-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:25.000000 trytond_sale_invoice_date-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-04-29 15:25:18.000000 trytond_sale_invoice_date-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:09.267318 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2730 2024-04-29 15:48:08.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2044 2024-04-29 15:48:09.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:08.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:48:08.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-29 15:48:08.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:08.000000 trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:09.267318 trytond_sale_invoice_date-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/invoice_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/invoice_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      647 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/invoice_term_relative_delta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/invoice_term_relative_delta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/invoice_term_relative_delta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_sale_invoice_date-7.2.0/view/sale_form.xml
```

### Comparing `trytond_sale_invoice_date-7.0.1/CHANGELOG` & `trytond_sale_invoice_date-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2023-11-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_invoice_date-7.0.1/COPYRIGHT` & `trytond_sale_invoice_date-7.2.0/COPYRIGHT`

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

### Comparing `trytond_sale_invoice_date-7.0.1/LICENSE` & `trytond_sale_invoice_date-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/PKG-INFO` & `trytond_sale_invoice_date-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale_invoice_date
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to compute invoice date of sale
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-invoice-date
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-invoice-date
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale invoice date
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_invoice_grouping<7.3,>=7.2; extra == "test"
 
 ########################
 Sale Invoice Date Module
 ########################
 
 The *Sale Invoice Date Module* fills the invoice date of invoices created by sales.
```

### Comparing `trytond_sale_invoice_date-7.0.1/__init__.py` & `trytond_sale_invoice_date-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/doc/conf.py` & `trytond_sale_invoice_date-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_invoice_date-7.0.1/doc/design.rst` & `trytond_sale_invoice_date-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/bg.po` & `trytond_sale_invoice_date-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/ca.po` & `trytond_sale_invoice_date-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/cs.po` & `trytond_sale_invoice_date-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/de.po` & `trytond_sale_invoice_date-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/es.po` & `trytond_sale_invoice_date-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/es_419.po` & `trytond_sale_invoice_date-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/et.po` & `trytond_sale_invoice_date-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/fa.po` & `trytond_sale_invoice_date-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/fi.po` & `trytond_sale_invoice_date-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/fr.po` & `trytond_sale_invoice_date-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/hu.po` & `trytond_sale_invoice_date-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/id.po` & `trytond_sale_invoice_date-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/it.po` & `trytond_sale_invoice_date-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/lo.po` & `trytond_sale_invoice_date-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/lt.po` & `trytond_sale_invoice_date-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/nl.po` & `trytond_sale_invoice_date-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/pl.po` & `trytond_sale_invoice_date-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/pt.po` & `trytond_sale_invoice_date-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/ro.po` & `trytond_sale_invoice_date-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/ru.po` & `trytond_sale_invoice_date-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/sl.po` & `trytond_sale_invoice_date-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/tr.po` & `trytond_sale_invoice_date-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/uk.po` & `trytond_sale_invoice_date-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/locale/zh_CN.po` & `trytond_sale_invoice_date-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/party.py` & `trytond_sale_invoice_date-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/party.xml` & `trytond_sale_invoice_date-7.2.0/party.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_sale_invoice_date-7.0.1/party.xml` & `trytond_sale_invoice_date-7.2.0/party.xml`

```diff
@@ -5,19 +5,21 @@
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_invoice_term">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_invoice_term')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_invoice_term</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_invoice_term_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_invoice_term')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_invoice_term</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale_invoice_date-7.0.1/sale.py` & `trytond_sale_invoice_date-7.2.0/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,9 +125,9 @@
         invoice = super()._get_invoice_sale()
         if self.invoice_term:
             invoice.invoice_date = self.invoice_term.get_date(
                 date=self._invoice_term_date)
         return invoice
 
     def _get_invoice_grouping_fields(self, invoice):
-        return super()._get_invoice_grouping_fields(invoice) + [
-            'invoice_date']
+        return super()._get_invoice_grouping_fields(invoice) | {
+            'invoice_date'}
```

### Comparing `trytond_sale_invoice_date-7.0.1/sale.xml` & `trytond_sale_invoice_date-7.2.0/sale.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale_invoice_date-7.0.1/sale.xml` & `trytond_sale_invoice_date-7.2.0/sale.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_invoice_term_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="invoice_term_view_form"/>
       <field name="act_window" ref="act_invoice_term_form"/>
     </record>
     <menuitem parent="sale.menu_configuration" action="act_invoice_term_form" sequence="20" id="menu_invoice_term_form"/>
     <record model="ir.model.access" id="access_invoice_term">
-      <field name="model" search="[('model', '=', 'sale.invoice.term')]"/>
+      <field name="model">sale.invoice.term</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_term_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.invoice.term')]"/>
+      <field name="model">sale.invoice.term</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="invoice_term_relative_delta_view_form">
```

### Comparing `trytond_sale_invoice_date-7.0.1/setup.py` & `trytond_sale_invoice_date-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,31 @@
 
 requires = ['python-dateutil']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond_sale_invoice_grouping'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module to compute invoice date of sale',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-sale-invoice-date'),
+            'https://docs.tryton.org/modules-sale-invoice-date'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale invoice date',
     package_dir={'trytond.modules.sale_invoice_date': '.'},
     packages=(
         ['trytond.modules.sale_invoice_date']
```

### Comparing `trytond_sale_invoice_date-7.0.1/tests/scenario_sale_invoice_date.rst` & `trytond_sale_invoice_date-7.2.0/tests/scenario_sale_invoice_date.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from dateutil.relativedelta import relativedelta
 
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
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> end_month = today + relativedelta(day=31)
 
 Activate modules::
 
     >>> config = activate_modules('sale_invoice_date')
@@ -82,22 +81,20 @@
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
 
 Make a sale::
 
     >>> sale = Sale(party=customer)
-    >>> sale.invoice_term == invoice_term
-    True
+    >>> assertEqual(sale.invoice_term, invoice_term)
     >>> line = sale.lines.new()
     >>> line.product = product
     >>> line.quantity = 1
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> sale.state
     'processing'
 
 Check invoice date::
 
     >>> invoice, = sale.invoices
-    >>> invoice.invoice_date == end_month
-    True
+    >>> assertEqual(invoice.invoice_date, end_month)
```

### Comparing `trytond_sale_invoice_date-7.0.1/tox.ini` & `trytond_sale_invoice_date-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/PKG-INFO` & `trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-sale-invoice-date
-Version: 7.0.1
+Name: trytond_sale_invoice_date
+Version: 7.2.0
 Summary: Tryton module to compute invoice date of sale
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-invoice-date
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-invoice-date
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale invoice date
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_invoice_grouping<7.3,>=7.2; extra == "test"
 
 ########################
 Sale Invoice Date Module
 ########################
 
 The *Sale Invoice Date Module* fills the invoice date of invoices created by sales.
```

### Comparing `trytond_sale_invoice_date-7.0.1/trytond_sale_invoice_date.egg-info/SOURCES.txt` & `trytond_sale_invoice_date-7.2.0/trytond_sale_invoice_date.egg-info/SOURCES.txt`

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
 party.py
```

### Comparing `trytond_sale_invoice_date-7.0.1/view/invoice_term_relative_delta_form.xml` & `trytond_sale_invoice_date-7.2.0/view/invoice_term_relative_delta_form.xml`

 * *Files identical despite different names*

