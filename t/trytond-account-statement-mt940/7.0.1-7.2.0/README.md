# Comparing `tmp/trytond_account_statement_mt940-7.0.1.tar.gz` & `tmp/trytond_account_statement_mt940-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_mt940-7.0.1.tar", last modified: Wed Apr 17 10:41:15 2024, max compression
+gzip compressed data, was "trytond_account_statement_mt940-7.2.0.tar", last modified: Mon Apr 29 15:36:01 2024, max compression
```

## Comparing `trytond_account_statement_mt940-7.0.1.tar` & `trytond_account_statement_mt940-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-17 10:41:12.000000 trytond_account_statement_mt940-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-17 10:41:12.000000 trytond_account_statement_mt940-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5441 2024-04-12 22:34:01.000000 trytond_account_statement_mt940-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.104597 trytond_account_statement_mt940-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2802 2024-03-03 16:24:20.000000 trytond_account_statement_mt940-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.104597 trytond_account_statement_mt940-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/icons/LICENSE
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.104597 trytond_account_statement_mt940-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      967 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      973 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      980 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      967 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4749 2024-03-03 16:24:03.000000 trytond_account_statement_mt940-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/MT940.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3486 2024-02-05 16:24:27.000000 trytond_account_statement_mt940-7.0.1/tests/scenario_account_statement_mt940.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-02-05 16:24:27.000000 trytond_account_statement_mt940-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1649 2024-04-17 10:41:15.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:38.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:41:14.000000 trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:41:15.107930 trytond_account_statement_mt940-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_account_statement_mt940-7.0.1/view/statement_import_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.236359 trytond_account_statement_mt940-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-29 15:16:04.000000 trytond_account_statement_mt940-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:16:04.000000 trytond_account_statement_mt940-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-29 15:36:01.236359 trytond_account_statement_mt940-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5066 2024-04-27 16:30:39.000000 trytond_account_statement_mt940-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.233026 trytond_account_statement_mt940-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_account_statement_mt940-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:59.000000 trytond_account_statement_mt940-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.233026 trytond_account_statement_mt940-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/icons/LICENSE
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.233026 trytond_account_statement_mt940-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      972 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      967 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      973 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      980 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      967 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-27 16:43:21.000000 trytond_account_statement_mt940-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:01.236359 trytond_account_statement_mt940-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4749 2024-04-27 16:30:39.000000 trytond_account_statement_mt940-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.233026 trytond_account_statement_mt940-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/tests/MT940.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3471 2024-04-22 12:14:36.000000 trytond_account_statement_mt940-7.2.0/tests/scenario_account_statement_mt940.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:59.000000 trytond_account_statement_mt940-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:16:00.000000 trytond_account_statement_mt940-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.236359 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-04-29 15:36:00.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1649 2024-04-29 15:36:01.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:00.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:36:00.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:55:54.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-29 15:36:00.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:00.000000 trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:01.236359 trytond_account_statement_mt940-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-01-27 09:58:52.000000 trytond_account_statement_mt940-7.2.0/view/statement_import_start_form.xml
```

### Comparing `trytond_account_statement_mt940-7.0.1/COPYRIGHT` & `trytond_account_statement_mt940-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/LICENSE` & `trytond_account_statement_mt940-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/PKG-INFO` & `trytond_account_statement_mt940-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_mt940
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to import MT940 statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-mt940
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -49,19 +49,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: mt940
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##############################
 Account Statement MT940 Module
 ##############################
 
 The *Account Statement MT940 Module* implements the import of `MT940
 <https://en.wikipedia.org/wiki/MT940>`_ files as statements.
```

### Comparing `trytond_account_statement_mt940-7.0.1/__init__.py` & `trytond_account_statement_mt940-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/account.py` & `trytond_account_statement_mt940-7.2.0/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,42 +51,38 @@
         pool = Pool()
         Statement = pool.get('account.statement')
         Journal = pool.get('account.statement.journal')
 
         statement = Statement()
         statement.name = mt940_statement.information
         statement.company = self.start.company
+        account, currency = (
+            self.mt940_statement_account_currency(mt940_statement))
+        start_balance = mt940_statement.start_balance
+        end_balance = mt940_statement.end_balance
         statement.journal = Journal.get_by_bank_account(
-            statement.company, mt940_statement.account)
+            statement.company, account,
+            currency=currency or start_balance.currency)
         if not statement.journal:
             raise ImportStatementError(
                 gettext('account_statement.msg_import_no_journal',
                     account=mt940_statement.account))
