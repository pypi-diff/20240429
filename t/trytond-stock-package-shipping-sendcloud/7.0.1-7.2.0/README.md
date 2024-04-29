# Comparing `tmp/trytond_stock_package_shipping_sendcloud-7.0.1.tar.gz` & `tmp/trytond_stock_package_shipping_sendcloud-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_sendcloud-7.0.1.tar", last modified: Sat Dec 16 10:02:49 2023, max compression
+gzip compressed data, was "trytond_stock_package_shipping_sendcloud-7.2.0.tar", last modified: Mon Apr 29 15:52:12 2024, max compression
```

## Comparing `trytond_stock_package_shipping_sendcloud-7.0.1.tar` & `trytond_stock_package_shipping_sendcloud-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:02:49.172468 trytond_stock_package_shipping_sendcloud-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      765 2023-12-16 10:02:46.000000 trytond_stock_package_shipping_sendcloud-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-12-16 10:02:46.000000 trytond_stock_package_shipping_sendcloud-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3265 2023-12-16 10:02:49.172468 trytond_stock_package_shipping_sendcloud-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      792 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9652 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5549 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:02:49.165802 trytond_stock_package_shipping_sendcloud-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2833 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      998 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:02:49.169135 trytond_stock_package_shipping_sendcloud-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3547 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3527 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3567 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3584 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3570 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3468 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2975 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-12-16 10:02:49.172468 trytond_stock_package_shipping_sendcloud-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4901 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6844 2023-12-10 12:43:59.000000 trytond_stock_package_shipping_sendcloud-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:02:49.169135 trytond_stock_package_shipping_sendcloud-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7870 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/tests/scenario_stock_package_shipping_sendcloud.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-30 17:55:12.000000 trytond_stock_package_shipping_sendcloud-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:02:49.169135 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3265 2023-12-16 10:02:48.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2189 2023-12-16 10:02:49.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-12-16 10:02:48.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-12-16 10:02:48.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:16.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-12-16 10:02:48.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-12-16 10:02:48.000000 trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:02:49.169135 trytond_stock_package_shipping_sendcloud-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/carrier_address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/carrier_address_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/carrier_shipping_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/carrier_shipping_method_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:38.000000 trytond_stock_package_shipping_sendcloud-7.0.1/view/credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:12.700951 trytond_stock_package_shipping_sendcloud-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      765 2024-04-29 15:28:30.000000 trytond_stock_package_shipping_sendcloud-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:28:30.000000 trytond_stock_package_shipping_sendcloud-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3256 2024-04-29 15:52:12.700951 trytond_stock_package_shipping_sendcloud-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      792 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9652 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_sendcloud-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5411 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_sendcloud-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:12.697618 trytond_stock_package_shipping_sendcloud-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_sendcloud-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_sendcloud-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_sendcloud-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:12.697618 trytond_stock_package_shipping_sendcloud-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3547 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3527 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3567 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3584 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3561 2024-04-29 13:17:17.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3468 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2966 2024-04-29 13:17:17.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_sendcloud-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_sendcloud-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:12.700951 trytond_stock_package_shipping_sendcloud-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_sendcloud-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6844 2024-04-13 17:12:23.000000 trytond_stock_package_shipping_sendcloud-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:12.697618 trytond_stock_package_shipping_sendcloud-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7846 2024-04-22 12:14:37.000000 trytond_stock_package_shipping_sendcloud-7.2.0/tests/scenario_stock_package_shipping_sendcloud.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_sendcloud-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      223 2024-04-29 15:28:26.000000 trytond_stock_package_shipping_sendcloud-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:12.700951 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3256 2024-04-29 15:52:12.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2171 2024-04-29 15:52:12.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:12.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-29 15:52:12.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-29 15:52:12.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:12.000000 trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:12.700951 trytond_stock_package_shipping_sendcloud-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/carrier_address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/carrier_address_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/carrier_shipping_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/carrier_shipping_method_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-7.2.0/view/credential_list.xml
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/CHANGELOG` & `trytond_stock_package_shipping_sendcloud-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2023-12-16
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/COPYRIGHT` & `trytond_stock_package_shipping_sendcloud-7.2.0/COPYRIGHT`

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

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/LICENSE` & `trytond_stock_package_shipping_sendcloud-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/__init__.py` & `trytond_stock_package_shipping_sendcloud-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/carrier.py` & `trytond_stock_package_shipping_sendcloud-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/carrier.xml` & `trytond_stock_package_shipping_sendcloud-7.2.0/carrier.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/carrier.xml` & `trytond_stock_package_shipping_sendcloud-7.2.0/carrier.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_credential_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="credential_view_form"/>
       <field name="act_window" ref="act_credential_form"/>
     </record>
     <menuitem parent="carrier.menu_configuration" action="act_credential_form" sequence="20" id="menu_credential_form"/>
     <record model="ir.model.access" id="access_credential">
-      <field name="model" search="[('model', '=', 'carrier.credential.sendcloud')]"/>
+      <field name="model">carrier.credential.sendcloud</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_credential_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.credential.sendcloud')]"/>
+      <field name="model">carrier.credential.sendcloud</field>
       <field name="group" ref="carrier.group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="carrier_address_view_form">
@@ -50,22 +50,22 @@
     </record>
     <record model="ir.ui.view" id="carrier_address_view_list">
       <field name="model">carrier.sendcloud.address</field>
       <field name="type">tree</field>
       <field name="name">carrier_address_list</field>
     </record>
     <record model="ir.model.access" id="access_carrier_address">
-      <field name="model" search="[('model', '=', 'carrier.sendcloud.address')]"/>
+      <field name="model">carrier.sendcloud.address</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_address_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.sendcloud.address')]"/>
+      <field name="model">carrier.sendcloud.address</field>
       <field name="group" ref="carrier.group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="carrier_shipping_method_view_form">
@@ -75,22 +75,22 @@
     </record>
     <record model="ir.ui.view" id="carrier_shipping_method_view_list">
       <field name="model">carrier.sendcloud.shipping_method</field>
       <field name="type">tree</field>
       <field name="name">carrier_shipping_method_list</field>
     </record>
     <record model="ir.model.access" id="access_carrier_shipping_method">
-      <field name="model" search="[('model', '=', 'carrier.sendcloud.shipping_method')]"/>
+      <field name="model">carrier.sendcloud.shipping_method</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_shipping_method_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.sendcloud.shipping_method')]"/>
+      <field name="model">carrier.sendcloud.shipping_method</field>
       <field name="group" ref="carrier.group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="carrier_view_form">
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/doc/conf.py` & `trytond_stock_package_shipping_sendcloud-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/doc/configuration.rst` & `trytond_stock_package_shipping_sendcloud-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/doc/design.rst` & `trytond_stock_package_shipping_sendcloud-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/bg.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/ca.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/cs.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/de.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/es.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/es_419.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/et.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/fa.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/fi.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/fr.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/hu.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/id.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/it.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/it.po`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 msgid ""
 "Sendcloud webservice call failed with the following error message:\n"
 "%(message)s"
 msgstr ""
 "La chiamata al servizio web Sendcloud non è fallita con il seguente messaggio di errore:\n"
 "%(message)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_shipment_has_shipping_reference_number"
 msgid ""
 "You cannot create a shipping label for shipment \"%(shipment)s\" because it "
 "already has a shipping reference number."
 msgstr ""
 "Non puoi creare un'etichetta di spedizione per la spedizione "
 "\"%(shipment)s\" perché ha già un numero di riferimento."
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/lo.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/lt.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/nl.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/pl.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/pt.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/ro.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
 msgctxt "model:ir.message,text:msg_sendcloud_webserver_error"
 msgid ""
 "Sendcloud webservice call failed with the following error message:\n"
 "%(message)s"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_shipment_has_shipping_reference_number"
 msgid ""
 "You cannot create a shipping label for shipment \"%(shipment)s\" because it "
 "already has a shipping reference number."
 msgstr ""
 "Nu se poate crea o eticheta pentru expedierea \"%(shipment)s\" pentru că are"
 " deja un număr de referinţa."
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/ru.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/sl.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/tr.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/uk.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/locale/zh_CN.po` & `trytond_stock_package_shipping_sendcloud-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/message.xml` & `trytond_stock_package_shipping_sendcloud-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/setup.py` & `trytond_stock_package_shipping_sendcloud-7.2.0/setup.py`

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
             'modules-stock-package-shipping-sendcloud'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping sendcloud',
     package_dir={'trytond.modules.stock_package_shipping_sendcloud': '.'},
     packages=(
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/stock.py` & `trytond_stock_package_shipping_sendcloud-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/tests/scenario_stock_package_shipping_sendcloud.rst` & `trytond_stock_package_shipping_sendcloud-7.2.0/tests/scenario_stock_package_shipping_sendcloud.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
     >>> import os
     >>> from decimal import Decimal
     >>> from random import randint
 
     >>> import requests
 
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
     >>> from trytond.modules.stock_package_shipping_sendcloud.carrier import (
     ...     SENDCLOUD_API_URL)
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['stock_package_shipping_sendcloud', 'sale', 'sale_shipment_cost'])
 
     >>> Address = Model.get('party.address')
@@ -219,14 +218,15 @@
     True
     >>> pack.shipping_label is not None
     True
     >>> pack.shipping_label_mimetype
     'application/pdf'
     >>> pack.shipping_reference is not None
     True
-    >>> pack.shipping_tracking_url.startswith('http')
-    True
+    >>> pack.shipping_tracking_url
+    'http...'
 
 Clean up::
 
-    >>> _ = requests.post(SENDCLOUD_API_URL + 'parcels/%s/cancel' % pack.sendcloud_shipping_id,
+    >>> _ = requests.post(
+    ...     SENDCLOUD_API_URL + 'parcels/%s/cancel' % pack.sendcloud_shipping_id,
     ...     auth=(credential.public_key, credential.secret_key))
```

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/tox.ini` & `trytond_stock_package_shipping_sendcloud-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_sendcloud-7.2.0/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt`

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

### Comparing `trytond_stock_package_shipping_sendcloud-7.0.1/view/credential_form.xml` & `trytond_stock_package_shipping_sendcloud-7.2.0/view/credential_form.xml`

 * *Files identical despite different names*

