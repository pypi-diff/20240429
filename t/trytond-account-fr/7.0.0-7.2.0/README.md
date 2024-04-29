# Comparing `tmp/trytond_account_fr-7.0.0.tar.gz` & `tmp/trytond_account_fr-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_fr-7.0.0.tar", last modified: Mon Oct 30 17:20:19 2023, max compression
+gzip compressed data, was "trytond_account_fr-7.2.0.tar", last modified: Mon Apr 29 15:33:20 2024, max compression
```

## Comparing `trytond_account_fr-7.0.0.tar` & `trytond_account_fr-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:19.469377 trytond_account_fr-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-22 17:22:50.000000 trytond_account_fr-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2023-10-30 17:01:44.000000 trytond_account_fr-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-10-30 17:01:43.000000 trytond_account_fr-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_fr-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3170 2023-10-30 17:20:19.469377 trytond_account_fr-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-08-13 15:26:13.000000 trytond_account_fr-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11771 2023-08-13 15:26:13.000000 trytond_account_fr-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   436146 2023-10-07 15:40:36.000000 trytond_account_fr-7.0.0/account_fr.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:19.466044 trytond_account_fr-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-22 17:22:50.000000 trytond_account_fr-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:50.000000 trytond_account_fr-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:19.466044 trytond_account_fr-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1473 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1435 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1377 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1435 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1328 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1242 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1403 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1286 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1339 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1324 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1385 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1334 2023-10-30 16:47:45.000000 trytond_account_fr-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1296 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1203 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1314 2023-10-28 12:11:19.000000 trytond_account_fr-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:20:19.469377 trytond_account_fr-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4428 2023-10-27 17:38:49.000000 trytond_account_fr-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   194518 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/tax_fr.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:19.466044 trytond_account_fr-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/tests/FEC-previous.csv
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/tests/FEC.csv
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6924 2023-06-10 11:39:56.000000 trytond_account_fr-7.0.0/tests/scenario_fec.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_fr-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2481 2023-06-10 11:39:56.000000 trytond_account_fr-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_fr-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:01:40.000000 trytond_account_fr-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:19.469377 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3170 2023-10-30 17:20:19.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1663 2023-10-30 17:20:19.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:20:19.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-10-30 17:20:19.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      100 2023-10-30 17:20:19.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:20:19.000000 trytond_account_fr-7.0.0/trytond_account_fr.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:19.466044 trytond_account_fr-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_account_fr-7.0.0/view/fec_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:20.000000 trytond_account_fr-7.0.0/view/fec_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2959 2024-04-29 15:14:02.000000 trytond_account_fr-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      811 2024-04-29 15:14:02.000000 trytond_account_fr-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_fr-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3170 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-01-27 09:58:52.000000 trytond_account_fr-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11771 2024-01-27 09:58:52.000000 trytond_account_fr-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   436146 2024-01-27 09:58:52.000000 trytond_account_fr-7.2.0/account_fr.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:20.017243 trytond_account_fr-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_account_fr-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:54.000000 trytond_account_fr-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1269 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1473 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1435 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1269 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1377 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1269 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1435 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1328 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1242 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1403 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1286 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1339 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1324 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1385 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1334 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1296 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1203 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1314 2024-04-27 16:43:20.000000 trytond_account_fr-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4428 2024-03-17 11:01:36.000000 trytond_account_fr-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   194518 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/tax_fr.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/tests/FEC-previous.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/tests/FEC.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6906 2024-04-22 12:14:36.000000 trytond_account_fr-7.2.0/tests/scenario_fec.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_fr-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2481 2024-01-27 09:58:52.000000 trytond_account_fr-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:54.000000 trytond_account_fr-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-29 15:13:56.000000 trytond_account_fr-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3170 2024-04-29 15:33:19.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1645 2024-04-29 15:33:19.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:19.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:33:19.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      100 2024-04-29 15:33:19.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:19.000000 trytond_account_fr-7.2.0/trytond_account_fr.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:20.020576 trytond_account_fr-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_account_fr-7.2.0/view/fec_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:20.000000 trytond_account_fr-7.2.0/view/fec_start_form.xml
```

### Comparing `trytond_account_fr-7.0.0/CHANGELOG` & `trytond_account_fr-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_fr-7.0.0/COPYRIGHT` & `trytond_account_fr-7.2.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2010-2023 Cédric Krier.
+Copyright (C) 2010-2024 Cédric Krier.
 Copyright (C) 2010-2011 Bertrand Chenal.
 Copyright (C) 2010-2023 Nicolas Évrard.
-Copyright (C) 2010-2023 B2CK SPRL.
+Copyright (C) 2010-2024 B2CK SPRL.
 Copyright (C) 2014-2018 Raphaël Hertzog.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_account_fr-7.0.0/LICENSE` & `trytond_account_fr-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/PKG-INFO` & `trytond_account_fr-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_fr
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with French chart of accounts
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
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_party_siret<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_party_siret<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 French Account Module
 #####################
 
 The French account module defines the standard chart of account
 
 A wizard allows to generate the FEC file for a fiscal year.
