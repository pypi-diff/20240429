# Comparing `tmp/trytond_sale_promotion-7.0.1.tar.gz` & `tmp/trytond_sale_promotion-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_promotion-7.0.1.tar", last modified: Fri Nov 17 18:44:45 2023, max compression
+gzip compressed data, was "trytond_sale_promotion-7.2.0.tar", last modified: Mon Apr 29 15:49:11 2024, max compression
```

## Comparing `trytond_sale_promotion-7.0.1.tar` & `trytond_sale_promotion-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:44:45.741779 trytond_sale_promotion-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-11-17 18:44:43.000000 trytond_sale_promotion-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-11-17 18:44:42.000000 trytond_sale_promotion-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2023-11-17 18:44:45.738446 trytond_sale_promotion-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:44:45.738446 trytond_sale_promotion-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:44:45.738446 trytond_sale_promotion-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2970 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2916 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2525 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2929 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2953 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2680 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3168 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2960 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2486 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2928 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2831 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2627 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2868 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2779 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2798 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2396 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2527 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11801 2023-11-15 17:06:50.000000 trytond_sale_promotion-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3940 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-11-17 18:44:45.741779 trytond_sale_promotion-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4420 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:44:45.738446 trytond_sale_promotion-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4595 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/tests/scenario_sale_promotion.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2487 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/tests/scenario_sale_promotion_amount.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-10-30 17:55:12.000000 trytond_sale_promotion-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:44:45.738446 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2023-11-17 18:44:45.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1673 2023-11-17 18:44:45.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-11-17 18:44:45.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-11-17 18:44:45.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:09.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      228 2023-11-17 18:44:45.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-11-17 18:44:45.000000 trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:44:45.738446 trytond_sale_promotion-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/view/promotion_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-10-30 17:06:38.000000 trytond_sale_promotion-7.0.1/view/promotion_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1906 2024-04-29 15:26:13.000000 trytond_sale_promotion-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:26:12.000000 trytond_sale_promotion-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_promotion-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.439025 trytond_sale_promotion-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_promotion-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:28.000000 trytond_sale_promotion-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2970 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2916 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2525 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2953 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2643 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2680 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3168 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2960 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2486 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2928 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2831 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2627 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2868 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-04-29 13:17:17.000000 trytond_sale_promotion-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2779 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2798 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2396 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2527 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11801 2024-03-17 11:01:36.000000 trytond_sale_promotion-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3871 2024-04-27 16:30:39.000000 trytond_sale_promotion-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:11.445692 trytond_sale_promotion-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4420 2024-03-17 11:01:36.000000 trytond_sale_promotion-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4546 2024-04-22 12:14:36.000000 trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2473 2024-04-22 12:14:36.000000 trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion_amount.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:28.000000 trytond_sale_promotion-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-04-29 15:26:08.000000 trytond_sale_promotion-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1655 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/view/promotion_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/view/promotion_list.xml
```

### Comparing `trytond_sale_promotion-7.0.1/CHANGELOG` & `trytond_sale_promotion-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_sale_promotion-7.0.1/LICENSE` & `trytond_sale_promotion-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/PKG-INFO` & `trytond_sale_promotion-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_promotion
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for sale promotion
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
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Promotion
 ##############
 
 The sale_promotion module allows to apply promotions on sale based on criteria.
 
 The promotion is applied by changing the unit price of the affected lines when
```

### Comparing `trytond_sale_promotion-7.0.1/README.rst` & `trytond_sale_promotion-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/doc/conf.py` & `trytond_sale_promotion-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_promotion-7.0.1/doc/index.rst` & `trytond_sale_promotion-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/bg.po` & `trytond_sale_promotion-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/ca.po` & `trytond_sale_promotion-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/cs.po` & `trytond_sale_promotion-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/de.po` & `trytond_sale_promotion-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/es.po` & `trytond_sale_promotion-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/es_419.po` & `trytond_sale_promotion-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/et.po` & `trytond_sale_promotion-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/fa.po` & `trytond_sale_promotion-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/fi.po` & `trytond_sale_promotion-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/fr.po` & `trytond_sale_promotion-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/hu.po` & `trytond_sale_promotion-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/id.po` & `trytond_sale_promotion-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/it.po` & `trytond_sale_promotion-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/lo.po` & `trytond_sale_promotion-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/lt.po` & `trytond_sale_promotion-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/nl.po` & `trytond_sale_promotion-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/pl.po` & `trytond_sale_promotion-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/pt.po` & `trytond_sale_promotion-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/ro.po` & `trytond_sale_promotion-7.2.0/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 msgctxt "field:sale.promotion,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:sale.promotion,categories:"
 msgid "Categories"