-        start_balance = mt940_statement.start_balance
-        end_balance = mt940_statement.end_balance
-        if statement.journal.currency.code != start_balance.currency:
-            raise ImportStatementError(
-                gettext('account_statement.msg_import_wrong_currency',
-                    journal=statement.journal.rec_name,
-                    currency=start_balance.currency,
-                    journal_currency=statement.journal.currency.rec_name))
-        if statement.journal.currency.code != end_balance.currency:
-            raise ImportStatementError(
-                gettext('account_statement.msg_import_wrong_currency',
-                    journal=statement.journal.rec_name,
-                    currency=end_balance.currency,
-                    journal_currency=statement.journal.currency.rec_name))
         statement.date = end_balance.date
         statement.start_balance = start_balance.amount
         statement.end_balance = end_balance.amount
         statement.total_amount = (
             end_balance.amount - start_balance.amount)
         statement.number_of_lines = len(mt940_statement.transactions)
         return statement
 
+    def mt940_statement_account_currency(self, mt940_statement):
+        if self.start.mt940_bank == 'rabo':
+            return mt940_statement.account.split(' ', 1)
+        return mt940_statement.account, None
+
     def mt940_origin(self, mt940_statement, transaction):
         pool = Pool()
         Origin = pool.get('account.statement.origin')
 
         origin = Origin()
         origin.number = transaction.id
         origin.date = transaction.date
```

### Comparing `trytond_account_statement_mt940-7.0.1/account.xml` & `trytond_account_statement_mt940-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/doc/conf.py` & `trytond_account_statement_mt940-7.2.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
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

### Comparing `trytond_account_statement_mt940-7.0.1/icons/LICENSE` & `trytond_account_statement_mt940-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/bg.po` & `trytond_account_statement_mt940-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/ca.po` & `trytond_account_statement_mt940-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/cs.po` & `trytond_account_statement_mt940-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/de.po` & `trytond_account_statement_mt940-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/es.po` & `trytond_account_statement_mt940-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/es_419.po` & `trytond_account_statement_mt940-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/et.po` & `trytond_account_statement_mt940-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/fa.po` & `trytond_account_statement_mt940-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/fi.po` & `trytond_account_statement_mt940-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/fr.po` & `trytond_account_statement_mt940-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/hu.po` & `trytond_account_statement_mt940-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/id.po` & `trytond_account_statement_mt940-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/it.po` & `trytond_account_statement_mt940-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/lo.po` & `trytond_account_statement_mt940-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/lt.po` & `trytond_account_statement_mt940-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/nl.po` & `trytond_account_statement_mt940-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/pl.po` & `trytond_account_statement_mt940-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/pt.po` & `trytond_account_statement_mt940-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/ro.po` & `trytond_account_statement_mt940-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/ru.po` & `trytond_account_statement_mt940-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/sl.po` & `trytond_account_statement_mt940-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/tr.po` & `trytond_account_statement_mt940-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/uk.po` & `trytond_account_statement_mt940-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/locale/zh_CN.po` & `trytond_account_statement_mt940-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/setup.py` & `trytond_account_statement_mt940-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/tests/scenario_account_statement_mt940.rst` & `trytond_account_statement_mt940-7.2.0/tests/scenario_account_statement_mt940.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ================================
 Account Statement MT940 Scenario
 ================================
 
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
 
     >>> config = activate_modules('account_statement_mt940')
 
     >>> AccountJournal = Model.get('account.journal')
     >>> Bank = Model.get('bank')
@@ -106,13 +104,12 @@
     >>> origin, = statement.origins
     >>> origin.number
     'FFPC'
     >>> origin.date
     datetime.date(2019, 7, 31)
     >>> origin.amount
     Decimal('100.00')
-    >>> origin.party == customer
-    True
+    >>> assertEqual(origin.party, customer)
     >>> origin.description
     '98.76.54.321 John Doe'
     >>> origin.information['mt940_reference']
     '913000381'
```

### Comparing `trytond_account_statement_mt940-7.0.1/tox.ini` & `trytond_account_statement_mt940-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/PKG-INFO` & `trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_mt940
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to import MT940 statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-statement-mt940
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -49,19 +49,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: mt940
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##############################
 Account Statement MT940 Module
 ##############################
 
 The *Account Statement MT940 Module* implements the import of `MT940
 <https://en.wikipedia.org/wiki/MT940>`_ files as statements.
```

### Comparing `trytond_account_statement_mt940-7.0.1/trytond_account_statement_mt940.egg-info/SOURCES.txt` & `trytond_account_statement_mt940-7.2.0/trytond_account_statement_mt940.egg-info/SOURCES.txt`

 * *Files identical despite different names*

