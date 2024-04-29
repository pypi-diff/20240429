# Comparing `tmp/trytond_account_statement_coda-7.0.0.tar.gz` & `tmp/trytond_account_statement_coda-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_coda-7.0.0.tar", last modified: Mon Oct 30 17:24:25 2023, max compression
+gzip compressed data, was "trytond_account_statement_coda-7.2.0.tar", last modified: Mon Apr 29 15:35:55 2024, max compression
```

## Comparing `trytond_account_statement_coda-7.0.0.tar` & `trytond_account_statement_coda-7.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:25.820552 trytond_account_statement_coda-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:22:55.000000 trytond_account_statement_coda-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1268 2023-10-30 17:03:18.000000 trytond_account_statement_coda-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:03:18.000000 trytond_account_statement_coda-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement_coda-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2607 2023-10-30 17:24:25.820552 trytond_account_statement_coda-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-10-27 17:38:49.000000 trytond_account_statement_coda-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4266 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4149 2023-01-16 14:00:20.000000 trytond_account_statement_coda-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:25.817218 trytond_account_statement_coda-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:22:55.000000 trytond_account_statement_coda-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-10-27 17:38:49.000000 trytond_account_statement_coda-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:55.000000 trytond_account_statement_coda-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:25.817218 trytond_account_statement_coda-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2183 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2255 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2216 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1865 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2030 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2380 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2271 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1865 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2223 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2328 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2223 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2331 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1865 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1865 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-28 12:11:20.000000 trytond_account_statement_coda-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:24:25.820552 trytond_account_statement_coda-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4421 2023-10-27 17:38:49.000000 trytond_account_statement_coda-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:25.817218 trytond_account_statement_coda-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-01-16 14:00:20.000000 trytond_account_statement_coda-7.0.0/tests/CODA.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3032 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/tests/scenario_account_statement_coda.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_statement_coda-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2023-10-30 17:03:15.000000 trytond_account_statement_coda-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:25.817218 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2607 2023-10-30 17:24:25.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-30 17:24:25.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:24:25.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:24:25.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      117 2023-10-30 17:24:25.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:24:25.000000 trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:55.336514 trytond_account_statement_coda-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1369 2024-04-29 15:15:59.000000 trytond_account_statement_coda-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:59.000000 trytond_account_statement_coda-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement_coda-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-04-29 15:35:55.336514 trytond_account_statement_coda-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2024-02-04 18:51:26.000000 trytond_account_statement_coda-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3937 2024-04-27 16:30:39.000000 trytond_account_statement_coda-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4149 2023-01-16 14:00:20.000000 trytond_account_statement_coda-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:55.333181 trytond_account_statement_coda-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_statement_coda-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2024-02-04 18:51:26.000000 trytond_account_statement_coda-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:59.000000 trytond_account_statement_coda-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:55.333181 trytond_account_statement_coda-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2183 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2255 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2216 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1865 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2030 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2380 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2271 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1865 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2328 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2331 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2024-04-29 13:17:17.000000 trytond_account_statement_coda-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1865 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-27 16:43:21.000000 trytond_account_statement_coda-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:55.336514 trytond_account_statement_coda-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4421 2024-03-17 11:01:36.000000 trytond_account_statement_coda-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:55.333181 trytond_account_statement_coda-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-01-16 14:00:20.000000 trytond_account_statement_coda-7.2.0/tests/CODA.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-22 12:14:36.000000 trytond_account_statement_coda-7.2.0/tests/scenario_account_statement_coda.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_coda-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:59.000000 trytond_account_statement_coda-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:15:55.000000 trytond_account_statement_coda-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:55.336514 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-04-29 15:35:54.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1531 2024-04-29 15:35:55.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:54.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:35:54.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      117 2024-04-29 15:35:54.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:54.000000 trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/top_level.txt
```

### Comparing `trytond_account_statement_coda-7.0.0/CHANGELOG` & `trytond_account_statement_coda-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_statement_coda-7.0.0/COPYRIGHT` & `trytond_account_statement_coda-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2023 Cédric Krier
-Copyright (C) 2017-2023 B2CK
+Copyright (C) 2017-2024 Cédric Krier
+Copyright (C) 2017-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_statement_coda-7.0.0/LICENSE` & `trytond_account_statement_coda-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/PKG-INFO` & `trytond_account_statement_coda-7.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_coda
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to import CODA statements
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
@@ -46,18 +46,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: febelfin-coda
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Statement Coda Module
 #############################
 
 The Account Statement Coda module implements the import of the `CODA
 <http://downloads.tryton.org/standards/coda-2.6.pdf>`_ file as statement.
```

### Comparing `trytond_account_statement_coda-7.0.0/__init__.py` & `trytond_account_statement_coda-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/account.py` & `trytond_account_statement_coda-7.2.0/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,25 +37,20 @@
         Statement = pool.get('account.statement')
         Journal = pool.get('account.statement.journal')
 
         statement = Statement()
         statement.name = coda_statement.new_sequence
         statement.company = self.start.company
         statement.journal = Journal.get_by_bank_account(
-            statement.company, coda_statement.account)
+            statement.company, coda_statement.account,
+            currency=coda_statement.account_currency)
         if not statement.journal:
             raise ImportStatementError(
                 gettext('account_statement.msg_import_no_journal',
                     account=coda_statement.account))
