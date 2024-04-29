# Comparing `tmp/trytond_account_statement_sepa-7.0.0.tar.gz` & `tmp/trytond_account_statement_sepa-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_sepa-7.0.0.tar", last modified: Mon Oct 30 17:24:53 2023, max compression
+gzip compressed data, was "trytond_account_statement_sepa-7.2.0.tar", last modified: Mon Apr 29 15:36:19 2024, max compression
```

## Comparing `trytond_account_statement_sepa-7.0.0.tar` & `trytond_account_statement_sepa-7.2.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:53.960686 trytond_account_statement_sepa-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:22:56.000000 trytond_account_statement_sepa-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:03:36.000000 trytond_account_statement_sepa-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:03:36.000000 trytond_account_statement_sepa-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2788 2023-10-30 17:24:53.960686 trytond_account_statement_sepa-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9507 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6603 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:53.957353 trytond_account_statement_sepa-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:22:56.000000 trytond_account_statement_sepa-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:56.000000 trytond_account_statement_sepa-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:53.957353 trytond_account_statement_sepa-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3751 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3782 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3775 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3570 2023-10-30 16:47:45.000000 trytond_account_statement_sepa-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-10-28 12:11:20.000000 trytond_account_statement_sepa-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:24:53.960686 trytond_account_statement_sepa-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4698 2023-10-27 17:38:49.000000 trytond_account_statement_sepa-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:53.957353 trytond_account_statement_sepa-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4737 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/tests/camt.053.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/tests/scenario_account_statement_sepa.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_statement_sepa-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2023-10-30 17:03:32.000000 trytond_account_statement_sepa-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:53.960686 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2788 2023-10-30 17:24:53.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1588 2023-10-30 17:24:53.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:24:53.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:24:53.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-10-30 17:24:53.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:24:53.000000 trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:19.015894 trytond_account_statement_sepa-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:16:20.000000 trytond_account_statement_sepa-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:16:19.000000 trytond_account_statement_sepa-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2779 2024-04-29 15:36:19.015894 trytond_account_statement_sepa-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9142 2024-04-27 16:30:39.000000 trytond_account_statement_sepa-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6603 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:19.012561 trytond_account_statement_sepa-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_statement_sepa-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:00.000000 trytond_account_statement_sepa-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:19.015894 trytond_account_statement_sepa-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3751 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3782 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3775 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3570 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2024-04-27 16:43:21.000000 trytond_account_statement_sepa-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:19.015894 trytond_account_statement_sepa-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4689 2024-04-27 16:30:39.000000 trytond_account_statement_sepa-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:19.015894 trytond_account_statement_sepa-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4737 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/tests/camt.053.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3594 2024-04-22 12:14:36.000000 trytond_account_statement_sepa-7.2.0/tests/scenario_account_statement_sepa.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:00.000000 trytond_account_statement_sepa-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:16:15.000000 trytond_account_statement_sepa-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:19.015894 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2779 2024-04-29 15:36:18.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1570 2024-04-29 15:36:18.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:18.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:36:18.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2024-04-29 15:36:18.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:18.000000 trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/top_level.txt
```

### Comparing `trytond_account_statement_sepa-7.0.0/COPYRIGHT` & `trytond_account_statement_sepa-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2015-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 Copyright (C) 2015-2023 Nicolas Évrard
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_account_statement_sepa-7.0.0/LICENSE` & `trytond_account_statement_sepa-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/PKG-INFO` & `trytond_account_statement_sepa-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_sepa
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to import SEPA statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-statement-sepa
+Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-sepa
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement SEPA CAMT.052 CAMT.053 CAMT.054
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #############################
 Account Statement SEPA Module
 #############################
 
 The *Account Statement SEPA Module* implements the import of the CAMT.052,
 CAMT.053 and CAMT.054 `SEPA <https://www.iso20022.org/>`_ files as statement.
```

### Comparing `trytond_account_statement_sepa-7.0.0/account.py` & `trytond_account_statement_sepa-7.2.0/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,21 @@
         Statement = pool.get('account.statement')
         Journal = pool.get('account.statement.journal')
 
         statement = Statement()
         statement.name = camt_statement.findtext('./{*}Id')
         statement.company = self.start.company
         account_number = self.camt_account_number(camt_statement)
+        account_currency = self.camt_account_currency(camt_statement)
         statement.journal = Journal.get_by_bank_account(
-            statement.company, account_number)
+            statement.company, account_number, currency=account_currency)
         if not statement.journal:
             raise ImportStatementError(
                 gettext('account_statement.msg_import_no_journal',
                     account=account_number))
-        account_currency = self.camt_account_currency(camt_statement)
-        if (account_currency
-                and statement.journal.currency.code != account_currency):
-            raise ImportStatementError(
-                gettext('account_statement.msg_import_wrong_currency',
-                    journal=statement.journal.rec_name,
-                    currency=account_currency,
-                    journal_currency=statement.journal.currency.rec_name))
         statement.date = self.camt_statement_date(camt_statement)
         statement.start_balance, statement.end_balance = (
             self.camt_statement_balances(camt_statement))
         statement.total_amount = self.camt_statement_total(camt_statement)
         return statement
 
     def _camt_amount(self, node):