```

### Comparing `trytond_account_fr-7.0.0/README.rst` & `trytond_account_fr-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/account.py` & `trytond_account_fr-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/account.xml` & `trytond_account_fr-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/account_fr.xml` & `trytond_account_fr-7.2.0/account_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/doc/conf.py` & `trytond_account_fr-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_account_fr-7.0.0/doc/index.rst` & `trytond_account_fr-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/bg.po` & `trytond_account_fr-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/ca.po` & `trytond_account_fr-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/cs.po` & `trytond_account_fr-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/de.po` & `trytond_account_fr-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/es.po` & `trytond_account_fr-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/es_419.po` & `trytond_account_fr-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/et.po` & `trytond_account_fr-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/fa.po` & `trytond_account_fr-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/fi.po` & `trytond_account_fr-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/fr.po` & `trytond_account_fr-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/hu.po` & `trytond_account_fr-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/id.po` & `trytond_account_fr-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/it.po` & `trytond_account_fr-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/lo.po` & `trytond_account_fr-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/lt.po` & `trytond_account_fr-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/nl.po` & `trytond_account_fr-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/pl.po` & `trytond_account_fr-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/pt.po` & `trytond_account_fr-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/ro.po` & `trytond_account_fr-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/ru.po` & `trytond_account_fr-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/sl.po` & `trytond_account_fr-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/tr.po` & `trytond_account_fr-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/uk.po` & `trytond_account_fr-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/locale/zh_CN.po` & `trytond_account_fr-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/setup.py` & `trytond_account_fr-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/tax_fr.xml` & `trytond_account_fr-7.2.0/tax_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/tests/FEC.csv` & `trytond_account_fr-7.2.0/tests/FEC.csv`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/tests/scenario_fec.rst` & `trytond_account_fr-7.2.0/tests/scenario_fec.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ============
 FEC Scenario
 ============
 
 Imports::
 
     >>> import datetime as dt
-    >>> import os
     >>> import io
+    >>> import os
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
-    >>> from trytond.modules.account_fr.tests.tools import create_chart, \
-    ...     get_accounts
+    >>> from trytond.modules.account_fr.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account_fr')
 
 Create company::
 
@@ -145,16 +144,16 @@
     ...         'post_date': period.start_date,
     ...         'post_number': '3',
     ...         }, config.context)
     >>> move.click('post')
     >>> reconcile2, = [l for l in move.lines if l.account == receivable]
     >>> reconcile_lines = Wizard('account.move.reconcile_lines',
     ...     [reconcile1, reconcile2])
-    >>> reconcile_lines.state == 'end'
-    True
+    >>> reconcile_lines.state
+    'end'
     >>> reconcile_date = reconcile1.reconciliation.create_date
 
 Balance non-deferral::
 
     >>> Sequence = Model.get('ir.sequence')
     >>> Period = Model.get('account.period')
     >>> Account = Model.get('account.account')
@@ -196,19 +195,17 @@
     >>> file = os.path.join(os.path.dirname(__file__), 'FEC.csv')
     >>> with io.open(file, mode='rb') as fp:
     ...     template = fp.read().decode('utf-8')
     >>> current_date = reconcile_date.strftime('%Y%m%d')
     >>> template = template.format(
     ...         current_date=current_date,
     ...         )
-    >>> FEC.form.file.decode('utf-8') == template
-    True
+    >>> assertEqual(FEC.form.file.decode('utf-8'), template)
 
 Generate FEC for previous fiscal year::
 
     >>> FEC = Wizard('account.fr.fec')
     >>> FEC.form.fiscalyear = fiscalyear_previous
     >>> FEC.execute('generate')
     >>> file = os.path.join(os.path.dirname(__file__), 'FEC-previous.csv')
     >>> with io.open(file, mode='rb') as fp:
-    ...     FEC.form.file.decode('utf-8') == fp.read().decode('utf-8')
-    True
+    ...     assertEqual(FEC.form.file.decode('utf-8'), fp.read().decode('utf-8'))
```

### Comparing `trytond_account_fr-7.0.0/tests/test_module.py` & `trytond_account_fr-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/tests/tools.py` & `trytond_account_fr-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/tox.ini` & `trytond_account_fr-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-7.0.0/trytond_account_fr.egg-info/PKG-INFO` & `trytond_account_fr-7.2.0/trytond_account_fr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-fr
-Version: 7.0.0
+Name: trytond_account_fr
+Version: 7.2.0
 Summary: Tryton module with French chart of accounts
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
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_party_siret<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_party_siret<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 French Account Module
 #####################
 
 The French account module defines the standard chart of account
 
 A wizard allows to generate the FEC file for a fiscal year.
```

### Comparing `trytond_account_fr-7.0.0/trytond_account_fr.egg-info/SOURCES.txt` & `trytond_account_fr-7.2.0/trytond_account_fr.egg-info/SOURCES.txt`

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
 account.py
```

