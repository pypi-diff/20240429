# Comparing `tmp/trytond_account_invoice_secondary_unit-7.0.0.tar.gz` & `tmp/trytond_account_invoice_secondary_unit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_secondary_unit-7.0.0.tar", last modified: Mon Oct 30 17:21:25 2023, max compression
+gzip compressed data, was "trytond_account_invoice_secondary_unit-7.2.0.tar", last modified: Mon Apr 29 15:34:08 2024, max compression
```

## Comparing `trytond_account_invoice_secondary_unit-7.0.0.tar` & `trytond_account_invoice_secondary_unit-7.2.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-22 17:22:52.000000 trytond_account_invoice_secondary_unit-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-10-30 17:02:13.000000 trytond_account_invoice_secondary_unit-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:02:12.000000 trytond_account_invoice_secondary_unit-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2673 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5031 2023-10-24 07:56:52.000000 trytond_account_invoice_secondary_unit-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2831 2023-10-22 17:22:52.000000 trytond_account_invoice_secondary_unit-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:52.000000 trytond_account_invoice_secondary_unit-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      996 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      960 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      942 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      939 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1001 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 16:47:45.000000 trytond_account_invoice_secondary_unit-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2023-10-27 17:38:49.000000 trytond_account_invoice_secondary_unit-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_invoice_secondary_unit-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-10-30 17:02:09.000000 trytond_account_invoice_secondary_unit-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2673 2023-10-30 17:21:24.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1511 2023-10-30 17:21:25.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:21:24.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-10-30 17:21:24.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-10-30 17:21:24.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:21:24.000000 trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:25.209690 trytond_account_invoice_secondary_unit-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.0.0/view/account_invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2024-04-29 15:14:42.000000 trytond_account_invoice_secondary_unit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:14:42.000000 trytond_account_invoice_secondary_unit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2673 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5031 2024-02-04 18:51:26.000000 trytond_account_invoice_secondary_unit-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:08.635971 trytond_account_invoice_secondary_unit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3093 2024-04-27 16:30:39.000000 trytond_account_invoice_secondary_unit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:55.000000 trytond_account_invoice_secondary_unit-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      996 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      960 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      942 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      939 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1001 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      974 2024-04-29 13:17:17.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:21.000000 trytond_account_invoice_secondary_unit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-03-17 11:01:36.000000 trytond_account_invoice_secondary_unit-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:55.000000 trytond_account_invoice_secondary_unit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-04-29 15:14:38.000000 trytond_account_invoice_secondary_unit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2673 2024-04-29 15:34:08.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1493 2024-04-29 15:34:08.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:08.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-29 15:34:08.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2024-04-29 15:34:08.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:08.000000 trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:08.639304 trytond_account_invoice_secondary_unit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-7.2.0/view/account_invoice_line_form.xml
```

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/CHANGELOG` & `trytond_account_invoice_secondary_unit-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/LICENSE` & `trytond_account_invoice_secondary_unit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/PKG-INFO` & `trytond_account_invoice_secondary_unit-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_secondary_unit
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on invoice line
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
@@ -47,18 +47,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Invoice Secondary Unit Module
 #####################################
 
 The account invoice secondary unit module adds a secondary unit of measure on
 invoice line.
```

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/account.py` & `trytond_account_invoice_secondary_unit-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/doc/conf.py` & `trytond_account_invoice_secondary_unit-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/bg.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/ca.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/cs.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/de.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/es.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/es_419.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/et.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/fa.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/fi.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/fr.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/hu.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/id.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/it.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/lo.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/lt.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/nl.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/pl.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/pt.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/ro.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Categorie Secundara UM pentru Produs"
 
 msgctxt "field:account.invoice.line,secondary_quantity:"
 msgid "Secondary Quantity"
 msgstr "Cantitate Secundara"
@@ -17,15 +16,15 @@
 
 msgctxt "field:account.invoice.line,secondary_unit_price:"
 msgid "Secondary Unit Price"
 msgstr "Preţ Unitate Secundara"
 
 msgctxt "help:account.invoice.line,product_secondary_uom_category:"
 msgid "The category of secondary Unit of Measure for the product."
-msgstr ""
+msgstr "Categoria Unitatii de Masura pentru produs."
 
 msgctxt "view:account.invoice.line:"
 msgid "Quantity:"
 msgstr "Cantitate:"
 
 msgctxt "view:account.invoice.line:"
 msgid "Unit Price:"
```

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/ru.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/sl.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/tr.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/uk.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/locale/zh_CN.po` & `trytond_account_invoice_secondary_unit-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/setup.py` & `trytond_account_invoice_secondary_unit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/tox.ini` & `trytond_account_invoice_secondary_unit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO` & `trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice-secondary-unit
-Version: 7.0.0
+Name: trytond_account_invoice_secondary_unit
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on invoice line
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
@@ -47,18 +47,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Invoice Secondary Unit Module
 #####################################
 
 The account invoice secondary unit module adds a secondary unit of measure on
 invoice line.
```

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt` & `trytond_account_invoice_secondary_unit-7.2.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_account_invoice_secondary_unit-7.0.0/view/account_invoice_line_form.xml` & `trytond_account_invoice_secondary_unit-7.2.0/view/account_invoice_line_form.xml`

 * *Files identical despite different names*