-msgstr "Categorii"
+msgstr ""
 
 msgctxt "field:sale.promotion,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.promotion,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:sale.promotion,end_date:"
 msgid "End Date"
@@ -60,23 +60,23 @@
 
 msgctxt "field:sale.promotion,untaxed_amount:"
 msgid "Untaxed Amount"
 msgstr ""
 
 msgctxt "field:sale.promotion-product.category,category:"
 msgid "Category"
-msgstr "Categorie"
+msgstr ""
 
 msgctxt "field:sale.promotion-product.category,promotion:"
 msgid "Promotion"
 msgstr ""
 
 msgctxt "field:sale.promotion-product.product,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:sale.promotion-product.product,promotion:"
 msgid "Promotion"
 msgstr ""
 
 msgctxt "help:sale.promotion,formula:"
 msgid ""
```

### Comparing `trytond_sale_promotion-7.0.1/locale/ru.po` & `trytond_sale_promotion-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/sl.po` & `trytond_sale_promotion-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/tr.po` & `trytond_sale_promotion-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/locale/uk.po` & `trytond_sale_promotion-7.2.0/locale/zh_CN.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.line,draft_unit_price:"
 msgid "Draft Unit Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.line,promotion:"
 msgid "Promotion"
-msgstr ""
+msgstr "Promotions"
 
 msgctxt "field:sale.promotion,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:sale.promotion,categories:"
 msgid "Categories"
@@ -30,17 +31,18 @@
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:sale.promotion,formula:"
 msgid "Formula"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.promotion,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
 msgctxt "field:sale.promotion,price_list:"
 msgid "Price List"
 msgstr ""
 
 msgctxt "field:sale.promotion,products:"
 msgid "Products"
@@ -62,57 +64,60 @@
 msgid "Untaxed Amount"
 msgstr ""
 
 msgctxt "field:sale.promotion-product.category,category:"
 msgid "Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.promotion-product.category,promotion:"
 msgid "Promotion"
-msgstr ""
+msgstr "Promotions"
 
 msgctxt "field:sale.promotion-product.product,product:"
 msgid "Product"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.promotion-product.product,promotion:"
 msgid "Promotion"
-msgstr ""
+msgstr "Promotions"
 
 msgctxt "help:sale.promotion,formula:"
 msgid ""
 "Python expression that will be evaluated with:\n"
 "- unit_price: the original unit_price"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_promotion_form"
 msgid "Promotions"
-msgstr ""
+msgstr "Promotions"
 
 msgctxt "model:ir.action,name:act_promotion_relate"
 msgid "Sale Promotions"
-msgstr ""
+msgstr "Sale Promotions"
 
 msgctxt "model:ir.message,text:msg_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in promotion \"%(promotion)s\" 'with "
 "exception \"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_promotion_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_promotion"
 msgid "Promotions"
-msgstr ""
+msgstr "Promotions"
 
+#, fuzzy
 msgctxt "model:sale.promotion,name:"
 msgid "Sale Promotion"
-msgstr ""
+msgstr "Sale Promotions"
 
 msgctxt "model:sale.promotion-product.category,name:"
 msgid "Sale Promotion - Product Category"
 msgstr ""
 
 msgctxt "model:sale.promotion-product.product,name:"
 msgid "Sale Promotion - Product"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_promotion-7.0.1/locale/zh_CN.po` & `trytond_sale_promotion-7.2.0/locale/ro.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,125 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:sale.line,draft_unit_price:"
 msgid "Draft Unit Price"
-msgstr ""
+msgstr "Ciornă Preț unitar"
 
-#, fuzzy
 msgctxt "field:sale.line,promotion:"
 msgid "Promotion"
-msgstr "Promotions"
+msgstr "Promoție"
 
 msgctxt "field:sale.promotion,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:sale.promotion,categories:"
 msgid "Categories"
-msgstr ""
+msgstr "Categorii"
 
 msgctxt "field:sale.promotion,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:sale.promotion,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:sale.promotion,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data de sfârşit"
 
 msgctxt "field:sale.promotion,formula:"
 msgid "Formula"
-msgstr ""
+msgstr "Formulă"
 
-#, fuzzy
 msgctxt "field:sale.promotion,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nume"
 
 msgctxt "field:sale.promotion,price_list:"
 msgid "Price List"
-msgstr ""
+msgstr "Listă de prețuri"
 
 msgctxt "field:sale.promotion,products:"
 msgid "Products"
-msgstr ""
+msgstr "Produse"
 
 msgctxt "field:sale.promotion,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:sale.promotion,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data de Început"
 
 msgctxt "field:sale.promotion,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:sale.promotion,untaxed_amount:"
 msgid "Untaxed Amount"
