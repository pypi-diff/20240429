# Comparing `tmp/trytond_web_shop_vue_storefront-7.0.0.tar.gz` & `tmp/trytond_web_shop_vue_storefront-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_vue_storefront-7.0.0.tar", last modified: Mon Oct 30 17:45:24 2023, max compression
+gzip compressed data, was "trytond_web_shop_vue_storefront-7.2.0.tar", last modified: Mon Apr 29 15:54:17 2024, max compression
```

## Comparing `trytond_web_shop_vue_storefront-7.0.0.tar` & `trytond_web_shop_vue_storefront-7.2.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:24.053220 trytond_web_shop_vue_storefront-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:23:30.000000 trytond_web_shop_vue_storefront-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      746 2023-10-30 17:16:27.000000 trytond_web_shop_vue_storefront-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:16:26.000000 trytond_web_shop_vue_storefront-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3482 2023-10-30 17:45:24.053220 trytond_web_shop_vue_storefront-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/carrier.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:24.049886 trytond_web_shop_vue_storefront-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:23:30.000000 trytond_web_shop_vue_storefront-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:30.000000 trytond_web_shop_vue_storefront-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:24.049886 trytond_web_shop_vue_storefront-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-10-30 16:47:45.000000 trytond_web_shop_vue_storefront-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2226 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2256 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1788 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2219 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2174 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-28 12:11:27.000000 trytond_web_shop_vue_storefront-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1561 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4908 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8819 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9014 2023-10-07 15:40:36.000000 trytond_web_shop_vue_storefront-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:45:24.053220 trytond_web_shop_vue_storefront-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4904 2023-10-27 17:38:49.000000 trytond_web_shop_vue_storefront-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:24.049886 trytond_web_shop_vue_storefront-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10462 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/tests/scenario_web_shop_vue_storefront.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    33611 2023-10-07 17:14:58.000000 trytond_web_shop_vue_storefront-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_web_shop_vue_storefront-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-30 17:16:21.000000 trytond_web_shop_vue_storefront-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:24.053220 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3482 2023-10-30 17:45:23.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1760 2023-10-30 17:45:24.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:45:23.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:45:23.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:45:23.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:45:23.000000 trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:24.049886 trytond_web_shop_vue_storefront-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22936 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.0.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:17.834345 trytond_web_shop_vue_storefront-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2024-04-29 15:30:06.000000 trytond_web_shop_vue_storefront-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:30:06.000000 trytond_web_shop_vue_storefront-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3482 2024-04-29 15:54:17.834345 trytond_web_shop_vue_storefront-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/carrier.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:17.831012 trytond_web_shop_vue_storefront-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_web_shop_vue_storefront-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:39.000000 trytond_web_shop_vue_storefront-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:17.831012 trytond_web_shop_vue_storefront-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2226 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1788 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2219 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2174 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-27 16:43:28.000000 trytond_web_shop_vue_storefront-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1561 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4908 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8819 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9014 2024-02-04 18:51:27.000000 trytond_web_shop_vue_storefront-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:17.834345 trytond_web_shop_vue_storefront-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4904 2024-03-17 11:01:36.000000 trytond_web_shop_vue_storefront-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:17.834345 trytond_web_shop_vue_storefront-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10432 2024-04-22 12:14:37.000000 trytond_web_shop_vue_storefront-7.2.0/tests/scenario_web_shop_vue_storefront.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    33611 2024-02-04 18:51:27.000000 trytond_web_shop_vue_storefront-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:39.000000 trytond_web_shop_vue_storefront-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2024-04-29 15:30:02.000000 trytond_web_shop_vue_storefront-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:17.834345 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3482 2024-04-29 15:54:17.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1742 2024-04-29 15:54:17.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:17.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:54:17.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-29 15:54:17.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:17.000000 trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:17.834345 trytond_web_shop_vue_storefront-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22936 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront-7.2.0/web.xml
```

### Comparing `trytond_web_shop_vue_storefront-7.0.0/CHANGELOG` & `trytond_web_shop_vue_storefront-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_web_shop_vue_storefront-7.0.0/COPYRIGHT` & `trytond_web_shop_vue_storefront-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2023 B2CK
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 B2CK
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_web_shop_vue_storefront-7.0.0/LICENSE` & `trytond_web_shop_vue_storefront-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/PKG-INFO` & `trytond_web_shop_vue_storefront-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_vue_storefront
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to integrate with Vue Storefront
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
@@ -49,27 +49,27 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: elasticsearch
 Requires-Dist: python-stdnum>=1.1.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_web_shop<7.1,>=7.0
-Requires-Dist: trytond_web_user<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_web_shop<7.3,>=7.2
+Requires-Dist: trytond_web_user<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_attribute<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_image<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_promotion_coupon<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_attribute<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_promotion_coupon<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier<7.3,>=7.2; extra == "test"
 
 Web Vue Storefront Module
 #########################
 
 The web_shop_vue_storefront module provides the back-end to integrate with `Vue
 Storefront`_ 1.x.
