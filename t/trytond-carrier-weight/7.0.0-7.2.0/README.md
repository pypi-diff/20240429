# Comparing `tmp/trytond_carrier_weight-7.0.0.tar.gz` & `tmp/trytond_carrier_weight-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_weight-7.0.0.tar", last modified: Mon Oct 30 17:28:23 2023, max compression
+gzip compressed data, was "trytond_carrier_weight-7.2.0.tar", last modified: Mon Apr 29 15:39:00 2024, max compression
```

## Comparing `trytond_carrier_weight-7.0.0.tar` & `trytond_carrier_weight-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:23.115017 trytond_carrier_weight-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:01.000000 trytond_carrier_weight-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2177 2023-10-30 17:05:29.000000 trytond_carrier_weight-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:05:29.000000 trytond_carrier_weight-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3034 2023-10-30 17:28:23.115017 trytond_carrier_weight-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-08-13 15:26:13.000000 trytond_carrier_weight-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4519 2023-10-24 07:56:52.000000 trytond_carrier_weight-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.0.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2023-10-07 17:14:58.000000 trytond_carrier_weight-7.0.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:23.111684 trytond_carrier_weight-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:01.000000 trytond_carrier_weight-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-08-13 15:26:13.000000 trytond_carrier_weight-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:01.000000 trytond_carrier_weight-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:23.108350 trytond_carrier_weight-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2157 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2257 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2174 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1731 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2225 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2201 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2085 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1706 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2061 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1842 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2181 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1739 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1819 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1715 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1778 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2023-10-30 16:47:45.000000 trytond_carrier_weight-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:28:23.115017 trytond_carrier_weight-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4590 2023-10-27 17:38:49.000000 trytond_carrier_weight-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-08-20 10:47:27.000000 trytond_carrier_weight-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:23.108350 trytond_carrier_weight-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7471 2023-10-24 07:56:52.000000 trytond_carrier_weight-7.0.0/tests/scenario_carrier_weight.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3683 2023-08-13 15:26:13.000000 trytond_carrier_weight-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_carrier_weight-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-10-30 17:05:25.000000 trytond_carrier_weight-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:23.111684 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3034 2023-10-30 17:28:22.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1683 2023-10-30 17:28:23.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:28:22.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:28:22.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:28:22.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:28:22.000000 trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:23.108350 trytond_carrier_weight-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.0.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.0.0/view/weight_price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.0.0/view/weight_price_list_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2278 2024-04-29 15:18:40.000000 trytond_carrier_weight-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:18:40.000000 trytond_carrier_weight-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3034 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2024-01-27 09:58:52.000000 trytond_carrier_weight-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4519 2024-02-04 18:51:26.000000 trytond_carrier_weight-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-02-04 18:51:26.000000 trytond_carrier_weight-7.2.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.441672 trytond_carrier_weight-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_carrier_weight-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2024-01-27 09:58:52.000000 trytond_carrier_weight-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:06.000000 trytond_carrier_weight-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2157 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2257 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2174 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1731 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2225 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2201 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2085 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1706 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2061 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1842 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2181 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1739 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1819 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2024-04-29 13:17:17.000000 trytond_carrier_weight-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4590 2024-03-17 11:01:36.000000 trytond_carrier_weight-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-08-20 10:47:27.000000 trytond_carrier_weight-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7465 2024-04-27 16:30:39.000000 trytond_carrier_weight-7.2.0/tests/scenario_carrier_weight.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3683 2024-01-27 09:58:52.000000 trytond_carrier_weight-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:06.000000 trytond_carrier_weight-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-04-29 15:18:36.000000 trytond_carrier_weight-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3034 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1665 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/view/weight_price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/view/weight_price_list_tree.xml
```

### Comparing `trytond_carrier_weight-7.0.0/CHANGELOG` & `trytond_carrier_weight-7.2.0/CHANGELOG`

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

### Comparing `trytond_carrier_weight-7.0.0/COPYRIGHT` & `trytond_carrier_weight-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2023 Cédric Krier.
+Copyright (C) 2011-2024 Cédric Krier.
 Copyright (C) 2011-2013 Bertrand Chenal.
 Copyright (C) 2011-2023 Nicolas Évrard.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_carrier_weight-7.0.0/LICENSE` & `trytond_carrier_weight-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/PKG-INFO` & `trytond_carrier_weight-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_weight
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add cost method "on weight" on carrier
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
@@ -48,25 +48,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_measurements<7.3,>=7.2
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
 
 Carrier Weight Module
 #####################
 
 The carrier weight module adds a cost method based on weight.
 The price is computed by finding the first line for which the weight is
 greater.
