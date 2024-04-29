# Comparing `tmp/trytond_stock_package_shipping_ups-7.0.2.tar.gz` & `tmp/trytond_stock_package_shipping_ups-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_ups-7.0.2.tar", last modified: Wed Apr 17 10:32:51 2024, max compression
+gzip compressed data, was "trytond_stock_package_shipping_ups-7.2.0.tar", last modified: Mon Apr 29 15:52:19 2024, max compression
```

## Comparing `trytond_stock_package_shipping_ups-7.0.2.tar` & `trytond_stock_package_shipping_ups-7.2.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-04-17 10:32:49.000000 trytond_stock_package_shipping_ups-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-17 10:32:48.000000 trytond_stock_package_shipping_ups-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      610 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.841093 trytond_stock_package_shipping_ups-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2805 2024-03-03 16:24:20.000000 trytond_stock_package_shipping_ups-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3397 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4132 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4247 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4176 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3349 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4293 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4279 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3335 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3243 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3330 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3310 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4165 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3374 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3435 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3377 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3544 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3298 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1284 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4786 2024-03-03 16:24:03.000000 trytond_stock_package_shipping_ups-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15604 2024-04-12 20:13:29.000000 trytond_stock_package_shipping_ups-7.0.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7906 2024-02-05 16:24:27.000000 trytond_stock_package_shipping_ups-7.0.2/tests/scenario_shipping_ups.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-02-29 11:49:06.000000 trytond_stock_package_shipping_ups-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-03-03 12:15:34.000000 trytond_stock_package_shipping_ups-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1895 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:16.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:32:51.000000 trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:32:51.844426 trytond_stock_package_shipping_ups-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/package_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/ups_credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_ups-7.0.2/view/ups_credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:19.294112 trytond_stock_package_shipping_ups-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1934 2024-04-29 15:28:35.000000 trytond_stock_package_shipping_ups-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-29 15:28:35.000000 trytond_stock_package_shipping_ups-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-29 15:52:19.294112 trytond_stock_package_shipping_ups-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      610 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_ups-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_ups-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:19.290779 trytond_stock_package_shipping_ups-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_ups-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1316 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       57 2024-04-22 12:14:36.000000 trytond_stock_package_shipping_ups-7.2.0/doc/linkcheck_ignore.json
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:35.000000 trytond_stock_package_shipping_ups-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_ups-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:19.290779 trytond_stock_package_shipping_ups-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3397 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4132 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4247 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4176 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3212 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3349 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4293 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4279 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3335 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3243 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3330 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3310 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4165 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3374 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3590 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3435 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3377 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3544 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3212 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3298 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_ups-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1284 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_ups-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:19.294112 trytond_stock_package_shipping_ups-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4786 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_ups-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15604 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_ups-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:19.290779 trytond_stock_package_shipping_ups-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7828 2024-04-22 12:14:36.000000 trytond_stock_package_shipping_ups-7.2.0/tests/scenario_shipping_ups.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_ups-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:35.000000 trytond_stock_package_shipping_ups-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-04-29 15:28:31.000000 trytond_stock_package_shipping_ups-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:19.294112 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-29 15:52:18.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1921 2024-04-29 15:52:19.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:18.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:52:18.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-29 15:52:18.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:18.000000 trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:19.294112 trytond_stock_package_shipping_ups-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-7.2.0/view/package_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/view/ups_credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_ups-7.2.0/view/ups_credential_list.xml
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/CHANGELOG` & `trytond_stock_package_shipping_ups-7.2.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-04-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-03-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/COPYRIGHT` & `trytond_stock_package_shipping_ups-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/LICENSE` & `trytond_stock_package_shipping_ups-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/PKG-INFO` & `trytond_stock_package_shipping_ups-7.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_ups
-Version: 7.0.2
+Version: 7.2.0
 Summary: UPS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-stock-package-shipping-ups
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -49,26 +49,26 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: requests-oauthlib
 Requires-Dist: oauthlib
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_package_shipping<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock_package<7.3,>=7.2
+Requires-Dist: trytond_stock_package_shipping<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 ##########################
 Stock Package Shipping UPS
 ##########################
 
 The *Stock Package Shipping UPS Module* allows to generate `UPS
 <https://www.ups.com/>`_ labels per package using their APIs.
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/__init__.py` & `trytond_stock_package_shipping_ups-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/carrier.py` & `trytond_stock_package_shipping_ups-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/carrier.xml` & `trytond_stock_package_shipping_ups-7.2.0/carrier.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_stock_package_shipping_ups-7.0.2/carrier.xml` & `trytond_stock_package_shipping_ups-7.2.0/carrier.xml`

```diff
@@ -30,22 +30,22 @@
     <record model="ir.action.act_window.view" id="act_ups_credential_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="credential_view_form"/>
       <field name="act_window" ref="act_ups_credential_form"/>
     </record>
     <menuitem parent="carrier.menu_configuration" action="act_ups_credential_form" sequence="20" id="menu_ups_credential_form"/>
     <record model="ir.model.access" id="access_carrier_credential">
