# Comparing `tmp/trytond_carrier-7.0.0.tar.gz` & `tmp/trytond_carrier-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier-7.0.0.tar", last modified: Mon Oct 30 17:27:42 2023, max compression
+gzip compressed data, was "trytond_carrier-7.2.0.tar", last modified: Mon Apr 29 15:38:36 2024, max compression
```

## Comparing `trytond_carrier-7.0.0.tar` & `trytond_carrier-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.354822 trytond_carrier-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-22 17:23:00.000000 trytond_carrier-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2370 2023-10-30 17:05:10.000000 trytond_carrier-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:05:10.000000 trytond_carrier-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3339 2023-10-30 17:27:42.354822 trytond_carrier-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-01-16 14:00:20.000000 trytond_carrier-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5115 2023-08-13 15:26:13.000000 trytond_carrier-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6323 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.351489 trytond_carrier-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-22 17:23:00.000000 trytond_carrier-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-01-16 14:00:20.000000 trytond_carrier-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:00.000000 trytond_carrier-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.351489 trytond_carrier-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-01-16 14:00:20.000000 trytond_carrier-7.0.0/icons/tryton-carrier.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.351489 trytond_carrier-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2704 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2717 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2175 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2563 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2959 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2718 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2780 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2334 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2398 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2949 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-10-30 16:47:45.000000 trytond_carrier-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2332 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2506 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2575 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2296 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2429 2023-10-30 16:47:45.000000 trytond_carrier-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2108 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-10-28 12:11:21.000000 trytond_carrier-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:27:42.354822 trytond_carrier-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4217 2023-10-27 17:38:49.000000 trytond_carrier-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.351489 trytond_carrier-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_carrier-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-10-30 17:05:06.000000 trytond_carrier-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.354822 trytond_carrier-7.0.0/trytond_carrier.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3339 2023-10-30 17:27:41.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1624 2023-10-30 17:27:42.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:27:41.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-10-30 17:27:41.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2023-10-30 17:27:41.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:27:41.000000 trytond_carrier-7.0.0/trytond_carrier.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:42.351489 trytond_carrier-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/view/carrier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-01-16 14:00:20.000000 trytond_carrier-7.0.0/view/selection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/view/selection_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_carrier-7.0.0/view/selection_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.112309 trytond_carrier-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2024-04-29 15:18:20.000000 trytond_carrier-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:18:19.000000 trytond_carrier-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3339 2024-04-29 15:38:36.112309 trytond_carrier-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-01-16 14:00:20.000000 trytond_carrier-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5115 2024-01-27 09:58:52.000000 trytond_carrier-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6231 2024-04-27 16:30:39.000000 trytond_carrier-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.108976 trytond_carrier-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_carrier-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-01-16 14:00:20.000000 trytond_carrier-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:05.000000 trytond_carrier-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.108976 trytond_carrier-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-01-16 14:00:20.000000 trytond_carrier-7.2.0/icons/tryton-carrier.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.108976 trytond_carrier-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2704 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2717 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2175 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2563 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2959 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2718 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2780 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2334 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2398 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2332 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2506 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2575 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2296 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2429 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2108 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2024-04-27 16:43:22.000000 trytond_carrier-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:36.112309 trytond_carrier-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4217 2024-03-17 11:01:36.000000 trytond_carrier-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.108976 trytond_carrier-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:05.000000 trytond_carrier-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-29 15:18:15.000000 trytond_carrier-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.112309 trytond_carrier-7.2.0/trytond_carrier.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3339 2024-04-29 15:38:35.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1606 2024-04-29 15:38:36.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:35.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:38:35.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-04-29 15:38:35.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:35.000000 trytond_carrier-7.2.0/trytond_carrier.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:36.112309 trytond_carrier-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/view/carrier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-01-16 14:00:20.000000 trytond_carrier-7.2.0/view/selection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/view/selection_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_carrier-7.2.0/view/selection_list_sequence.xml
```

### Comparing `trytond_carrier-7.0.0/CHANGELOG` & `trytond_carrier-7.2.0/CHANGELOG`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_carrier-7.0.0/COPYRIGHT` & `trytond_carrier-7.2.0/COPYRIGHT`

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