-msgstr ""
+msgstr "Sumă neimpozată"
 
 msgctxt "field:sale.promotion-product.category,category:"
 msgid "Category"
-msgstr ""
+msgstr "Categorie"
 
-#, fuzzy
 msgctxt "field:sale.promotion-product.category,promotion:"
 msgid "Promotion"
-msgstr "Promotions"
+msgstr "Promoție"
 
 msgctxt "field:sale.promotion-product.product,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
-#, fuzzy
 msgctxt "field:sale.promotion-product.product,promotion:"
 msgid "Promotion"
-msgstr "Promotions"
+msgstr "Promoție"
 
+#, fuzzy
 msgctxt "help:sale.promotion,formula:"
 msgid ""
 "Python expression that will be evaluated with:\n"
 "- unit_price: the original unit_price"
 msgstr ""
+"Expresie Python care va fi evaluată cu:\n"
+"- unit_price: unit_price inițial"
 
 msgctxt "model:ir.action,name:act_promotion_form"
 msgid "Promotions"
-msgstr "Promotions"
+msgstr "Promoții"
 
 msgctxt "model:ir.action,name:act_promotion_relate"
 msgid "Sale Promotions"
-msgstr "Sale Promotions"
+msgstr "Promoții de vânzare"
 
 msgctxt "model:ir.message,text:msg_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in promotion \"%(promotion)s\" 'with "
 "exception \"%(exception)s\"."
 msgstr ""
+"Formula \"%(formula)s\" invalidă în promoția \"%(promotion)s\" cu excepția "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.rule.group,name:rule_group_promotion_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.ui.menu,name:menu_promotion"
 msgid "Promotions"
-msgstr "Promotions"
+msgstr "Promoții"
 
-#, fuzzy
 msgctxt "model:sale.promotion,name:"
 msgid "Sale Promotion"
-msgstr "Sale Promotions"
+msgstr "Promoție de vânzare"
 
 msgctxt "model:sale.promotion-product.category,name:"
 msgid "Sale Promotion - Product Category"
-msgstr ""
+msgstr "Promoție de vânzare - Categorie de produse"
 
 msgctxt "model:sale.promotion-product.product,name:"
 msgid "Sale Promotion - Product"
-msgstr ""
+msgstr "Promoție de vânzare - Produs"
```

### Comparing `trytond_sale_promotion-7.0.1/sale.py` & `trytond_sale_promotion-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/sale.xml` & `trytond_sale_promotion-7.2.0/sale.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_sale_promotion-7.0.1/sale.xml` & `trytond_sale_promotion-7.2.0/sale.xml`

```diff
@@ -38,30 +38,30 @@
     <record model="ir.action.keyword" id="act_promotion_relate_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">product.price_list,-1</field>
       <field name="action" ref="act_promotion_relate"/>
     </record>
     <record model="ir.rule.group" id="rule_group_promotion_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.promotion')]"/>
+      <field name="model">sale.promotion</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_promotion_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_promotion_companies"/>
     </record>
     <record model="ir.model.access" id="access_promotion">
-      <field name="model" search="[('model', '=', 'sale.promotion')]"/>
+      <field name="model">sale.promotion</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_promotion_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.promotion')]"/>
+      <field name="model">sale.promotion</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_sale_promotion-7.0.1/setup.py` & `trytond_sale_promotion-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/tests/scenario_sale_promotion.rst` & `trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 Sale Promotion Scenario
 =======================
 
 Imports::
 
     >>> import datetime
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_promotion')
 
 Create company::
```

### Comparing `trytond_sale_promotion-7.0.1/tests/scenario_sale_promotion_amount.rst` & `trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion_amount.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ==============================
 Sale Promotion Amount Scenario
 ==============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate modules::
 
     >>> config = activate_modules('sale_promotion')
 
 Create company::
```

### Comparing `trytond_sale_promotion-7.0.1/tox.ini` & `trytond_sale_promotion-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/PKG-INFO` & `trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-promotion
-Version: 7.0.1
+Name: trytond_sale_promotion
+Version: 7.2.0
 Summary: Tryton module for sale promotion
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
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Promotion
 ##############
 
 The sale_promotion module allows to apply promotions on sale based on criteria.
 
 The promotion is applied by changing the unit price of the affected lines when
```

### Comparing `trytond_sale_promotion-7.0.1/trytond_sale_promotion.egg-info/SOURCES.txt` & `trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/SOURCES.txt`

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

### Comparing `trytond_sale_promotion-7.0.1/view/promotion_form.xml` & `trytond_sale_promotion-7.2.0/view/promotion_form.xml`

 * *Files identical despite different names*

