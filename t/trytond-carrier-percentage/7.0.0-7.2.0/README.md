# Comparing `tmp/trytond_carrier_percentage-7.0.0.tar.gz` & `tmp/trytond_carrier_percentage-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_percentage-7.0.0.tar", last modified: Mon Oct 30 17:27:59 2023, max compression
+gzip compressed data, was "trytond_carrier_percentage-7.2.0.tar", last modified: Mon Apr 29 15:38:48 2024, max compression
```

## Comparing `trytond_carrier_percentage-7.0.0.tar` & `trytond_carrier_percentage-7.2.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:59.058236 trytond_carrier_percentage-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:01.000000 trytond_carrier_percentage-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2068 2023-10-30 17:05:20.000000 trytond_carrier_percentage-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:05:19.000000 trytond_carrier_percentage-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-10-30 17:27:59.058236 trytond_carrier_percentage-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.0.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:59.054902 trytond_carrier_percentage-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:01.000000 trytond_carrier_percentage-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:01.000000 trytond_carrier_percentage-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:59.054902 trytond_carrier_percentage-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-28 12:11:21.000000 trytond_carrier_percentage-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      956 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:27:59.058236 trytond_carrier_percentage-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4638 2023-10-27 17:38:49.000000 trytond_carrier_percentage-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2155 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:59.054902 trytond_carrier_percentage-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6880 2023-06-10 11:39:56.000000 trytond_carrier_percentage-7.0.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_carrier_percentage-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-10-30 17:05:16.000000 trytond_carrier_percentage-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:59.058236 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-10-30 17:27:58.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-10-30 17:27:59.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:27:58.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:27:58.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:27:58.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:27:58.000000 trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:59.054902 trytond_carrier_percentage-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.0.0/view/carrier_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:48.701979 trytond_carrier_percentage-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2169 2024-04-29 15:18:30.000000 trytond_carrier_percentage-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:18:30.000000 trytond_carrier_percentage-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2024-04-29 15:38:48.701979 trytond_carrier_percentage-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:48.698646 trytond_carrier_percentage-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_carrier_percentage-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:06.000000 trytond_carrier_percentage-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:48.698646 trytond_carrier_percentage-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-27 16:43:22.000000 trytond_carrier_percentage-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      956 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:48.701979 trytond_carrier_percentage-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4638 2024-03-17 11:01:36.000000 trytond_carrier_percentage-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2155 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:48.698646 trytond_carrier_percentage-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6880 2024-04-27 16:30:39.000000 trytond_carrier_percentage-7.2.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_percentage-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:06.000000 trytond_carrier_percentage-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-29 15:18:25.000000 trytond_carrier_percentage-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:48.701979 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2024-04-29 15:38:48.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1603 2024-04-29 15:38:48.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:48.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:38:48.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-29 15:38:48.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:48.000000 trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:48.701979 trytond_carrier_percentage-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_carrier_percentage-7.2.0/view/carrier_form.xml
```

### Comparing `trytond_carrier_percentage-7.0.0/CHANGELOG` & `trytond_carrier_percentage-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_carrier_percentage-7.0.0/COPYRIGHT` & `trytond_carrier_percentage-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2023 Cédric Krier.
+Copyright (C) 2011-2024 Cédric Krier.
 Copyright (C) 2011-2012 Bertrand Chenal.
 Copyright (C) 2011-2023 Nicolas Évrard.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_carrier_percentage-7.0.0/LICENSE` & `trytond_carrier_percentage-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/PKG-INFO` & `trytond_carrier_percentage-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_percentage
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add cost method "on percentage" on carrier
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
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2; extra == "test"
 
 Carrier Percentage Module
 #########################
 
 The carrier percentage module adds a cost method based on percentage.
