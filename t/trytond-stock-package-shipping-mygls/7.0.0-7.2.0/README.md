# Comparing `tmp/trytond_stock_package_shipping_mygls-7.0.0.tar.gz` & `tmp/trytond_stock_package_shipping_mygls-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_mygls-7.0.0.tar", last modified: Mon Oct 30 17:42:48 2023, max compression
+gzip compressed data, was "trytond_stock_package_shipping_mygls-7.2.0.tar", last modified: Mon Apr 29 15:52:06 2024, max compression
```

## Comparing `trytond_stock_package_shipping_mygls-7.0.0.tar` & `trytond_stock_package_shipping_mygls-7.2.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:48.709145 trytond_stock_package_shipping_mygls-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-10-22 17:23:25.000000 trytond_stock_package_shipping_mygls-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-10-30 17:14:54.000000 trytond_stock_package_shipping_mygls-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:14:54.000000 trytond_stock_package_shipping_mygls-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3048 2023-10-30 17:42:48.709145 trytond_stock_package_shipping_mygls-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/api.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4021 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2734 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:48.705812 trytond_stock_package_shipping_mygls-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2829 2023-10-22 17:23:25.000000 trytond_stock_package_shipping_mygls-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:25.000000 trytond_stock_package_shipping_mygls-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:48.702479 trytond_stock_package_shipping_mygls-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6819 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6950 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6900 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6988 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5164 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5273 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6778 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6826 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_mygls-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2010 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_mygls-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:42:48.709145 trytond_stock_package_shipping_mygls-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4862 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_mygls-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_mygls-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:48.702479 trytond_stock_package_shipping_mygls-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6618 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_mygls-7.0.0/tests/scenario_stock_package_shipping_mygls.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_mygls-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-10-30 17:14:49.000000 trytond_stock_package_shipping_mygls-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:48.705812 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3048 2023-10-30 17:42:48.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-10-30 17:42:48.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:42:48.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2023-10-30 17:42:48.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-30 17:42:48.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:42:48.000000 trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:48.705812 trytond_stock_package_shipping_mygls-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/view/credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.0.0/view/credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      765 2024-04-29 15:28:25.000000 trytond_stock_package_shipping_mygls-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:28:25.000000 trytond_stock_package_shipping_mygls-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/api.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4021 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_mygls-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2688 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_mygls-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.491114 trytond_stock_package_shipping_mygls-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3091 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_mygls-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.491114 trytond_stock_package_shipping_mygls-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6819 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6950 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6900 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6988 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5164 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5264 2024-04-29 13:17:17.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6778 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6817 2024-04-29 13:17:17.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2010 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_mygls-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4853 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_mygls-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_mygls-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.491114 trytond_stock_package_shipping_mygls-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6596 2024-04-22 12:14:36.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/scenario_stock_package_shipping_mygls.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_mygls-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-29 15:28:21.000000 trytond_stock_package_shipping_mygls-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1849 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/view/credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/view/credential_list.xml
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/CHANGELOG` & `trytond_stock_package_shipping_mygls-7.2.0/CHANGELOG`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/COPYRIGHT` & `trytond_stock_package_shipping_mygls-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2023 B2CK
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 B2CK
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/LICENSE` & `trytond_stock_package_shipping_mygls-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/PKG-INFO` & `trytond_stock_package_shipping_mygls-7.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_mygls
-Version: 7.0.0
+Version: 7.2.0
 Summary: MyGLS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-mygls
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-package-shipping-mygls
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping gls mygls
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: zeep
 Requires-Dist: pypdf>=3
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_package_shipping<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
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
 
 ###################################
 Stock Package Shipping MyGLS Module
 ###################################
 
 The *Stock Package Shipping MyGLS Module* allows package labels to be generated
 for shipments using `MyGLS <https://api.mygls.hu/>`_ webservices.
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/__init__.py` & `trytond_stock_package_shipping_mygls-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/api.py` & `trytond_stock_package_shipping_mygls-7.2.0/api.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/carrier.py` & `trytond_stock_package_shipping_mygls-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/carrier.xml` & `trytond_stock_package_shipping_mygls-7.2.0/carrier.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_stock_package_shipping_mygls-7.0.0/carrier.xml` & `trytond_stock_package_shipping_mygls-7.2.0/carrier.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_credential_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="credential_view_form"/>
       <field name="act_window" ref="act_credential_form"/>
     </record>
     <menuitem parent="carrier.menu_configuration" action="act_credential_form" sequence="50" id="menu_credential_form"/>
     <record model="ir.model.access" id="access_carrier_credential">