```

### Comparing `trytond_account_statement_sepa-7.0.0/account.xml` & `trytond_account_statement_sepa-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/doc/conf.py` & `trytond_account_statement_sepa-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_statement_sepa-7.0.0/locale/bg.po` & `trytond_account_statement_sepa-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/ca.po` & `trytond_account_statement_sepa-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/cs.po` & `trytond_account_statement_sepa-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/de.po` & `trytond_account_statement_sepa-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/es.po` & `trytond_account_statement_sepa-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/es_419.po` & `trytond_account_statement_sepa-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/et.po` & `trytond_account_statement_sepa-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/fa.po` & `trytond_account_statement_sepa-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/fi.po` & `trytond_account_statement_sepa-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/fr.po` & `trytond_account_statement_sepa-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/hu.po` & `trytond_account_statement_sepa-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/id.po` & `trytond_account_statement_sepa-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/it.po` & `trytond_account_statement_sepa-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/lo.po` & `trytond_account_statement_sepa-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/lt.po` & `trytond_account_statement_sepa-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/nl.po` & `trytond_account_statement_sepa-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/pl.po` & `trytond_account_statement_sepa-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/pt.po` & `trytond_account_statement_sepa-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/ro.po` & `trytond_account_statement_sepa-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/ru.po` & `trytond_account_statement_sepa-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/sl.po` & `trytond_account_statement_sepa-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/tr.po` & `trytond_account_statement_sepa-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/uk.po` & `trytond_account_statement_sepa-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/locale/zh_CN.po` & `trytond_account_statement_sepa-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/setup.py` & `trytond_account_statement_sepa-7.2.0/setup.py`

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
-            'https://docs.tryton.org/projects/modules-account-statement-sepa'),
+            'https://docs.tryton.org/modules-account-statement-sepa'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement SEPA CAMT.052 CAMT.053 CAMT.054',
     package_dir={'trytond.modules.account_statement_sepa': '.'},
     packages=(
         ['trytond.modules.account_statement_sepa']
```

### Comparing `trytond_account_statement_sepa-7.0.0/tests/camt.053.001.02.xml` & `trytond_account_statement_sepa-7.2.0/tests/camt.053.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/tests/scenario_account_statement_sepa.rst` & `trytond_account_statement_sepa-7.2.0/tests/scenario_account_statement_sepa.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ===============================
 Account Statement Sepa Scenario
 ===============================
 
 Imports::
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.tools import file_open
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+    >>> from trytond.tools import file_open
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_sepa')
 
     >>> AccountJournal = Model.get('account.journal')
     >>> Bank = Model.get('bank')
@@ -71,15 +69,16 @@
     ...     bank_account=bank_account,
     ...     )
     >>> journal.save()
 
 Import CAMT.053 file::
 
     >>> statement_import = Wizard('account.statement.import')
-    >>> with file_open('account_statement_sepa/tests/camt.053.001.02.xml', mode='rb') as fp:
+    >>> with file_open(
+    ...         'account_statement_sepa/tests/camt.053.001.02.xml', mode='rb') as fp:
     ...     camt = fp.read()
     >>> statement_import.form.file_ = camt
     >>> statement_import.form.file_format = 'camt_053_001'
     >>> statement_import.execute('import_')
 
 Check Statement::
 
@@ -100,16 +99,15 @@
     1
     >>> origin, = statement.origins
     >>> origin.number
     >>> origin.date
     datetime.date(2009, 4, 29)
     >>> origin.amount
     Decimal('-100.00')
-    >>> origin.party == supplier
-    True
+    >>> assertEqual(origin.party, supplier)
     >>> origin.description
     >>> origin.information['camt_creditor_name']
     'Supplier'
     >>> origin.information['camt_creditor_iban']
     'DE79370400440123619900'
     >>> origin.information['camt_remittance_information']
     'INV 2150135'
```

### Comparing `trytond_account_statement_sepa-7.0.0/tox.ini` & `trytond_account_statement_sepa-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/PKG-INFO` & `trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-statement-sepa
-Version: 7.0.0
+Name: trytond_account_statement_sepa
+Version: 7.2.0
 Summary: Tryton module to import SEPA statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-statement-sepa
+Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-sepa
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement SEPA CAMT.052 CAMT.053 CAMT.054
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #############################
 Account Statement SEPA Module
 #############################
 
 The *Account Statement SEPA Module* implements the import of the CAMT.052,
 CAMT.053 and CAMT.054 `SEPA <https://www.iso20022.org/>`_ files as statement.
```

### Comparing `trytond_account_statement_sepa-7.0.0/trytond_account_statement_sepa.egg-info/SOURCES.txt` & `trytond_account_statement_sepa-7.2.0/trytond_account_statement_sepa.egg-info/SOURCES.txt`

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