```

### Comparing `trytond_carrier_percentage-7.0.0/__init__.py` & `trytond_carrier_percentage-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/carrier.py` & `trytond_carrier_percentage-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/doc/conf.py` & `trytond_carrier_percentage-7.2.0/doc/conf.py`

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

### Comparing `trytond_carrier_percentage-7.0.0/locale/lo.po` & `trytond_carrier_percentage-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/sale.py` & `trytond_carrier_percentage-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/setup.py` & `trytond_carrier_percentage-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/stock.py` & `trytond_carrier_percentage-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst` & `trytond_carrier_percentage-7.2.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =======================================================
 Carrier Percentage with Purchase Shipment Cost Scenario
 =======================================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'carrier_percentage',
     ...         'purchase_shipment_cost',
     ...         'sale_shipment_cost',
@@ -116,16 +116,15 @@
     >>> move.product = product
     >>> move.quantity = 50
     >>> move.unit_price = Decimal('8')
     >>> move.currency = company.currency
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('60.0000')
-    >>> shipment.cost_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_currency_used, company.currency)
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> move, = shipment.incoming_moves
     >>> move.unit_price
     Decimal('9.2000')
 
@@ -144,16 +143,15 @@
     >>> sale.invoice_method = 'shipment'
     >>> sale.shipment_cost_method = 'shipment'
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 5.0
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
     >>> cost_line.quantity
     1.0
     >>> cost_line.amount
     Decimal('15.00')
     >>> sale.click('confirm')
     >>> sale.click('process')
     >>> sale.state
@@ -161,42 +159,39 @@
     >>> sale.untaxed_amount
     Decimal('115.00')
 
 Send products::
 
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> shipment, = sale.shipments
-    >>> shipment.carrier == carrier
-    True
+    >>> assertEqual(shipment.carrier, carrier)
     >>> shipment.cost_used
     Decimal('15.0000')
     >>> shipment.cost_sale_used
     Decimal('15.0000')
-    >>> shipment.cost_sale_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_sale_currency_used, company.currency)
     >>> move, = shipment.inventory_moves
     >>> move.quantity = 4
     >>> shipment.cost_used
     Decimal('12.0000')
     >>> shipment.cost_sale_used
     Decimal('12.0000')
-    >>> shipment.cost_sale_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_sale_currency_used, company.currency)
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_force')
     >>> shipment.state
     'assigned'
     >>> shipment.click('pick')
     >>> shipment.state
     'picked'
     >>> shipment.click('pack')
     >>> shipment.state
     'packed'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
@@ -212,32 +207,30 @@
     >>> sale.invoice_method = 'order'
     >>> sale.shipment_cost_method = 'order'
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 3.0
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
-    >>> cost_line.quantity == 1
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
+    >>> cost_line.quantity
+    1.0
     >>> cost_line.amount
     Decimal('9.00')
     >>> sale.click('confirm')
     >>> sale.click('process')
     >>> sale.state
     'processing'
     >>> sale.untaxed_amount
     Decimal('69.00')
 
 Check customer shipment::
 
     >>> shipment, = sale.shipments
-    >>> shipment.carrier == carrier
-    True
+    >>> assertEqual(shipment.carrier, carrier)
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
     >>> invoice.untaxed_amount
     Decimal('69.00')
```

### Comparing `trytond_carrier_percentage-7.0.0/tests/test_module.py` & `trytond_carrier_percentage-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/tox.ini` & `trytond_carrier_percentage-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/PKG-INFO` & `trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-carrier-percentage
-Version: 7.0.0
+Name: trytond_carrier_percentage
+Version: 7.2.0
 Summary: Tryton module to add cost method "on percentage" on carrier
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
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2; extra == "test"
 
 Carrier Percentage Module
 #########################
 
 The carrier percentage module adds a cost method based on percentage.
```

### Comparing `trytond_carrier_percentage-7.0.0/trytond_carrier_percentage.egg-info/SOURCES.txt` & `trytond_carrier_percentage-7.2.0/trytond_carrier_percentage.egg-info/SOURCES.txt`

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
 carrier.py
```

