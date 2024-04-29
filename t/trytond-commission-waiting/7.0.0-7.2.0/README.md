# Comparing `tmp/trytond_commission_waiting-7.0.0.tar.gz` & `tmp/trytond_commission_waiting-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_commission_waiting-7.0.0.tar", last modified: Mon Oct 30 17:28:40 2023, max compression
+gzip compressed data, was "trytond_commission_waiting-7.2.0.tar", last modified: Mon Apr 29 15:39:15 2024, max compression
```

## Comparing `trytond_commission_waiting-7.0.0.tar` & `trytond_commission_waiting-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:40.431766 trytond_commission_waiting-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:01.000000 trytond_commission_waiting-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-10-30 17:05:38.000000 trytond_commission_waiting-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:05:38.000000 trytond_commission_waiting-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-10-30 17:28:40.431766 trytond_commission_waiting-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3496 2023-08-13 15:26:13.000000 trytond_commission_waiting-7.0.0/commission.py
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.0.0/commission.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:40.428433 trytond_commission_waiting-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:01.000000 trytond_commission_waiting-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:01.000000 trytond_commission_waiting-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2224 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:40.428433 trytond_commission_waiting-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-28 12:11:21.000000 trytond_commission_waiting-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:28:40.431766 trytond_commission_waiting-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4448 2023-10-27 17:38:49.000000 trytond_commission_waiting-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:40.428433 trytond_commission_waiting-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4599 2023-06-10 11:39:56.000000 trytond_commission_waiting-7.0.0/tests/scenario_commission_waiting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_commission_waiting-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2023-10-30 17:05:34.000000 trytond_commission_waiting-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:40.431766 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-10-30 17:28:40.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1635 2023-10-30 17:28:40.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:28:40.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:28:40.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      133 2023-10-30 17:28:40.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:28:40.000000 trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:40.428433 trytond_commission_waiting-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.0.0/view/agent_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.0.0/view/commission_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1709 2024-04-29 15:18:50.000000 trytond_commission_waiting-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:18:50.000000 trytond_commission_waiting-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3496 2024-01-27 09:58:52.000000 trytond_commission_waiting-7.2.0/commission.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.2.0/commission.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:15.291284 trytond_commission_waiting-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_commission_waiting-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:07.000000 trytond_commission_waiting-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2224 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-27 16:43:22.000000 trytond_commission_waiting-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4448 2024-03-17 11:01:36.000000 trytond_commission_waiting-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4576 2024-04-22 12:14:36.000000 trytond_commission_waiting-7.2.0/tests/scenario_commission_waiting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission_waiting-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:07.000000 trytond_commission_waiting-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2024-04-29 15:18:46.000000 trytond_commission_waiting-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-04-29 15:39:14.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1617 2024-04-29 15:39:15.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:14.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:39:14.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      133 2024-04-29 15:39:14.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:14.000000 trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:15.294617 trytond_commission_waiting-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.2.0/view/agent_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:20.000000 trytond_commission_waiting-7.2.0/view/commission_form.xml
```

### Comparing `trytond_commission_waiting-7.0.0/CHANGELOG` & `trytond_commission_waiting-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_commission_waiting-7.0.0/LICENSE` & `trytond_commission_waiting-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-7.0.0/PKG-INFO` & `trytond_commission_waiting-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_commission_waiting
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for commission waiting
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
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_commission<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_commission<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Commission Waiting
 ##################
 
 The commission_waiting module allows to generate account move for each
 commission between the expense/revenue account to a waiting account defined on
 the agent.
```

### Comparing `trytond_commission_waiting-7.0.0/commission.py` & `trytond_commission_waiting-7.2.0/commission.py`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-7.0.0/commission.xml` & `trytond_commission_waiting-7.2.0/commission.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-7.0.0/doc/conf.py` & `trytond_commission_waiting-7.2.0/doc/conf.py`

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

### Comparing `trytond_commission_waiting-7.0.0/invoice.py` & `trytond_commission_waiting-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-7.0.0/setup.py` & `trytond_commission_waiting-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-7.0.0/tests/scenario_commission_waiting.rst` & `trytond_commission_waiting-7.2.0/tests/scenario_commission_waiting.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Commission Scenario
 ===================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('commission_waiting')
```

### Comparing `trytond_commission_waiting-7.0.0/tox.ini` & `trytond_commission_waiting-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/PKG-INFO` & `trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-commission-waiting
-Version: 7.0.0
+Name: trytond_commission_waiting
+Version: 7.2.0
 Summary: Tryton module for commission waiting
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
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_commission<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_commission<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Commission Waiting
 ##################
 
 The commission_waiting module allows to generate account move for each
 commission between the expense/revenue account to a waiting account defined on
 the agent.
```

### Comparing `trytond_commission_waiting-7.0.0/trytond_commission_waiting.egg-info/SOURCES.txt` & `trytond_commission_waiting-7.2.0/trytond_commission_waiting.egg-info/SOURCES.txt`

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
 account.py
```

