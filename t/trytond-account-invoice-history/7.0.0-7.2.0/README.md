# Comparing `tmp/trytond_account_invoice_history-7.0.0.tar.gz` & `tmp/trytond_account_invoice_history-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_history-7.0.0.tar", last modified: Mon Oct 30 17:21:06 2023, max compression
+gzip compressed data, was "trytond_account_invoice_history-7.2.0.tar", last modified: Mon Apr 29 15:33:56 2024, max compression
```

## Comparing `trytond_account_invoice_history-7.0.0.tar` & `trytond_account_invoice_history-7.2.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:06.799603 trytond_account_invoice_history-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:22:51.000000 trytond_account_invoice_history-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2668 2023-10-30 17:02:04.000000 trytond_account_invoice_history-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:02:04.000000 trytond_account_invoice_history-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_history-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2023-10-30 17:21:06.796269 trytond_account_invoice_history-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-08-13 15:26:13.000000 trytond_account_invoice_history-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4044 2023-08-13 15:26:13.000000 trytond_account_invoice_history-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.0.0/account_invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:06.796269 trytond_account_invoice_history-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:22:51.000000 trytond_account_invoice_history-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:51.000000 trytond_account_invoice_history-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:06.796269 trytond_account_invoice_history-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      234 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      252 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-28 12:11:19.000000 trytond_account_invoice_history-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-08-13 15:26:13.000000 trytond_account_invoice_history-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:21:06.799603 trytond_account_invoice_history-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4372 2023-10-27 17:38:49.000000 trytond_account_invoice_history-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:06.796269 trytond_account_invoice_history-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_invoice_history-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-30 17:02:00.000000 trytond_account_invoice_history-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:06.796269 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2023-10-30 17:21:06.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1424 2023-10-30 17:21:06.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:21:06.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:21:06.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-10-30 17:21:06.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:21:06.000000 trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:56.056300 trytond_account_invoice_history-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2769 2024-04-29 15:14:31.000000 trytond_account_invoice_history-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:14:31.000000 trytond_account_invoice_history-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_history-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2643 2024-04-29 15:33:56.052967 trytond_account_invoice_history-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      543 2024-01-27 09:58:52.000000 trytond_account_invoice_history-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4044 2024-01-27 09:58:52.000000 trytond_account_invoice_history-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.2.0/account_invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:56.052967 trytond_account_invoice_history-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_account_invoice_history-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:55.000000 trytond_account_invoice_history-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:56.052967 trytond_account_invoice_history-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      234 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      252 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-27 16:43:21.000000 trytond_account_invoice_history-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-01-27 09:58:52.000000 trytond_account_invoice_history-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:56.056300 trytond_account_invoice_history-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4372 2024-03-17 11:01:36.000000 trytond_account_invoice_history-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:56.052967 trytond_account_invoice_history-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_account_invoice_history-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:55.000000 trytond_account_invoice_history-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:14:26.000000 trytond_account_invoice_history-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:56.052967 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2643 2024-04-29 15:33:55.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1406 2024-04-29 15:33:56.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:55.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:33:55.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-04-29 15:33:55.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:55.000000 trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/top_level.txt
```

### Comparing `trytond_account_invoice_history-7.0.0/CHANGELOG` & `trytond_account_invoice_history-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_invoice_history-7.0.0/COPYRIGHT` & `trytond_account_invoice_history-7.2.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2023 Cédric Krier.
+Copyright (C) 2009-2024 Cédric Krier.
 Copyright (C) 2009-2012 Bertrand Chenal.
-Copyright (C) 2009-2023 B2CK SPRL.
+Copyright (C) 2009-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_history-7.0.0/LICENSE` & `trytond_account_invoice_history-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-7.0.0/PKG-INFO` & `trytond_account_invoice_history-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_history
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to historize invoices
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
@@ -49,16 +49,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Account Invoice History Module
 ##############################
 
 The account invoice history module activates the historization of the invoice
 and its related fields.
```

### Comparing `trytond_account_invoice_history-7.0.0/__init__.py` & `trytond_account_invoice_history-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-7.0.0/account.py` & `trytond_account_invoice_history-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-7.0.0/account_invoice.py` & `trytond_account_invoice_history-7.2.0/account_invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-7.0.0/doc/conf.py` & `trytond_account_invoice_history-7.2.0/doc/conf.py`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_invoice_history-7.0.0/setup.py` & `trytond_account_invoice_history-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-7.0.0/tox.ini` & `trytond_account_invoice_history-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/PKG-INFO` & `trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice-history
-Version: 7.0.0
+Name: trytond_account_invoice_history
+Version: 7.2.0
 Summary: Tryton module to historize invoices
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
@@ -49,16 +49,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Account Invoice History Module
 ##############################
 
 The account invoice history module activates the historization of the invoice
 and its related fields.
```

### Comparing `trytond_account_invoice_history-7.0.0/trytond_account_invoice_history.egg-info/SOURCES.txt` & `trytond_account_invoice_history-7.2.0/trytond_account_invoice_history.egg-info/SOURCES.txt`

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
