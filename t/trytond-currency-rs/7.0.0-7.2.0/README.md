# Comparing `tmp/trytond_currency_rs-7.0.0.tar.gz` & `tmp/trytond_currency_rs-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_currency_rs-7.0.0.tar", last modified: Mon Oct 30 17:29:23 2023, max compression
+gzip compressed data, was "trytond_currency_rs-7.2.0.tar", last modified: Mon Apr 29 15:39:57 2024, max compression
```

## Comparing `trytond_currency_rs-7.0.0.tar` & `trytond_currency_rs-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:23.781973 trytond_currency_rs-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-10-22 17:23:03.000000 trytond_currency_rs-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      627 2023-10-30 17:06:06.000000 trytond_currency_rs-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:06:05.000000 trytond_currency_rs-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2659 2023-10-30 17:29:23.781973 trytond_currency_rs-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3384 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:23.778640 trytond_currency_rs-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2812 2023-10-22 17:23:03.000000 trytond_currency_rs-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:03.000000 trytond_currency_rs-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:23.778640 trytond_currency_rs-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      514 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      501 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-28 12:11:22.000000 trytond_currency_rs-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:29:23.781973 trytond_currency_rs-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4581 2023-10-27 17:38:49.000000 trytond_currency_rs-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:23.778640 trytond_currency_rs-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/tests/scenario_currency_rs.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_currency_rs-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:06:02.000000 trytond_currency_rs-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:23.781973 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2659 2023-10-30 17:29:23.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1530 2023-10-30 17:29:23.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:23.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-10-30 17:29:23.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-10-30 17:29:23.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:29:23.000000 trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:23.778640 trytond_currency_rs-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      573 2023-04-15 07:12:15.000000 trytond_currency_rs-7.0.0/view/cron_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:57.256853 trytond_currency_rs-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:19:21.000000 trytond_currency_rs-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:21.000000 trytond_currency_rs-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2650 2024-04-29 15:39:57.256853 trytond_currency_rs-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3384 2024-03-25 13:26:54.000000 trytond_currency_rs-7.2.0/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1351 2024-04-27 16:30:39.000000 trytond_currency_rs-7.2.0/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:57.253520 trytond_currency_rs-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_currency_rs-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:08.000000 trytond_currency_rs-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:57.253520 trytond_currency_rs-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      514 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:23.000000 trytond_currency_rs-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-27 16:43:24.000000 trytond_currency_rs-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:57.256853 trytond_currency_rs-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4572 2024-04-27 16:30:39.000000 trytond_currency_rs-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:57.253520 trytond_currency_rs-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/tests/scenario_currency_rs.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:08.000000 trytond_currency_rs-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:19:16.000000 trytond_currency_rs-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:57.256853 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2650 2024-04-29 15:39:56.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1512 2024-04-29 15:39:57.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:56.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:39:56.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2024-04-29 15:39:56.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:56.000000 trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:57.256853 trytond_currency_rs-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      573 2023-04-15 07:12:15.000000 trytond_currency_rs-7.2.0/view/cron_form.xml
```

### Comparing `trytond_currency_rs-7.0.0/COPYRIGHT` & `trytond_currency_rs-7.2.0/COPYRIGHT`

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

### Comparing `trytond_currency_rs-7.0.0/LICENSE` & `trytond_currency_rs-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/PKG-INFO` & `trytond_currency_rs-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_currency_rs
-Version: 7.0.0
+Version: 7.2.0
 Summary: Fetch currency rates from the Serbian National Bank
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-currency-rs
+Project-URL: Documentation, https://docs.tryton.org/modules-currency-rs
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton currency serbia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,18 +49,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: zeep
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##################
 Currency RS Module
 ##################
 
 The *Currency RS Module* adds the `Serbian National Bank
 <https://nbs.rs/en/indeks/>`_ as a source for currency exchange rates.
```

### Comparing `trytond_currency_rs-7.0.0/currency.py` & `trytond_currency_rs-7.2.0/currency.py`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/currency.xml` & `trytond_currency_rs-7.2.0/currency.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_currency_rs-7.0.0/currency.xml` & `trytond_currency_rs-7.2.0/currency.xml`

```diff
@@ -5,22 +5,24 @@
   <data>
     <record model="ir.ui.view" id="cron_view_form">
       <field name="model">currency.cron</field>
       <field name="inherit" ref="currency.cron_view_form"/>
       <field name="name">cron_form</field>
     </record>
     <record model="ir.model.field.access" id="access_cron_password">
-      <field name="field" search="[('name', '=', 'rs_password'), ('model.model', '=', 'currency.cron')]"/>
+      <field name="model">currency.cron</field>
+      <field name="field">rs_password</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_cron_password_currency_admin">
-      <field name="field" search="[('name', '=', 'rs_password'), ('model.model', '=', 'currency.cron')]"/>
+      <field name="model">currency.cron</field>
+      <field name="field">rs_password</field>
       <field name="group" ref="currency.group_currency_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_currency_rs-7.0.0/doc/conf.py` & `trytond_currency_rs-7.2.0/doc/conf.py`

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

### Comparing `trytond_currency_rs-7.0.0/locale/ca.po` & `trytond_currency_rs-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/locale/es.po` & `trytond_currency_rs-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/locale/fr.po` & `trytond_currency_rs-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/setup.py` & `trytond_currency_rs-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-currency-rs'),
+            'https://docs.tryton.org/modules-currency-rs'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton currency serbia',
     package_dir={'trytond.modules.currency_rs': '.'},
     packages=(
         ['trytond.modules.currency_rs']
```

### Comparing `trytond_currency_rs-7.0.0/tests/scenario_currency_rs.rst` & `trytond_currency_rs-7.2.0/tests/scenario_currency_rs.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/tox.ini` & `trytond_currency_rs-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/PKG-INFO` & `trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-currency-rs
-Version: 7.0.0
+Name: trytond_currency_rs
+Version: 7.2.0
 Summary: Fetch currency rates from the Serbian National Bank
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-currency-rs
+Project-URL: Documentation, https://docs.tryton.org/modules-currency-rs
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton currency serbia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,18 +49,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: zeep
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##################
 Currency RS Module
 ##################
 
 The *Currency RS Module* adds the `Serbian National Bank
 <https://nbs.rs/en/indeks/>`_ as a source for currency exchange rates.
```

### Comparing `trytond_currency_rs-7.0.0/trytond_currency_rs.egg-info/SOURCES.txt` & `trytond_currency_rs-7.2.0/trytond_currency_rs.egg-info/SOURCES.txt`

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
 currency.py
```

### Comparing `trytond_currency_rs-7.0.0/view/cron_form.xml` & `trytond_currency_rs-7.2.0/view/cron_form.xml`

 * *Files identical despite different names*

