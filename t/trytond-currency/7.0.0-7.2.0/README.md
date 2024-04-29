# Comparing `tmp/trytond_currency-7.0.0.tar.gz` & `tmp/trytond_currency-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_currency-7.0.0.tar", last modified: Mon Oct 30 17:29:10 2023, max compression
+gzip compressed data, was "trytond_currency-7.2.0.tar", last modified: Mon Apr 29 15:39:43 2024, max compression
```

## Comparing `trytond_currency-7.0.0.tar` & `trytond_currency-7.2.0.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.138574 trytond_currency-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      197 2023-10-22 17:23:02.000000 trytond_currency-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3883 2023-10-30 17:05:57.000000 trytond_currency-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:05:56.000000 trytond_currency-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_currency-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2978 2023-10-30 17:29:10.138574 trytond_currency-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15628 2023-08-13 15:26:13.000000 trytond_currency-7.0.0/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6572 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.135241 trytond_currency-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2809 2023-10-22 17:23:02.000000 trytond_currency-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:02.000000 trytond_currency-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-08-13 15:26:13.000000 trytond_currency-7.0.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/ecb.py
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1364 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.138574 trytond_currency-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_currency-7.0.0/icons/tryton-currency.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.131908 trytond_currency-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5012 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5977 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4810 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5914 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5185 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5949 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5901 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5480 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5615 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5532 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5369 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5853 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5764 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5654 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5806 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5186 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5594 2023-10-30 16:47:45.000000 trytond_currency-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6453 2023-10-28 12:11:22.000000 trytond_currency-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5508 2023-10-30 16:47:45.000000 trytond_currency-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/message.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.135241 trytond_currency-7.0.0/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3222 2023-10-07 15:40:36.000000 trytond_currency-7.0.0/scripts/import_currencies.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:29:10.138574 trytond_currency-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4810 2023-10-27 17:38:49.000000 trytond_currency-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.135241 trytond_currency-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/tests/scenario_currency_compute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/tests/scenario_currency_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1295 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/tests/scenario_currency_rate_update.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14824 2023-06-10 11:39:56.000000 trytond_currency-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-08-13 15:26:13.000000 trytond_currency-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_currency-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-10-30 17:05:53.000000 trytond_currency-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.138574 trytond_currency-7.0.0/trytond_currency.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2978 2023-10-30 17:29:09.000000 trytond_currency-7.0.0/trytond_currency.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2327 2023-10-30 17:29:10.000000 trytond_currency-7.0.0/trytond_currency.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:09.000000 trytond_currency-7.0.0/trytond_currency.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-10-30 17:29:09.000000 trytond_currency-7.0.0/trytond_currency.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_currency-7.0.0/trytond_currency.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-10-30 17:29:09.000000 trytond_currency-7.0.0/trytond_currency.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:29:09.000000 trytond_currency-7.0.0/trytond_currency.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:10.135241 trytond_currency-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-07 15:40:36.000000 trytond_currency-7.0.0/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-01-16 14:00:20.000000 trytond_currency-7.0.0/view/currency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_currency-7.0.0/view/currency_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:20.000000 trytond_currency-7.0.0/view/currency_rate_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/view/currency_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-04-15 07:12:15.000000 trytond_currency-7.0.0/view/currency_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3984 2024-04-29 15:19:11.000000 trytond_currency-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:19:10.000000 trytond_currency-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15628 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-27 16:30:39.000000 trytond_currency-7.2.0/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_currency-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:08.000000 trytond_currency-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/ecb.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1364 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/icons/tryton-currency.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5012 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5977 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4810 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5914 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5185 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5949 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5901 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5480 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5615 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5532 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5369 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5853 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5764 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5654 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5806 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5594 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6453 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5508 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/message.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3222 2024-02-04 18:51:26.000000 trytond_currency-7.2.0/scripts/import_currencies.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4801 2024-04-27 16:30:39.000000 trytond_currency-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-22 12:14:36.000000 trytond_currency-7.2.0/tests/scenario_currency_compute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-22 12:14:36.000000 trytond_currency-7.2.0/tests/scenario_currency_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1296 2024-04-22 12:14:36.000000 trytond_currency-7.2.0/tests/scenario_currency_rate_update.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14824 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:08.000000 trytond_currency-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-04-29 15:19:06.000000 trytond_currency-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/trytond_currency.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2309 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_currency-7.2.0/trytond_currency.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/view/currency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/view/currency_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/view/currency_rate_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/view/currency_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/view/currency_tree.xml
```

### Comparing `trytond_currency-7.0.0/CHANGELOG` & `trytond_currency-7.2.0/CHANGELOG`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_currency-7.0.0/LICENSE` & `trytond_currency-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/PKG-INFO` & `trytond_currency-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-currency/
+Project-URL: Documentation, https://docs.tryton.org/modules-currency/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton currency
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
@@ -51,20 +51,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.9
 Requires-Dist: python-dateutil
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: data
 Requires-Dist: pycountry; extra == "data"
-Requires-Dist: proteus<7.1,>=7.0; extra == "data"
+Requires-Dist: proteus<7.3,>=7.2; extra == "data"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 Requires-Dist: pycountry; extra == "test"
 Provides-Extra: completion
 Requires-Dist: argcomplete; extra == "completion"
 
 ###############
 Currency Module
 ###############
```

### Comparing `trytond_currency-7.0.0/currency.py` & `trytond_currency-7.2.0/currency.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/currency.xml` & `trytond_currency-7.2.0/currency.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_currency-7.0.0/currency.xml` & `trytond_currency-7.2.0/currency.xml`