### Comparing `trytond_carrier-7.0.0/LICENSE` & `trytond_carrier-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/PKG-INFO` & `trytond_carrier-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_carrier
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with carriers
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Carrier Module
 ##############
 
 The carrier module defines the concept of carrier.
 
 Carrier
```

### Comparing `trytond_carrier-7.0.0/README.rst` & `trytond_carrier-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/carrier.py` & `trytond_carrier-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/carrier.xml` & `trytond_carrier-7.2.0/carrier.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_carrier-7.0.0/carrier.xml` & `trytond_carrier-7.2.0/carrier.xml`

```diff
@@ -46,22 +46,22 @@
     <record model="ir.action.act_window.view" id="act_carrier_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="carrier_view_form"/>
       <field name="act_window" ref="act_carrier_form"/>
     </record>
     <menuitem parent="menu_carrier" action="act_carrier_form" sequence="10" id="menu_carrier_form"/>
     <record model="ir.model.access" id="access_carrier">
-      <field name="model" search="[('model', '=', 'carrier')]"/>
+      <field name="model">carrier</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier')]"/>
+      <field name="model">carrier</field>
       <field name="group" ref="group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="carrier_selection_view_form">
@@ -93,22 +93,22 @@
     <record model="ir.action.act_window.view" id="act_carrier_selection_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="carrier_selection_view_form"/>
       <field name="act_window" ref="act_carrier_selection_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_carrier_selection_form" sequence="20" id="menu_carrier_selection"/>
     <record model="ir.model.access" id="access_carrier_selection">
-      <field name="model" search="[('model', '=', 'carrier.selection')]"/>
+      <field name="model">carrier.selection</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_selection_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.selection')]"/>
+      <field name="model">carrier.selection</field>
       <field name="group" ref="group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_carrier-7.0.0/doc/conf.py` & `trytond_carrier-7.2.0/doc/conf.py`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_carrier-7.0.0/doc/index.rst` & `trytond_carrier-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/icons/LICENSE` & `trytond_carrier-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/bg.po` & `trytond_carrier-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/ca.po` & `trytond_carrier-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/cs.po` & `trytond_carrier-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/de.po` & `trytond_carrier-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/es.po` & `trytond_carrier-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/es_419.po` & `trytond_carrier-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/et.po` & `trytond_carrier-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/fa.po` & `trytond_carrier-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/fi.po` & `trytond_carrier-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/fr.po` & `trytond_carrier-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/hu.po` & `trytond_carrier-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/id.po` & `trytond_carrier-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/it.po` & `trytond_carrier-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/lo.po` & `trytond_carrier-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/lt.po` & `trytond_carrier-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/nl.po` & `trytond_carrier-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/pl.po` & `trytond_carrier-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/pt.po` & `trytond_carrier-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/ro.po` & `trytond_carrier-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/ru.po` & `trytond_carrier-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/sl.po` & `trytond_carrier-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/tr.po` & `trytond_carrier-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/uk.po` & `trytond_carrier-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/locale/zh_CN.po` & `trytond_carrier-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/setup.py` & `trytond_carrier-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/tox.ini` & `trytond_carrier-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_carrier-7.0.0/trytond_carrier.egg-info/PKG-INFO` & `trytond_carrier-7.2.0/trytond_carrier.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-carrier
-Version: 7.0.0
+Name: trytond_carrier
+Version: 7.2.0
 Summary: Tryton module with carriers
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Carrier Module
 ##############
 
 The carrier module defines the concept of carrier.
 
 Carrier
```

### Comparing `trytond_carrier-7.0.0/trytond_carrier.egg-info/SOURCES.txt` & `trytond_carrier-7.2.0/trytond_carrier.egg-info/SOURCES.txt`

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
 carrier.py
```