```

### Comparing `trytond_carrier_weight-7.0.0/__init__.py` & `trytond_carrier_weight-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/carrier.py` & `trytond_carrier_weight-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/carrier.xml` & `trytond_carrier_weight-7.2.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/common.py` & `trytond_carrier_weight-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/doc/conf.py` & `trytond_carrier_weight-7.2.0/doc/conf.py`

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

### Comparing `trytond_carrier_weight-7.0.0/locale/bg.po` & `trytond_carrier_weight-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/ca.po` & `trytond_carrier_weight-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/cs.po` & `trytond_carrier_weight-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/de.po` & `trytond_carrier_weight-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/es.po` & `trytond_carrier_weight-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/es_419.po` & `trytond_carrier_weight-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/et.po` & `trytond_carrier_weight-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/fa.po` & `trytond_carrier_weight-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/fi.po` & `trytond_carrier_weight-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/fr.po` & `trytond_carrier_weight-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/hu.po` & `trytond_carrier_weight-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/id.po` & `trytond_carrier_weight-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/it.po` & `trytond_carrier_weight-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/lo.po` & `trytond_carrier_weight-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/lt.po` & `trytond_carrier_weight-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/nl.po` & `trytond_carrier_weight-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/pl.po` & `trytond_carrier_weight-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/pt.po` & `trytond_carrier_weight-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/ro.po` & `trytond_carrier_weight-7.2.0/locale/tr.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Listă de prețuri"
+msgstr ""
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight UoM"
 msgstr ""
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
 msgstr ""
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_carrier_weight-7.0.0/locale/ru.po` & `trytond_carrier_weight-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/sl.po` & `trytond_carrier_weight-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/tr.po` & `trytond_carrier_weight-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/locale/uk.po` & `trytond_carrier_weight-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/sale.py` & `trytond_carrier_weight-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/setup.py` & `trytond_carrier_weight-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/stock.py` & `trytond_carrier_weight-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/tests/scenario_carrier_weight.rst` & `trytond_carrier_weight-7.2.0/tests/scenario_carrier_weight.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =======================
 Carrier Weight Scenario
 =======================
 
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
     ...         'carrier_weight',
     ...         'purchase_shipment_cost',
     ...         'sale_shipment_cost',
@@ -127,16 +127,15 @@
     >>> move.product = product
     >>> move.quantity = 4
     >>> move.unit_price = Decimal('8')
     >>> move.currency = company.currency
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('25.0000')
-    >>> shipment.cost_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_currency_used, company.currency)
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> move, = shipment.incoming_moves
     >>> move.unit_price
     Decimal('14.2500')
 
@@ -161,59 +160,55 @@
     >>> sale_line.product = product
     >>> sale_line.quantity = 2.0
     >>> sale_line = sale.lines.new()
     >>> sale_line.type = 'comment'
     >>> sale_line.description = 'Comment'
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
     Decimal('40.00')
     >>> sale.click('confirm')
     >>> sale.click('process')
     >>> sale.state
     'processing'
     >>> sale.untaxed_amount
     Decimal('140.00')
 
 Send products::
 
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> shipment, = sale.shipments
-    >>> shipment.carrier == carrier
-    True
+    >>> assertEqual(shipment.carrier, carrier)
     >>> shipment.cost_used
     Decimal('40.0000')
     >>> shipment.cost_sale_used
     Decimal('40.0000')
-    >>> shipment.cost_sale_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_sale_currency_used, company.currency)
     >>> move = shipment.inventory_moves[0]
     >>> move.quantity -= 1
     >>> shipment.cost_used
     Decimal('25.0000')
     >>> shipment.cost_sale_used
     Decimal('25.0000')
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
@@ -229,32 +224,30 @@
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
     Decimal('25.00')
     >>> sale.click('confirm')
     >>> sale.click('process')
     >>> sale.state
     'processing'
     >>> sale.untaxed_amount
     Decimal('85.00')
 
 Check customer shipment::
 
     >>> shipment, = sale.shipments
-    >>> shipment.carrier == carrier
-    True
+    >>> assertEqual(shipment.carrier, carrier)
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
     >>> invoice.untaxed_amount
     Decimal('85.00')
```

### Comparing `trytond_carrier_weight-7.0.0/tests/test_module.py` & `trytond_carrier_weight-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/tox.ini` & `trytond_carrier_weight-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/PKG-INFO` & `trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-carrier-weight
-Version: 7.0.0
+Name: trytond_carrier_weight
+Version: 7.2.0
 Summary: Tryton module to add cost method "on weight" on carrier
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
@@ -48,25 +48,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_measurements<7.3,>=7.2
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
 
 Carrier Weight Module
 #####################
 
 The carrier weight module adds a cost method based on weight.
 The price is computed by finding the first line for which the weight is
 greater.
```

### Comparing `trytond_carrier_weight-7.0.0/trytond_carrier_weight.egg-info/SOURCES.txt` & `trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/SOURCES.txt`

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

