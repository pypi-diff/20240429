# Comparing `tmp/trytond_account_invoice_correction-7.0.0.tar.gz` & `tmp/trytond_account_invoice_correction-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_correction-7.0.0.tar", last modified: Mon Oct 30 17:20:51 2023, max compression
+gzip compressed data, was "trytond_account_invoice_correction-7.2.0.tar", last modified: Mon Apr 29 15:33:42 2024, max compression
```

## Comparing `trytond_account_invoice_correction-7.0.0.tar` & `trytond_account_invoice_correction-7.2.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:51.282862 trytond_account_invoice_correction-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-22 17:22:51.000000 trytond_account_invoice_correction-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1372 2023-10-30 17:01:55.000000 trytond_account_invoice_correction-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-10-30 17:01:55.000000 trytond_account_invoice_correction-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2795 2023-10-30 17:20:51.282862 trytond_account_invoice_correction-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:51.279529 trytond_account_invoice_correction-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-22 17:22:51.000000 trytond_account_invoice_correction-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:51.000000 trytond_account_invoice_correction-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2776 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.0.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:51.279529 trytond_account_invoice_correction-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      858 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      877 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      908 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      864 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      849 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      896 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      855 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      851 2023-10-30 16:47:45.000000 trytond_account_invoice_correction-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-10-28 12:11:19.000000 trytond_account_invoice_correction-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:20:51.282862 trytond_account_invoice_correction-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4508 2023-10-27 17:38:49.000000 trytond_account_invoice_correction-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:51.279529 trytond_account_invoice_correction-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2096 2023-08-13 15:26:13.000000 trytond_account_invoice_correction-7.0.0/tests/scenario_invoice_correction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_invoice_correction-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:01:52.000000 trytond_account_invoice_correction-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:51.282862 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2795 2023-10-30 17:20:50.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1651 2023-10-30 17:20:51.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:20:50.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:20:50.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:20:50.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:20:50.000000 trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:51.279529 trytond_account_invoice_correction-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.0.0/view/correct_start_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.0.0/view/invoice_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:42.543320 trytond_account_invoice_correction-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1473 2024-04-29 15:14:19.000000 trytond_account_invoice_correction-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2024-04-29 15:14:19.000000 trytond_account_invoice_correction-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-29 15:33:42.543320 trytond_account_invoice_correction-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:42.539987 trytond_account_invoice_correction-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_account_invoice_correction-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:54.000000 trytond_account_invoice_correction-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2776 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1233 2024-04-27 16:30:39.000000 trytond_account_invoice_correction-7.2.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:42.539987 trytond_account_invoice_correction-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      858 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      877 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      752 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      908 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      864 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      849 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      896 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      855 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      846 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      851 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      752 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2024-04-27 16:43:21.000000 trytond_account_invoice_correction-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:42.543320 trytond_account_invoice_correction-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4508 2024-03-17 11:01:36.000000 trytond_account_invoice_correction-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:42.539987 trytond_account_invoice_correction-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2065 2024-04-22 12:14:36.000000 trytond_account_invoice_correction-7.2.0/tests/scenario_invoice_correction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:54.000000 trytond_account_invoice_correction-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:14:14.000000 trytond_account_invoice_correction-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:42.543320 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-29 15:33:42.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1633 2024-04-29 15:33:42.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:42.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:33:42.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:33:42.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:42.000000 trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:42.543320 trytond_account_invoice_correction-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-7.2.0/view/correct_start_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-7.2.0/view/invoice_form.xml
```

### Comparing `trytond_account_invoice_correction-7.0.0/CHANGELOG` & `trytond_account_invoice_correction-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_account_invoice_correction-7.0.0/COPYRIGHT` & `trytond_account_invoice_correction-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2014-2023 Nicolas Évrard.
-Copyright (C) 2014-2023 B2CK SPRL.
-Copyright (C) 2016-2023 Cédric Krier
+Copyright (C) 2014-2024 B2CK SPRL.
+Copyright (C) 2016-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_correction-7.0.0/LICENSE` & `trytond_account_invoice_correction-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/PKG-INFO` & `trytond_account_invoice_correction-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_correction
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to correct invoice
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Invoice Correction Module
 #################################
 
 The account invoice correction module adds a wizard on invoice which allows
 select lines for which the unit price must be corrected.
 A new invoice is created with those lines in double: once with the original
```

### Comparing `trytond_account_invoice_correction-7.0.0/doc/conf.py` & `trytond_account_invoice_correction-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_invoice_correction-7.0.0/invoice.py` & `trytond_account_invoice_correction-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/invoice.xml` & `trytond_account_invoice_correction-7.2.0/invoice.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_account_invoice_correction-7.0.0/invoice.xml` & `trytond_account_invoice_correction-7.2.0/invoice.xml`

```diff
@@ -15,13 +15,13 @@
     </record>
     <record model="ir.action.wizard" id="wizard_invoice_correct">
       <field name="name">Correct</field>
       <field name="wiz_name">account.invoice.correct</field>
       <field name="model">account.invoice</field>
     </record>
     <record model="ir.model.button" id="invoice_correct_button">
+      <field name="model">account.invoice</field>
       <field name="name">correct</field>
       <field name="string">Correct</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_invoice_correction-7.0.0/locale/bg.po` & `trytond_account_invoice_correction-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/ca.po` & `trytond_account_invoice_correction-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/cs.po` & `trytond_account_invoice_correction-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/de.po` & `trytond_account_invoice_correction-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/es.po` & `trytond_account_invoice_correction-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/es_419.po` & `trytond_account_invoice_correction-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/et.po` & `trytond_account_invoice_correction-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/fa.po` & `trytond_account_invoice_correction-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/fi.po` & `trytond_account_invoice_correction-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/fr.po` & `trytond_account_invoice_correction-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/hu.po` & `trytond_account_invoice_correction-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/id.po` & `trytond_account_invoice_correction-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/it.po` & `trytond_account_invoice_correction-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/lo.po` & `trytond_account_invoice_correction-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/lt.po` & `trytond_account_invoice_correction-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/nl.po` & `trytond_account_invoice_correction-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/pl.po` & `trytond_account_invoice_correction-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/pt.po` & `trytond_account_invoice_correction-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/ro.po` & `trytond_account_invoice_correction-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/ru.po` & `trytond_account_invoice_correction-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/sl.po` & `trytond_account_invoice_correction-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/tr.po` & `trytond_account_invoice_correction-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/uk.po` & `trytond_account_invoice_correction-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/locale/zh_CN.po` & `trytond_account_invoice_correction-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/setup.py` & `trytond_account_invoice_correction-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/tests/scenario_invoice_correction.rst` & `trytond_account_invoice_correction-7.2.0/tests/scenario_invoice_correction.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ===========================
 Invoice Correction Scenario
 ===========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice_correction')
 
 Create company::
```

### Comparing `trytond_account_invoice_correction-7.0.0/tox.ini` & `trytond_account_invoice_correction-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/PKG-INFO` & `trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice-correction
-Version: 7.0.0
+Name: trytond_account_invoice_correction
+Version: 7.2.0
 Summary: Tryton module to correct invoice
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Invoice Correction Module
 #################################
 
 The account invoice correction module adds a wizard on invoice which allows
 select lines for which the unit price must be corrected.
 A new invoice is created with those lines in double: once with the original
```

### Comparing `trytond_account_invoice_correction-7.0.0/trytond_account_invoice_correction.egg-info/SOURCES.txt` & `trytond_account_invoice_correction-7.2.0/trytond_account_invoice_correction.egg-info/SOURCES.txt`

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
 invoice.py
```