```diff
@@ -41,22 +41,22 @@
     <record model="ir.action.act_window.view" id="act_currency_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="currency_view_form"/>
       <field name="act_window" ref="act_currency_form"/>
     </record>
     <menuitem parent="menu_currency" action="act_currency_form" sequence="10" id="menu_currency_form"/>
     <record model="ir.model.access" id="access_currency">
-      <field name="model" search="[('model', '=', 'currency.currency')]"/>
+      <field name="model">currency.currency</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_currency_currency_admin">
-      <field name="model" search="[('model', '=', 'currency.currency')]"/>
+      <field name="model">currency.currency</field>
       <field name="group" ref="group_currency_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="currency_rate_view_list">
@@ -96,32 +96,32 @@
     <record model="ir.action.act_window.view" id="act_cron_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="cron_view_form"/>
       <field name="act_window" ref="act_cron_form"/>
     </record>
     <menuitem parent="menu_currency" action="act_cron_form" sequence="20" id="menu_cron_form"/>
     <record model="ir.model.access" id="access_cron">
-      <field name="model" search="[('model', '=', 'currency.cron')]"/>
+      <field name="model">currency.cron</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_cron_currency_admin">
-      <field name="model" search="[('model', '=', 'currency.cron')]"/>
+      <field name="model">currency.cron</field>
       <field name="group" ref="group_currency_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="cron_run_button">
+      <field name="model">currency.cron</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'currency.cron')]"/>
     </record>
     <record model="ir.cron" id="cron_cron">
       <field name="method">currency.cron|update</field>
       <field name="interval_number" eval="1"/>
       <field name="interval_type">days</field>
     </record>
   </data>
```

### Comparing `trytond_currency-7.0.0/doc/conf.py` & `trytond_currency-7.2.0/doc/conf.py`

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

### Comparing `trytond_currency-7.0.0/doc/configuration.rst` & `trytond_currency-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/doc/design.rst` & `trytond_currency-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/doc/usage.rst` & `trytond_currency-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/ecb.py` & `trytond_currency-7.2.0/ecb.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/fields.py` & `trytond_currency-7.2.0/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/icons/LICENSE` & `trytond_currency-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/ir.py` & `trytond_currency-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/bg.po` & `trytond_currency-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/ca.po` & `trytond_currency-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/cs.po` & `trytond_currency-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/de.po` & `trytond_currency-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/es.po` & `trytond_currency-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/es_419.po` & `trytond_currency-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/et.po` & `trytond_currency-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/fa.po` & `trytond_currency-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/fi.po` & `trytond_currency-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/fr.po` & `trytond_currency-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/hu.po` & `trytond_currency-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/id.po` & `trytond_currency-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/it.po` & `trytond_currency-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/lo.po` & `trytond_currency-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/lt.po` & `trytond_currency-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/nl.po` & `trytond_currency-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/pl.po` & `trytond_currency-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/pt.po` & `trytond_currency-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/ro.po` & `trytond_currency-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/ru.po` & `trytond_currency-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/sl.po` & `trytond_currency-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/tr.po` & `trytond_currency-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/uk.po` & `trytond_currency-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/locale/zh_CN.po` & `trytond_currency-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/message.xml` & `trytond_currency-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/scripts/import_currencies.py` & `trytond_currency-7.2.0/scripts/import_currencies.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/setup.py` & `trytond_currency-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-currency/',
+        "Documentation": 'https://docs.tryton.org/modules-currency/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton currency',
     package_dir={'trytond.modules.currency': '.'},
     packages=(
         ['trytond.modules.currency']
```

### Comparing `trytond_currency-7.0.0/tests/scenario_currency_compute.rst` & `trytond_currency-7.2.0/tests/scenario_currency_compute.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 =========================
 Currency Compute Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('currency')
 
 Call compute::
```

### Comparing `trytond_currency-7.0.0/tests/scenario_currency_rate_update.rst` & `trytond_currency-7.2.0/tests/scenario_currency_rate_update.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ====================
 Currency Rate Update
 ====================
 
 Imports::
 
     >>> import datetime as dt
+
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
     >>> previous_week = today - dt.timedelta(days=7)
     >>> before_previous_week = previous_week - dt.timedelta(days=1)
```

### Comparing `trytond_currency-7.0.0/tests/test_module.py` & `trytond_currency-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/tests/tools.py` & `trytond_currency-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/tox.ini` & `trytond_currency-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/trytond_currency.egg-info/PKG-INFO` & `trytond_currency-7.2.0/trytond_currency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-currency
-Version: 7.0.0
+Name: trytond_currency
+Version: 7.2.0
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-currency/
+Project-URL: Documentation, https://docs.tryton.org/modules-currency/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton currency
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
@@ -51,20 +51,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.9
 Requires-Dist: python-dateutil
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: data
 Requires-Dist: pycountry; extra == "data"
-Requires-Dist: proteus<7.1,>=7.0; extra == "data"
+Requires-Dist: proteus<7.3,>=7.2; extra == "data"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 Requires-Dist: pycountry; extra == "test"
 Provides-Extra: completion
 Requires-Dist: argcomplete; extra == "completion"
 
 ###############
 Currency Module
 ###############
```

### Comparing `trytond_currency-7.0.0/trytond_currency.egg-info/SOURCES.txt` & `trytond_currency-7.2.0/trytond_currency.egg-info/SOURCES.txt`

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
 currency.py
```

### Comparing `trytond_currency-7.0.0/view/cron_form.xml` & `trytond_currency-7.2.0/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.0.0/view/currency_form.xml` & `trytond_currency-7.2.0/view/currency_form.xml`

 * *Files identical despite different names*