```

### Comparing `trytond_web_shop_vue_storefront-7.0.0/__init__.py` & `trytond_web_shop_vue_storefront-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/carrier.py` & `trytond_web_shop_vue_storefront-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/doc/conf.py` & `trytond_web_shop_vue_storefront-7.2.0/doc/conf.py`

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

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/bg.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/ca.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/cs.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/de.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/es.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/es_419.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/et.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/fa.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/fi.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/fr.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/hu.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/id.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/it.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/lo.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/lt.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/nl.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/pl.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/pt.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/ro.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/ru.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/sl.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/tr.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/uk.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/locale/zh_CN.po` & `trytond_web_shop_vue_storefront-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/message.xml` & `trytond_web_shop_vue_storefront-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/party.py` & `trytond_web_shop_vue_storefront-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/product.py` & `trytond_web_shop_vue_storefront-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/routes.py` & `trytond_web_shop_vue_storefront-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/sale.py` & `trytond_web_shop_vue_storefront-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/setup.py` & `trytond_web_shop_vue_storefront-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/tests/scenario_web_shop_vue_storefront.rst` & `trytond_web_shop_vue_storefront-7.2.0/tests/scenario_web_shop_vue_storefront.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 Web Shop Vue Storefront Scenario
 ================================
 
 Imports::
 
     >>> import base64
     >>> from decimal import Decimal
-    >>> from unittest.mock import MagicMock, ANY, patch
+    >>> from unittest.mock import ANY, MagicMock, patch
 
     >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.web_shop_vue_storefront import web
+    >>> from trytond.modules.web_shop_vue_storefront.tests.tools import AnyDictWith
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
-
-    >>> from trytond.modules.web_shop_vue_storefront.tests.tools import (
-    ...     AnyDictWith)
 
     >>> pixel = base64.decodebytes(
-    ...     b'/9j/4AAQSkZJRgABAQEASABIAAD/2wBDAAUDBAQEAwUEBAQFBQUGBwwIBwcHBw8LCwkMEQ8SEhEP'
-    ...     b'ERETFhwXExQaFRERGCEYGh0dHx8fExciJCIeJBweHx7/wAALCAABAAEBAREA/8QAHwAAAQUBAQEB'
-    ...     b'AQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1Fh'
-    ...     b'ByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZ'
-    ...     b'WmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXG'
-    ...     b'x8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/9oACAEBAAA/APsuv//Z')
+    ...     b'/9j/4AAQSkZJRgABAQEASABIAAD/2wBDAAUDBAQEAwUEBAQFBQUGBwwIBwcHBw8LCwkMEQ8S'
+    ...     b'EhEPERETFhwXExQaFRERGCEYGh0dHx8fExciJCIeJBweHx7/wAALCAABAAEBAREA/8QAHwAA'
+    ...     b'AQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQR'
+    ...     b'BRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RF'
+    ...     b'RkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ip'
+    ...     b'qrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/9oACAEB'
+    ...     b'AAA/APsuv//Z')
 
 Patch elasticsearch::
 
-    >>> from trytond.modules.web_shop_vue_storefront import web
     >>> es = MagicMock()
     >>> _ = patch.object(
     ...     web, 'VSFElasticsearch', return_value=es).start()
 
 Install web_shop_vue_storefront::
 
     >>> config = activate_modules(
```

### Comparing `trytond_web_shop_vue_storefront-7.0.0/tests/test_module.py` & `trytond_web_shop_vue_storefront-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/tox.ini` & `trytond_web_shop_vue_storefront-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/PKG-INFO` & `trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-web-shop-vue-storefront
-Version: 7.0.0
+Name: trytond_web_shop_vue_storefront
+Version: 7.2.0
 Summary: Tryton module to integrate with Vue Storefront
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
@@ -49,27 +49,27 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: elasticsearch
 Requires-Dist: python-stdnum>=1.1.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_web_shop<7.1,>=7.0
-Requires-Dist: trytond_web_user<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_web_shop<7.3,>=7.2
+Requires-Dist: trytond_web_user<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_attribute<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_image<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_promotion_coupon<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_attribute<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_promotion_coupon<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier<7.3,>=7.2; extra == "test"
 
 Web Vue Storefront Module
 #########################
 
 The web_shop_vue_storefront module provides the back-end to integrate with `Vue
 Storefront`_ 1.x.
```

### Comparing `trytond_web_shop_vue_storefront-7.0.0/trytond_web_shop_vue_storefront.egg-info/SOURCES.txt` & `trytond_web_shop_vue_storefront-7.2.0/trytond_web_shop_vue_storefront.egg-info/SOURCES.txt`

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

### Comparing `trytond_web_shop_vue_storefront-7.0.0/view/shop_form.xml` & `trytond_web_shop_vue_storefront-7.2.0/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/web.py` & `trytond_web_shop_vue_storefront-7.2.0/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront-7.0.0/web.xml` & `trytond_web_shop_vue_storefront-7.2.0/web.xml`

 * *Files identical despite different names*

