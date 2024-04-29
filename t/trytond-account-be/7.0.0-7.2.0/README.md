# Comparing `tmp/trytond_account_be-7.0.0.tar.gz` & `tmp/trytond_account_be-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_be-7.0.0.tar", last modified: Mon Oct 30 17:18:21 2023, max compression
+gzip compressed data, was "trytond_account_be-7.2.0.tar", last modified: Mon Apr 29 15:31:45 2024, max compression
```

## Comparing `trytond_account_be-7.0.0.tar` & `trytond_account_be-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:21.178813 trytond_account_be-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-22 17:22:47.000000 trytond_account_be-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2725 2023-10-30 17:00:50.000000 trytond_account_be-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:00:50.000000 trytond_account_be-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_be-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2182 2023-10-30 17:18:21.178813 trytond_account_be-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-08-13 15:26:13.000000 trytond_account_be-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5834 2023-08-13 15:26:13.000000 trytond_account_be-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   300597 2023-10-07 15:40:36.000000 trytond_account_be-7.0.0/account_be.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   247910 2023-10-07 15:40:36.000000 trytond_account_be-7.0.0/account_be_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   248385 2023-10-07 15:40:36.000000 trytond_account_be-7.0.0/account_be_nl.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:21.175479 trytond_account_be-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-22 17:22:47.000000 trytond_account_be-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:47.000000 trytond_account_be-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:21.172146 trytond_account_be-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1247 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1372 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1099 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1228 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1096 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1220 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-10-28 12:11:19.000000 trytond_account_be-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:18:21.178813 trytond_account_be-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3494 2023-10-27 17:38:49.000000 trytond_account_be-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   169644 2023-08-13 15:26:13.000000 trytond_account_be-7.0.0/tax_be.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   159994 2023-08-13 15:26:13.000000 trytond_account_be-7.0.0/tax_be_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   159831 2023-08-13 15:26:13.000000 trytond_account_be-7.0.0/tax_be_nl.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:21.175479 trytond_account_be-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_be-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:00:47.000000 trytond_account_be-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:21.175479 trytond_account_be-7.0.0/trytond_account_be.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2182 2023-10-30 17:18:20.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1602 2023-10-30 17:18:21.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:18:20.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-10-30 17:18:20.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       73 2023-10-30 17:18:20.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:18:20.000000 trytond_account_be-7.0.0/trytond_account_be.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:21.175479 trytond_account_be-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-16 14:00:20.000000 trytond_account_be-7.0.0/view/vat_customer_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account_be-7.0.0/view/vat_customer_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2826 2024-04-29 15:12:48.000000 trytond_account_be-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:12:48.000000 trytond_account_be-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_be-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2182 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5834 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   300597 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/account_be.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   247910 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/account_be_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   248385 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/account_be_nl.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:45.596379 trytond_account_be-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_account_be-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account_be-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1250 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1247 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1372 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1099 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1228 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1096 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1220 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1040 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-04-27 16:43:20.000000 trytond_account_be-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3494 2024-03-17 11:01:36.000000 trytond_account_be-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   169644 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/tax_be.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   159994 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/tax_be_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   159831 2024-01-27 09:58:52.000000 trytond_account_be-7.2.0/tax_be_nl.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account_be-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:12:44.000000 trytond_account_be-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/trytond_account_be.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2182 2024-04-29 15:31:45.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1584 2024-04-29 15:31:45.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:45.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:31:45.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       73 2024-04-29 15:31:45.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:45.000000 trytond_account_be-7.2.0/trytond_account_be.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:45.599712 trytond_account_be-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-16 14:00:20.000000 trytond_account_be-7.2.0/view/vat_customer_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account_be-7.2.0/view/vat_customer_list.xml
```

### Comparing `trytond_account_be-7.0.0/CHANGELOG` & `trytond_account_be-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_be-7.0.0/LICENSE` & `trytond_account_be-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/PKG-INFO` & `trytond_account_be-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_be
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with Belgian chart of accounts
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
@@ -29,17 +29,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_eu<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_eu<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Belgian Account Module
 ######################
 
 The Belgian account module defines the standard chart of account.
 
 The module generates french and dutch chart of accounts / chart of taxes. The
```

### Comparing `trytond_account_be-7.0.0/README.rst` & `trytond_account_be-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/account.py` & `trytond_account_be-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/account.xml` & `trytond_account_be-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/account_be.xml` & `trytond_account_be-7.2.0/account_be.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/account_be_fr.xml` & `trytond_account_be-7.2.0/account_be_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/account_be_nl.xml` & `trytond_account_be-7.2.0/account_be_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/doc/conf.py` & `trytond_account_be-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_be-7.0.0/doc/index.rst` & `trytond_account_be-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/bg.po` & `trytond_account_be-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/ca.po` & `trytond_account_be-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/cs.po` & `trytond_account_be-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/de.po` & `trytond_account_be-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/es.po` & `trytond_account_be-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/es_419.po` & `trytond_account_be-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/et.po` & `trytond_account_be-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/fa.po` & `trytond_account_be-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/fi.po` & `trytond_account_be-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/fr.po` & `trytond_account_be-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/hu.po` & `trytond_account_be-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/id.po` & `trytond_account_be-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/it.po` & `trytond_account_be-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/lo.po` & `trytond_account_be-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/lt.po` & `trytond_account_be-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/nl.po` & `trytond_account_be-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/pl.po` & `trytond_account_be-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/pt.po` & `trytond_account_be-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/ro.po` & `trytond_account_be-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/ru.po` & `trytond_account_be-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/sl.po` & `trytond_account_be-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/tr.po` & `trytond_account_be-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/uk.po` & `trytond_account_be-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/locale/zh_CN.po` & `trytond_account_be-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/localize.xsl` & `trytond_account_be-7.2.0/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/setup.py` & `trytond_account_be-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/tax_be.xml` & `trytond_account_be-7.2.0/tax_be.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/tax_be_fr.xml` & `trytond_account_be-7.2.0/tax_be_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/tax_be_nl.xml` & `trytond_account_be-7.2.0/tax_be_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/tests/test_module.py` & `trytond_account_be-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/tox.ini` & `trytond_account_be-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_be-7.0.0/trytond_account_be.egg-info/PKG-INFO` & `trytond_account_be-7.2.0/trytond_account_be.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-be
-Version: 7.0.0
+Name: trytond_account_be
+Version: 7.2.0
 Summary: Tryton module with Belgian chart of accounts
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
@@ -29,17 +29,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_eu<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_eu<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Belgian Account Module
 ######################
 
 The Belgian account module defines the standard chart of account.
 
 The module generates french and dutch chart of accounts / chart of taxes. The
```

### Comparing `trytond_account_be-7.0.0/trytond_account_be.egg-info/SOURCES.txt` & `trytond_account_be-7.2.0/trytond_account_be.egg-info/SOURCES.txt`

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

