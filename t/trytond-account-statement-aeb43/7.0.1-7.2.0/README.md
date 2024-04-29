# Comparing `tmp/trytond_account_statement_aeb43-7.0.1.tar.gz` & `tmp/trytond_account_statement_aeb43-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_aeb43-7.0.1.tar", last modified: Sat Feb  3 11:28:02 2024, max compression
+gzip compressed data, was "trytond_account_statement_aeb43-7.2.0.tar", last modified: Mon Apr 29 15:35:48 2024, max compression
```

## Comparing `trytond_account_statement_aeb43-7.0.1.tar` & `trytond_account_statement_aeb43-7.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:28:02.139500 trytond_account_statement_aeb43-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1193 2024-02-03 11:27:59.000000 trytond_account_statement_aeb43-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-02-03 11:27:59.000000 trytond_account_statement_aeb43-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2757 2024-02-03 11:28:02.139500 trytond_account_statement_aeb43-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:28:02.136167 trytond_account_statement_aeb43-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:28:02.139500 trytond_account_statement_aeb43-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1780 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1982 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1801 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:28:02.139500 trytond_account_statement_aeb43-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4525 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3776 2024-01-26 17:56:28.000000 trytond_account_statement_aeb43-7.0.1/statement.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/statement.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:28:02.139500 trytond_account_statement_aeb43-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/tests/n43.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3161 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/tests/scenario_account_statement_aeb43.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_statement_aeb43-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       93 2023-10-30 17:55:12.000000 trytond_account_statement_aeb43-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:28:02.139500 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2757 2024-02-03 11:28:01.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1564 2024-02-03 11:28:02.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:28:01.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-02-03 11:28:01.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:38.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-02-03 11:28:01.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:28:01.000000 trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:48.783352 trytond_account_statement_aeb43-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1409 2024-04-29 15:15:54.000000 trytond_account_statement_aeb43-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-04-29 15:15:54.000000 trytond_account_statement_aeb43-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2788 2024-04-29 15:35:48.783352 trytond_account_statement_aeb43-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:48.780018 trytond_account_statement_aeb43-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:59.000000 trytond_account_statement_aeb43-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:48.783352 trytond_account_statement_aeb43-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1780 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1805 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1982 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1801 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1805 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1785 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:21.000000 trytond_account_statement_aeb43-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:48.783352 trytond_account_statement_aeb43-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4677 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3228 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/statement.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-7.2.0/statement.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:48.783352 trytond_account_statement_aeb43-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-7.2.0/tests/n43.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3221 2024-04-27 16:30:39.000000 trytond_account_statement_aeb43-7.2.0/tests/scenario_account_statement_aeb43.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:59.000000 trytond_account_statement_aeb43-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       93 2024-04-29 15:15:50.000000 trytond_account_statement_aeb43-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:48.783352 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2788 2024-04-29 15:35:48.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2024-04-29 15:35:48.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:48.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:35:48.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-29 15:35:48.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:48.000000 trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/top_level.txt
```

### Comparing `trytond_account_statement_aeb43-7.0.1/CHANGELOG` & `trytond_account_statement_aeb43-7.2.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-02-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
@@ -16,33 +16,41 @@
 * Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
 * Remove support for Python 3.6
 
 Version 6.2.0 - 2021-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.0.0 - 2021-05-03
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Rename aeb43_informations to aeb43_information
 
 Version 5.0.0 - 2018-10-01
+--------------------------
 * Initial release
```

### Comparing `trytond_account_statement_aeb43-7.0.1/COPYRIGHT` & `trytond_account_statement_aeb43-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/LICENSE` & `trytond_account_statement_aeb43-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/PKG-INFO` & `trytond_account_statement_aeb43-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_aeb43
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to import AEB43 statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/
+Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-aeb43
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement AEB 43
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,21 +47,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: python-stdnum
-Requires-Dist: csb43>=0.8
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: aeb43
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
+##############################
 Account Statement AEB43 Module
 ##############################
 
-The Account Statement AEB43 module implements the import of the `Norm 43
+The *Account Statement AEB43 Module* implements the import of the `Norm 43
 <https://downloads.tryton.org/standards/aeb43.pdf>`_ of the Spanish banks
 association file as statement.
