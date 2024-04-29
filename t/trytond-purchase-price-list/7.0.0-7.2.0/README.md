# Comparing `tmp/trytond_purchase_price_list-7.0.0.tar.gz` & `tmp/trytond_purchase_price_list-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_price_list-7.0.0.tar", last modified: Mon Oct 30 17:35:34 2023, max compression
+gzip compressed data, was "trytond_purchase_price_list-7.2.0.tar", last modified: Mon Apr 29 15:45:59 2024, max compression
```

## Comparing `trytond_purchase_price_list-7.0.0.tar` & `trytond_purchase_price_list-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:34.907076 trytond_purchase_price_list-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-22 17:23:14.000000 trytond_purchase_price_list-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-10-30 17:10:40.000000 trytond_purchase_price_list-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:10:40.000000 trytond_purchase_price_list-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-30 17:35:34.907076 trytond_purchase_price_list-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:34.907076 trytond_purchase_price_list-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-22 17:23:14.000000 trytond_purchase_price_list-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:14.000000 trytond_purchase_price_list-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:34.903743 trytond_purchase_price_list-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      937 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-28 12:11:24.000000 trytond_purchase_price_list-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1893 2023-10-07 15:40:36.000000 trytond_purchase_price_list-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:35:34.907076 trytond_purchase_price_list-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4627 2023-10-27 17:38:49.000000 trytond_purchase_price_list-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:34.903743 trytond_purchase_price_list-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2548 2023-10-24 07:56:52.000000 trytond_purchase_price_list-7.0.0/tests/scenario_purchase_price_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_price_list-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-30 17:10:36.000000 trytond_purchase_price_list-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:34.907076 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-30 17:35:34.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1606 2023-10-30 17:35:34.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:35:34.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:35:34.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2023-10-30 17:35:34.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:35:34.000000 trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:34.903743 trytond_purchase_price_list-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-29 15:23:50.000000 trytond_purchase_price_list-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:23:49.000000 trytond_purchase_price_list-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2813 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:59.974033 trytond_purchase_price_list-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_purchase_price_list-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:21.000000 trytond_purchase_price_list-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      937 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_purchase_price_list-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1419 2024-04-22 12:14:36.000000 trytond_purchase_price_list-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1893 2024-02-04 18:51:26.000000 trytond_purchase_price_list-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4618 2024-04-27 16:30:39.000000 trytond_purchase_price_list-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-04-22 12:14:36.000000 trytond_purchase_price_list-7.2.0/tests/scenario_purchase_price_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:21.000000 trytond_purchase_price_list-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-29 15:23:45.000000 trytond_purchase_price_list-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2813 2024-04-29 15:45:59.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1588 2024-04-29 15:45:59.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:59.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:45:59.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-29 15:45:59.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:59.000000 trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:59.977366 trytond_purchase_price_list-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_purchase_price_list-7.2.0/view/party_form.xml
```

### Comparing `trytond_purchase_price_list-7.0.0/CHANGELOG` & `trytond_purchase_price_list-7.2.0/CHANGELOG`

 * *Files 25% similar despite different names*

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

### Comparing `trytond_purchase_price_list-7.0.0/COPYRIGHT` & `trytond_purchase_price_list-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_price_list-7.0.0/LICENSE` & `trytond_purchase_price_list-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/PKG-INFO` & `trytond_purchase_price_list-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_price_list
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add price list on purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase-price-list
+Project-URL: Documentation, https://docs.tryton.org/modules-purchase-price-list
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase price list
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,23 +47,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##########################
 Purchase Price List Module
 ##########################
 
 The *Purchase Price List Module* allows price lists to be defined for
 suppliers.
```

### Comparing `trytond_purchase_price_list-7.0.0/doc/conf.py` & `trytond_purchase_price_list-7.2.0/doc/conf.py`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_purchase_price_list-7.0.0/doc/design.rst` & `trytond_purchase_price_list-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/bg.po` & `trytond_purchase_price_list-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/ca.po` & `trytond_purchase_price_list-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/cs.po` & `trytond_purchase_price_list-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/de.po` & `trytond_purchase_price_list-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/es.po` & `trytond_purchase_price_list-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/es_419.po` & `trytond_purchase_price_list-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/et.po` & `trytond_purchase_price_list-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/fa.po` & `trytond_purchase_price_list-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/fi.po` & `trytond_purchase_price_list-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/fr.po` & `trytond_purchase_price_list-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/hu.po` & `trytond_purchase_price_list-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/id.po` & `trytond_purchase_price_list-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/it.po` & `trytond_purchase_price_list-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/lo.po` & `trytond_purchase_price_list-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/lt.po` & `trytond_purchase_price_list-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/nl.po` & `trytond_purchase_price_list-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/pl.po` & `trytond_purchase_price_list-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/pt.po` & `trytond_purchase_price_list-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/ro.po` & `trytond_purchase_price_list-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/ru.po` & `trytond_purchase_price_list-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/sl.po` & `trytond_purchase_price_list-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/tr.po` & `trytond_purchase_price_list-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/uk.po` & `trytond_purchase_price_list-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/locale/zh_CN.po` & `trytond_purchase_price_list-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/party.py` & `trytond_purchase_price_list-7.2.0/party.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     party = fields.Many2One(
         'party.party', "Party", ondelete='CASCADE',
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     purchase_price_list = fields.Many2One(
-        'product.price_list', "Purchase Price List",
+        'product.price_list', "Purchase Price List", ondelete='RESTRICT',
         domain=[
             ('company', '=', Eval('company', -1)),
             ])
```

### Comparing `trytond_purchase_price_list-7.0.0/product.py` & `trytond_purchase_price_list-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/purchase.py` & `trytond_purchase_price_list-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/setup.py` & `trytond_purchase_price_list-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-purchase-price-list'),
+            'https://docs.tryton.org/modules-purchase-price-list'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase price list',
     package_dir={'trytond.modules.purchase_price_list': '.'},
     packages=(
         ['trytond.modules.purchase_price_list']
```

### Comparing `trytond_purchase_price_list-7.0.0/tests/scenario_purchase_price_list.rst` & `trytond_purchase_price_list-7.2.0/tests/scenario_purchase_price_list.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ============================
 Purchase Price List Scenario
 ============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+
+    >>> from proteus import Model
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('purchase_price_list')
 
     >>> Party = Model.get('party.party')
     >>> PriceList = Model.get('product.price_list')
```

### Comparing `trytond_purchase_price_list-7.0.0/tox.ini` & `trytond_purchase_price_list-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/PKG-INFO` & `trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-price-list
-Version: 7.0.0
+Name: trytond_purchase_price_list
+Version: 7.2.0
 Summary: Tryton module to add price list on purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase-price-list
+Project-URL: Documentation, https://docs.tryton.org/modules-purchase-price-list
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase price list
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,23 +47,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##########################
 Purchase Price List Module
 ##########################
 
 The *Purchase Price List Module* allows price lists to be defined for
 suppliers.
```

### Comparing `trytond_purchase_price_list-7.0.0/trytond_purchase_price_list.egg-info/SOURCES.txt` & `trytond_purchase_price_list-7.2.0/trytond_purchase_price_list.egg-info/SOURCES.txt`

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

