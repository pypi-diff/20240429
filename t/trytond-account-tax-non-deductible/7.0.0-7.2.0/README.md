# Comparing `tmp/trytond_account_tax_non_deductible-7.0.0.tar.gz` & `tmp/trytond_account_tax_non_deductible-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_tax_non_deductible-7.0.0.tar", last modified: Mon Oct 30 17:26:08 2023, max compression
+gzip compressed data, was "trytond_account_tax_non_deductible-7.2.0.tar", last modified: Mon Apr 29 15:37:23 2024, max compression
```

## Comparing `trytond_account_tax_non_deductible-7.0.0.tar` & `trytond_account_tax_non_deductible-7.2.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:08.644376 trytond_account_tax_non_deductible-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-22 17:22:58.000000 trytond_account_tax_non_deductible-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:04:17.000000 trytond_account_tax_non_deductible-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:04:16.000000 trytond_account_tax_non_deductible-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2776 2023-10-30 17:26:08.644376 trytond_account_tax_non_deductible-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      252 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3594 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:08.641042 trytond_account_tax_non_deductible-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-22 17:22:58.000000 trytond_account_tax_non_deductible-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      252 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:58.000000 trytond_account_tax_non_deductible-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:08.641042 trytond_account_tax_non_deductible-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 16:47:45.000000 trytond_account_tax_non_deductible-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-28 12:11:20.000000 trytond_account_tax_non_deductible-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:26:08.644376 trytond_account_tax_non_deductible-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4767 2023-10-27 17:38:49.000000 trytond_account_tax_non_deductible-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:08.641042 trytond_account_tax_non_deductible-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3217 2023-06-10 11:39:56.000000 trytond_account_tax_non_deductible-7.0.0/tests/scenario_account_tax_non_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_tax_non_deductible-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-10-30 17:04:13.000000 trytond_account_tax_non_deductible-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:08.644376 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2776 2023-10-30 17:26:08.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1623 2023-10-30 17:26:08.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:26:08.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:26:08.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-10-30 17:26:08.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:26:08.000000 trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:08.641042 trytond_account_tax_non_deductible-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.0.0/view/tax_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:23.840865 trytond_account_tax_non_deductible-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:17:24.000000 trytond_account_tax_non_deductible-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:17:24.000000 trytond_account_tax_non_deductible-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2767 2024-04-29 15:37:23.840865 trytond_account_tax_non_deductible-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      252 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3594 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:23.837532 trytond_account_tax_non_deductible-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_account_tax_non_deductible-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      252 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:03.000000 trytond_account_tax_non_deductible-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:23.837532 trytond_account_tax_non_deductible-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-27 16:43:22.000000 trytond_account_tax_non_deductible-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:23.840865 trytond_account_tax_non_deductible-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4758 2024-04-27 16:30:39.000000 trytond_account_tax_non_deductible-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:23.837532 trytond_account_tax_non_deductible-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3182 2024-04-22 12:14:36.000000 trytond_account_tax_non_deductible-7.2.0/tests/scenario_account_tax_non_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:03.000000 trytond_account_tax_non_deductible-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-04-29 15:17:19.000000 trytond_account_tax_non_deductible-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:23.837532 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2767 2024-04-29 15:37:23.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1605 2024-04-29 15:37:23.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:23.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:37:23.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2024-04-29 15:37:23.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:23.000000 trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:23.837532 trytond_account_tax_non_deductible-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_tax_non_deductible-7.2.0/view/tax_form.xml
```

### Comparing `trytond_account_tax_non_deductible-7.0.0/COPYRIGHT` & `trytond_account_tax_non_deductible-7.2.0/COPYRIGHT`

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

### Comparing `trytond_account_tax_non_deductible-7.0.0/LICENSE` & `trytond_account_tax_non_deductible-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_non_deductible-7.0.0/PKG-INFO` & `trytond_account_tax_non_deductible-7.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_non_deductible
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to report non-deductible tax
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-tax-non-deductible
+Project-URL: Documentation, https://docs.tryton.org/modules-account-tax-non-deductible
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account tax non-deductible
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #################################
 Account Tax Non-Deductible Module
 #################################
 
 The *Account Tax Non-Deductible Module* allows to define non-deductible taxes
 and reports them.
```

### Comparing `trytond_account_tax_non_deductible-7.0.0/account.py` & `trytond_account_tax_non_deductible-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_non_deductible-7.0.0/account.xml` & `trytond_account_tax_non_deductible-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_non_deductible-7.0.0/doc/conf.py` & `trytond_account_tax_non_deductible-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_tax_non_deductible-7.0.0/setup.py` & `trytond_account_tax_non_deductible-7.2.0/setup.py`

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
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-account-tax-non-deductible'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account tax non-deductible',
     package_dir={'trytond.modules.account_tax_non_deductible': '.'},
     packages=(
```

### Comparing `trytond_account_tax_non_deductible-7.0.0/tests/scenario_account_tax_non_deductible.rst` & `trytond_account_tax_non_deductible-7.2.0/tests/scenario_account_tax_non_deductible.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 ===================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts,
-    ...     create_tax, create_tax_code)
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_tax_non_deductible')
```

### Comparing `trytond_account_tax_non_deductible-7.0.0/tox.ini` & `trytond_account_tax_non_deductible-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/PKG-INFO` & `trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-tax-non-deductible
-Version: 7.0.0
+Name: trytond_account_tax_non_deductible
+Version: 7.2.0
 Summary: Tryton module to report non-deductible tax
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-tax-non-deductible
+Project-URL: Documentation, https://docs.tryton.org/modules-account-tax-non-deductible
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account tax non-deductible
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #################################
 Account Tax Non-Deductible Module
 #################################
 
 The *Account Tax Non-Deductible Module* allows to define non-deductible taxes
 and reports them.
```

### Comparing `trytond_account_tax_non_deductible-7.0.0/trytond_account_tax_non_deductible.egg-info/SOURCES.txt` & `trytond_account_tax_non_deductible-7.2.0/trytond_account_tax_non_deductible.egg-info/SOURCES.txt`

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
 account.py
```