-      <field name="model" search="[('model', '=', 'carrier.credential.ups')]"/>
+      <field name="model">carrier.credential.ups</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_credential_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.credential.ups')]"/>
+      <field name="model">carrier.credential.ups</field>
       <field name="group" ref="carrier.group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/doc/conf.py` & `trytond_stock_package_shipping_ups-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
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

### Comparing `trytond_stock_package_shipping_ups-7.0.2/doc/design.rst` & `trytond_stock_package_shipping_ups-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/doc/usage.rst` & `trytond_stock_package_shipping_ups-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/bg.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/ca.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/cs.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/de.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/es.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/es_419.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/et.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/fa.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/fi.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/fr.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/hu.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/id.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/it.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/lo.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/lt.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/nl.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/pl.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/pt.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/ro.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/ru.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/sl.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/tr.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/uk.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/locale/zh_CN.po` & `trytond_stock_package_shipping_ups-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/message.xml` & `trytond_stock_package_shipping_ups-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/setup.py` & `trytond_stock_package_shipping_ups-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/stock.py` & `trytond_stock_package_shipping_ups-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/stock.xml` & `trytond_stock_package_shipping_ups-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/tests/scenario_shipping_ups.rst` & `trytond_stock_package_shipping_ups-7.2.0/tests/scenario_shipping_ups.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 Stock Package Shipping with UPS scenario
 ========================================
 
 Imports::
 
     >>> import os
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
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
 
     >>> config = activate_modules(
     ...     ['stock_package_shipping_ups', 'sale', 'sale_shipment_cost'])
 
 Create company::
@@ -223,17 +222,16 @@
     >>> pack, = shipment.root_packages
     >>> pack.shipping_label is not None
     True
     >>> pack.shipping_label_mimetype
     'image/gif'
     >>> pack.shipping_reference is not None
     True
-    >>> pack.shipping_tracking_url.startswith('https://www.ups.com/track?')
-    True
+    >>> pack.shipping_tracking_url
+    'https://www.ups.com/track?...'
     >>> pack.shipping_reference in pack.shipping_tracking_url
     True
 
 Because there is only one box, the pack shipping number is also the shipment
 identification number::
 
-    >>> pack.shipping_reference == shipment.shipping_reference
-    True
+    >>> assertEqual(pack.shipping_reference, shipment.shipping_reference)
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/tox.ini` & `trytond_stock_package_shipping_ups-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/PKG-INFO` & `trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_ups
-Version: 7.0.2
+Version: 7.2.0
 Summary: UPS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-stock-package-shipping-ups
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -49,26 +49,26 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: requests-oauthlib
 Requires-Dist: oauthlib
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_package_shipping<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock_package<7.3,>=7.2
+Requires-Dist: trytond_stock_package_shipping<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 ##########################
 Stock Package Shipping UPS
 ##########################
 
 The *Stock Package Shipping UPS Module* allows to generate `UPS
 <https://www.ups.com/>`_ labels per package using their APIs.
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_ups-7.2.0/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ./view/package_type_form.xml
 ./view/ups_credential_form.xml
 ./view/ups_credential_list.xml
 doc/conf.py
 doc/configuration.rst
 doc/design.rst
 doc/index.rst
+doc/linkcheck_ignore.json
 doc/releases.rst
 doc/requirements-doc.txt
 doc/usage.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

### Comparing `trytond_stock_package_shipping_ups-7.0.2/view/carrier_form.xml` & `trytond_stock_package_shipping_ups-7.2.0/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-7.0.2/view/ups_credential_form.xml` & `trytond_stock_package_shipping_ups-7.2.0/view/ups_credential_form.xml`

 * *Files identical despite different names*