+
```

### Comparing `trytond_account_statement_aeb43-7.0.1/doc/conf.py` & `trytond_account_statement_aeb43-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/bg.po` & `trytond_account_statement_aeb43-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/ca.po` & `trytond_account_statement_aeb43-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/cs.po` & `trytond_account_statement_aeb43-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/de.po` & `trytond_account_statement_aeb43-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/es.po` & `trytond_account_statement_aeb43-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/es_419.po` & `trytond_account_statement_aeb43-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/et.po` & `trytond_account_statement_aeb43-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/fa.po` & `trytond_account_statement_aeb43-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/fi.po` & `trytond_account_statement_aeb43-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/fr.po` & `trytond_account_statement_aeb43-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/hu.po` & `trytond_account_statement_aeb43-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/id.po` & `trytond_account_statement_aeb43-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/it.po` & `trytond_account_statement_aeb43-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/lo.po` & `trytond_account_statement_aeb43-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/lt.po` & `trytond_account_statement_aeb43-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/nl.po` & `trytond_account_statement_aeb43-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/pl.po` & `trytond_account_statement_aeb43-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/pt.po` & `trytond_account_statement_aeb43-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/ro.po` & `trytond_account_statement_aeb43-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/ru.po` & `trytond_account_statement_aeb43-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/sl.po` & `trytond_account_statement_aeb43-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/tr.po` & `trytond_account_statement_aeb43-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/uk.po` & `trytond_account_statement_aeb43-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/locale/zh_CN.po` & `trytond_account_statement_aeb43-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/setup.py` & `trytond_account_statement_aeb43-7.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
 def get_require_version(name):
     require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
@@ -37,15 +40,15 @@
 
 if minor_version % 2:
     download_url = ''
 else:
     download_url = 'http://downloads.tryton.org/%s.%s/' % (
         major_version, minor_version)
 
-requires = ['python-stdnum', 'csb43>=0.8']
+requires = ['aeb43']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
@@ -55,15 +58,17 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": (
+            'https://docs.tryton.org/'
+            'modules-account-statement-aeb43'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement AEB 43',
     package_dir={'trytond.modules.account_statement_aeb43': '.'},
     packages=(
         ['trytond.modules.account_statement_aeb43']
```

### Comparing `trytond_account_statement_aeb43-7.0.1/statement.py` & `trytond_account_statement_aeb43-7.2.0/statement.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from io import BytesIO, TextIOWrapper
 
-from csb43 import csb43
-from stdnum.es.ccc import calc_check_digits, to_iban
+from aeb43 import AEB43
 
 from trytond.i18n import gettext
 from trytond.modules.account_statement.exceptions import ImportStatementError
 from trytond.pool import Pool, PoolMeta
 
 
 class ImportStatementStart(metaclass=PoolMeta):
@@ -21,76 +20,65 @@
 
 
 class ImportStatement(metaclass=PoolMeta):
     __name__ = 'account.statement.import'
 
     def parse_aeb43(self, encoding='iso-8859-1'):
         file_ = TextIOWrapper(BytesIO(self.start.file_), encoding=encoding)
-        aeb43 = csb43.File(file_, strict=False)
+        aeb43 = AEB43(file_)
 
         for account in aeb43.accounts:
             statement = self.aeb43_statement(account)
             origins = []
             for transaction in account.transactions:
                 origins.extend(self.aeb43_origin(statement, transaction))
             statement.origins = origins
             yield statement
 
     def aeb43_statement(self, account):
         pool = Pool()
         Statement = pool.get('account.statement')
         Journal = pool.get('account.statement.journal')
 
-        # Compute IBAN code from spanish format
-        bank_code = account.bankCode
-        branch_code = account.branchCode
-        account_number = account.accountNumber
-        check_digits = calc_check_digits(
-            bank_code + branch_code + '00' + account_number)
-        bank_account = to_iban(
-            bank_code + branch_code + check_digits + account_number)
-        journal = Journal.get_by_bank_account(self.start.company, bank_account)
+        journal = Journal.get_by_bank_account(
+            self.start.company, account.ccc, currency=account.currency)
+        if not journal:
+            journal = Journal.get_by_bank_account(
+                self.start.company, account.iban, currency=account.currency)
         if not journal:
             raise ImportStatementError(
                 gettext('account_statement.msg_import_no_journal',
-                    account=bank_account))
+                    account=account.ccc))
 
         statement = Statement()
-        statement.name = '%(account)s@(%(start_date)s/%(end_date)s)' % {
-            'account': bank_account,
-            'start_date': account.initialDate,
-            'end_date': account.finalDate,
+        statement.name = '%(start_date)s - %(end_date)s' % {
+            'start_date': account.start_date,
+            'end_date': account.end_date,
             }
         statement.company = self.start.company
         statement.journal = journal
-        statement.start_balance = account.initialBalance
-        statement.end_balance = account.abstract.balance
-        statement.number_of_lines = (
-            account.abstract.incomeEntries + account.abstract.expenseEntries)
+        statement.date = account.end_date
+        statement.start_balance = account.initial_balance
+        statement.end_balance = account.final_balance
+        statement.number_of_lines = len(account.transactions)
         statement.total_amount = (
-            account.abstract.income - account.abstract.expense)
+            account.final_balance - account.initial_balance)
         return statement
 
     def aeb43_origin(self, statement, transaction):
         pool = Pool()
         Origin = pool.get('account.statement.origin')
         origin = Origin()