-        if statement.journal.currency.code != coda_statement.account_currency:
-            raise ImportStatementError(
-                gettext('account_statement.msg_import_wrong_currency',
-                    journal=statement.journal.rec_name,
-                    currency=coda_statement.account_currency,
-                    journal_currency=statement.journal.currency.rec_name))
         statement.date = coda_statement.creation_date
         statement.start_balance = coda_statement.old_balance
         statement.end_balance = coda_statement.new_balance
         statement.total_amount = (
             coda_statement.total_credit - coda_statement.total_debit)
         statement.number_of_lines = len(coda_statement.moves)
         return statement
```

### Comparing `trytond_account_statement_coda-7.0.0/account.xml` & `trytond_account_statement_coda-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/doc/conf.py` & `trytond_account_statement_coda-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_statement_coda-7.0.0/locale/bg.po` & `trytond_account_statement_coda-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/ca.po` & `trytond_account_statement_coda-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/cs.po` & `trytond_account_statement_coda-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/de.po` & `trytond_account_statement_coda-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/es.po` & `trytond_account_statement_coda-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/es_419.po` & `trytond_account_statement_coda-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/et.po` & `trytond_account_statement_coda-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/fa.po` & `trytond_account_statement_coda-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/fi.po` & `trytond_account_statement_coda-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/fr.po` & `trytond_account_statement_coda-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/hu.po` & `trytond_account_statement_coda-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/id.po` & `trytond_account_statement_coda-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/it.po` & `trytond_account_statement_coda-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/lo.po` & `trytond_account_statement_coda-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/lt.po` & `trytond_account_statement_coda-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/nl.po` & `trytond_account_statement_coda-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/pl.po` & `trytond_account_statement_coda-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/pt.po` & `trytond_account_statement_coda-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/ro.po` & `trytond_account_statement_coda-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/ru.po` & `trytond_account_statement_coda-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/sl.po` & `trytond_account_statement_coda-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/tr.po` & `trytond_account_statement_coda-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/locale/uk.po` & `trytond_account_statement_coda-7.2.0/locale/ro.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,86 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt ""
 "model:account.statement.origin.information,selection:information_r_transaction"
 msgid ""
 "0: Paid\n"
 "                1: Reject\n"
 "                2: Return\n"
 "                3: Refund\n"
 "                4: Reversal\n"
 "                5: Cancellation"
 msgstr ""
+"0: Platit\n"
+"                1: Respingere\n"
+"                2: Returnare\n"
+"                3: Restituire\n"
+"                4: Inversare\n"
+"                5: Anulare"
 
+#, fuzzy
 msgctxt ""
 "model:account.statement.origin.information,string:information_bank_reference"
 msgid "Bank Reference"
-msgstr ""
+msgstr "Referinta Bancara"
 
+#, fuzzy
 msgctxt ""
 "model:account.statement.origin.information,string:information_category_purpose"
 msgid "Category Purpose"
-msgstr ""
+msgstr "Scop Categorie"
 
+#, fuzzy
 msgctxt ""
 "model:account.statement.origin.information,string:information_counterparty_account"
 msgid "Counterparty Account"
-msgstr ""
+msgstr "Cont de Contraparte"
 
+#, fuzzy
 msgctxt ""
 "model:account.statement.origin.information,string:information_counterparty_bic"
 msgid "Counterparty BIC"
-msgstr ""
+msgstr "BIC Contraparte"
 
+#, fuzzy
 msgctxt ""
 "model:account.statement.origin.information,string:information_counterparty_name"
 msgid "Counterparty Name"
-msgstr ""
+msgstr "Nume Contraparte"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_customer_reference"
 msgid "Customer Reference"
-msgstr ""
+msgstr "Referinta Client"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_purpose"
 msgid "Purpose"
-msgstr ""
+msgstr "Scop"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_r_reason"
 msgid "Return Reason"
-msgstr ""
+msgstr "Motiv Retur"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_r_transaction"
 msgid "Return Type"
-msgstr ""
+msgstr "Tip Retur"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_transaction_category"
 msgid "Transaction Category"
-msgstr ""
+msgstr "Categorie Tranzactie"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_transaction_family"
 msgid "Transaction Family"
-msgstr ""
+msgstr "Familie Tranzactie"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_transaction_transaction"
 msgid "Transaction"
-msgstr ""
+msgstr "Tranzactie"
```

### Comparing `trytond_account_statement_coda-7.0.0/locale/zh_CN.po` & `trytond_account_statement_coda-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/setup.py` & `trytond_account_statement_coda-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/tests/CODA.txt` & `trytond_account_statement_coda-7.2.0/tests/CODA.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/tests/scenario_account_statement_coda.rst` & `trytond_account_statement_coda-7.2.0/tests/scenario_account_statement_coda.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ===============================
 Account Statement Coda Scenario
 ===============================
 
 Imports::
 
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.tools import file_open
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_coda')
 
 Create company::
```

### Comparing `trytond_account_statement_coda-7.0.0/tox.ini` & `trytond_account_statement_coda-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/PKG-INFO` & `trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-statement-coda
-Version: 7.0.0
+Name: trytond_account_statement_coda
+Version: 7.2.0
 Summary: Tryton module to import CODA statements
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
@@ -46,18 +46,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: febelfin-coda
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Statement Coda Module
 #############################
 
 The Account Statement Coda module implements the import of the `CODA
 <http://downloads.tryton.org/standards/coda-2.6.pdf>`_ file as statement.
```

### Comparing `trytond_account_statement_coda-7.0.0/trytond_account_statement_coda.egg-info/SOURCES.txt` & `trytond_account_statement_coda-7.2.0/trytond_account_statement_coda.egg-info/SOURCES.txt`

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