-      <field name="model" search="[('model', '=', 'carrier.credential.mygls')]"/>
+      <field name="model">carrier.credential.mygls</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_credential_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.credential.mygls')]"/>
+      <field name="model">carrier.credential.mygls</field>
       <field name="group" ref="carrier.group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="carrier_view_form">
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/doc/conf.py` & `trytond_stock_package_shipping_mygls-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/doc/design.rst` & `trytond_stock_package_shipping_mygls-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/bg.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/ca.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/cs.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/de.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/es.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/es_419.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/et.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/fa.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/fi.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/fr.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/hu.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/id.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/it.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
 msgctxt "model:ir.message,text:msg_phone_mobile_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add a phone or mobile number "
 "for address \"%(address)s\"."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_shipment_has_shipping_reference_number"
 msgid ""
 "You cannot create a shipping label for shipment \"%(shipment)s\" because it "
 "already has a shipping reference number."
 msgstr ""
 "Non puoi creare un'etichetta di spedizione per la spedizione "
 "\"%(shipment)s\" perché ha già un numero di riferimento."
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/lo.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/lt.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/nl.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/pl.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/pt.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/ro.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add a phone or mobile number "
 "for address \"%(address)s\"."
 msgstr ""
 "Pentru a valida expedierea \"%(shipment)s\" trebuie adăugat un număr de "
 "telefon sau mobil pentru adresa \"%(address)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_shipment_has_shipping_reference_number"
 msgid ""
 "You cannot create a shipping label for shipment \"%(shipment)s\" because it "
 "already has a shipping reference number."
 msgstr ""
 "Nu se poate crea o eticheta pentru expedierea \"%(shipment)s\" pentru că are"
 " deja un număr de referinţa."
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/ru.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/sl.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/tr.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/uk.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/locale/zh_CN.po` & `trytond_stock_package_shipping_mygls-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/message.xml` & `trytond_stock_package_shipping_mygls-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/setup.py` & `trytond_stock_package_shipping_mygls-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-stock-package-shipping-mygls'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping gls mygls',
     package_dir={'trytond.modules.stock_package_shipping_mygls': '.'},
     packages=(
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/stock.py` & `trytond_stock_package_shipping_mygls-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/tests/scenario_stock_package_shipping_mygls.rst` & `trytond_stock_package_shipping_mygls-7.2.0/tests/scenario_stock_package_shipping_mygls.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 Imports::
 
     >>> import os
     >>> import uuid
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
 
     >>> config = activate_modules(
     ...     ['stock_package_shipping_mygls', 'sale', 'sale_shipment_cost'])
 
     >>> Address = Model.get('party.address')
@@ -49,15 +48,15 @@
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
 Create countries::
 
-    >>> hungary= Country(code='HU', name="Hungary")
+    >>> hungary = Country(code='HU', name="Hungary")
     >>> hungary.save()
 
 Create parties::
 
     >>> customer = Party(name='Customer')
     >>> customer.save()
     >>> customer_address = customer.addresses.new()
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/tox.ini` & `trytond_stock_package_shipping_mygls-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO` & `trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-stock-package-shipping-mygls
-Version: 7.0.0
+Name: trytond_stock_package_shipping_mygls
+Version: 7.2.0
 Summary: MyGLS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-mygls
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-package-shipping-mygls
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping gls mygls
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: zeep
 Requires-Dist: pypdf>=3
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_package_shipping<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
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
 
 ###################################
 Stock Package Shipping MyGLS Module
 ###################################
 
 The *Stock Package Shipping MyGLS Module* allows package labels to be generated
 for shipments using `MyGLS <https://api.mygls.hu/>`_ webservices.
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt`

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
 api.py
```

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/view/carrier_form.xml` & `trytond_stock_package_shipping_mygls-7.2.0/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.0.0/view/credential_form.xml` & `trytond_stock_package_shipping_mygls-7.2.0/view/credential_form.xml`

 * *Files identical despite different names*