-        origin.date = transaction.transactionDate
+        origin.date = transaction.transaction_date
         origin.amount = transaction.amount
-        descriptions = []
-        for item in transaction.optionalItems:
-            if item.item1:
-                descriptions.append(item.item1)
-            if item.item2:
-                descriptions.append(item.item2)
-        origin.description = ''.join(descriptions)
+        origin.description = ''.join(transaction.items)
         origin.information = self.aeb43_information(statement, transaction)
         return [origin]
 
     def aeb43_information(self, statement, transaction):
         return {
-            'aeb43_operation_date': transaction.transactionDate,
-            'aeb43_record_type': transaction.sharedItem,
-            'aeb43_document_number': transaction.documentNumber,
+            'aeb43_operation_date': transaction.transaction_date,
+            'aeb43_record_type': transaction.shared_item,
+            'aeb43_document_number': transaction.document,
             'aeb43_first_reference': transaction.reference1,
             'aeb43_second_reference': transaction.reference2,
             }
```

### Comparing `trytond_account_statement_aeb43-7.0.1/statement.xml` & `trytond_account_statement_aeb43-7.2.0/statement.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/tests/scenario_account_statement_aeb43.rst` & `trytond_account_statement_aeb43-7.2.0/tests/scenario_account_statement_aeb43.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ================================
 Account Statement AEB43 Scenario
 ================================
 
 Imports::
 
-    >>> import datetime
-    >>> from decimal import Decimal
-    >>> from proteus import config, Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual
     >>> from trytond.tools import file_open
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_aeb43')
 
 Create company::
 
-    >>> _ = create_company()
+    >>> eur = get_currency('EUR')
+    >>> eur.numeric_code = '978'
+    >>> eur.save()
+    >>> _ = create_company(currency=eur)
     >>> company = get_company()
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> cash = accounts['cash']
@@ -76,29 +76,28 @@
     >>> waeb43.form.file_ = aeb43
     >>> waeb43.execute('import_')
 
 Check Statement::
 
     >>> Statement = Model.get('account.statement')
     >>> statement, = Statement.find([])
-    >>> statement.journal == journal
-    True
+    >>> assertEqual(statement.journal, journal)
     >>> statement.number_of_lines
     1
     >>> statement.total_amount
     Decimal('-10.98')
     >>> statement.start_balance
     Decimal('3005')
     >>> statement.end_balance
     Decimal('2994.02')
     >>> statement.number_of_lines
     1
     >>> origin, = statement.origins
-    >>> origin.date == datetime.date(2018, 3, 19)
-    True
+    >>> origin.date
+    datetime.date(2018, 3, 19)
     >>> origin.amount
     Decimal('-10.98')
     >>> origin.description
     'COMPRA TARG 5540XXXXXXXX3014 DNH*MICHAEL SCOTT'
     >>> origin.information['aeb43_record_type']
     '12'
     >>> origin.information['aeb43_first_reference']
```

### Comparing `trytond_account_statement_aeb43-7.0.1/tox.ini` & `trytond_account_statement_aeb43-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/PKG-INFO` & `trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_aeb43
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to import AEB43 statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/
+Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-aeb43
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement AEB 43
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,21 +47,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: python-stdnum
-Requires-Dist: csb43>=0.8
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: aeb43
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
+##############################
 Account Statement AEB43 Module
 ##############################
 
-The Account Statement AEB43 module implements the import of the `Norm 43
+The *Account Statement AEB43 Module* implements the import of the `Norm 43
 <https://downloads.tryton.org/standards/aeb43.pdf>`_ of the Spanish banks
 association file as statement.
+
```

### Comparing `trytond_account_statement_aeb43-7.0.1/trytond_account_statement_aeb43.egg-info/SOURCES.txt` & `trytond_account_statement_aeb43-7.2.0/trytond_account_statement_aeb43.egg-info/SOURCES.txt`

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
 setup.py
@@ -41,14 +40,15 @@
 ./tests/__init__.py
 ./tests/n43.txt
 ./tests/scenario_account_statement_aeb43.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 doc/conf.py
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

