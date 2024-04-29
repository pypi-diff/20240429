# Comparing `tmp/trytond_account_es_sii-7.0.0.tar.gz` & `tmp/trytond_account_es_sii-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es_sii-7.0.0.tar", last modified: Mon Oct 30 17:20:02 2023, max compression
+gzip compressed data, was "trytond_account_es_sii-7.2.0.tar", last modified: Mon Apr 29 15:33:06 2024, max compression
```

## Comparing `trytond_account_es_sii-7.0.0.tar` & `trytond_account_es_sii-7.2.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:02.252628 trytond_account_es_sii-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:22:50.000000 trytond_account_es_sii-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:01:36.000000 trytond_account_es_sii-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:01:36.000000 trytond_account_es_sii-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2023-10-30 17:20:02.252628 trytond_account_es_sii-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-08-13 15:26:13.000000 trytond_account_es_sii-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24770 2023-10-07 15:40:36.000000 trytond_account_es_sii-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5887 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:02.249295 trytond_account_es_sii-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:22:50.000000 trytond_account_es_sii-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1085 2023-08-13 15:26:13.000000 trytond_account_es_sii-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-06-10 11:39:56.000000 trytond_account_es_sii-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:50.000000 trytond_account_es_sii-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:02.245962 trytond_account_es_sii-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5430 2023-10-30 16:47:45.000000 trytond_account_es_sii-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5476 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5566 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4430 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5484 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-10-28 12:11:19.000000 trytond_account_es_sii-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      979 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:20:02.252628 trytond_account_es_sii-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4632 2023-10-27 17:38:49.000000 trytond_account_es_sii-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12629 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:02.245962 trytond_account_es_sii-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2039 2023-08-13 15:26:13.000000 trytond_account_es_sii-7.0.0/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    24476 2023-10-27 17:38:49.000000 trytond_account_es_sii-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-08-13 15:26:13.000000 trytond_account_es_sii-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_es_sii-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      135 2023-10-30 17:01:33.000000 trytond_account_es_sii-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:02.252628 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2023-10-30 17:20:01.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-10-30 17:20:02.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:20:01.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:20:01.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-10-30 17:20:01.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:20:01.000000 trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:02.249295 trytond_account_es_sii-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/invoice_sii_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/invoice_sii_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.0.0/view/tax_template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:13:49.000000 trytond_account_es_sii-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:13:49.000000 trytond_account_es_sii-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      677 2024-01-27 09:58:52.000000 trytond_account_es_sii-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24770 2024-02-04 18:51:26.000000 trytond_account_es_sii-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5818 2024-04-27 16:30:39.000000 trytond_account_es_sii-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:06.714257 trytond_account_es_sii-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_account_es_sii-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1085 2024-01-27 09:58:52.000000 trytond_account_es_sii-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2024-01-27 09:58:52.000000 trytond_account_es_sii-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:53.000000 trytond_account_es_sii-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5430 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5476 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5566 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4430 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5484 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4461 2024-04-29 13:17:17.000000 trytond_account_es_sii-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2024-04-27 16:43:20.000000 trytond_account_es_sii-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      979 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4632 2024-03-17 11:01:36.000000 trytond_account_es_sii-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12629 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2017 2024-04-22 12:14:36.000000 trytond_account_es_sii-7.2.0/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    24476 2024-02-04 18:51:26.000000 trytond_account_es_sii-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_account_es_sii-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:53.000000 trytond_account_es_sii-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-04-29 15:13:43.000000 trytond_account_es_sii-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-29 15:33:06.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1963 2024-04-29 15:33:06.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:06.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:33:06.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-29 15:33:06.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:06.000000 trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:06.717590 trytond_account_es_sii-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/invoice_sii_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/invoice_sii_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-7.2.0/view/tax_template_form.xml
```

### Comparing `trytond_account_es_sii-7.0.0/COPYRIGHT` & `trytond_account_es_sii-7.2.0/COPYRIGHT`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2020-2023 Sergi Almacellas Abellana
-Copyright (C) 2023 B2CK
-Copyright (C) 2023 Cédric Krier
+Copyright (C) 2023-2024 B2CK
+Copyright (C) 2023-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_es_sii-7.0.0/LICENSE` & `trytond_account_es_sii-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/PKG-INFO` & `trytond_account_es_sii-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_es_sii
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that sends invoices to the Spanish SII webservice
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
@@ -50,20 +50,20 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: zeep
 Requires-Dist: requests
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_es<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_es<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##########################
 Acounts Spanish SII Module
 ##########################
 
 The *Account Spanish SII Module* allow to send invoices to the `SII
 <https://www.agenciatributaria.es/AEAT.internet/Ayuda_P_G417_IVA_Llevanza_libros_registro_SII.shtml>`_
```

### Comparing `trytond_account_es_sii-7.0.0/__init__.py` & `trytond_account_es_sii-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/account.py` & `trytond_account_es_sii-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/account.xml` & `trytond_account_es_sii-7.2.0/account.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account_es_sii-7.0.0/account.xml` & `trytond_account_es_sii-7.2.0/account.xml`

```diff
@@ -76,30 +76,30 @@
     <record model="ir.action.act_window.domain" id="act_invoice_sii_form_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="act_window" ref="act_invoice_sii_form"/>
     </record>
     <menuitem parent="account_invoice.menu_invoices" action="act_invoice_sii_form" id="menu_invoice_sii_form"/>
     <record model="ir.model.access" id="access_invoice_sii">
-      <field name="model" search="[('model', '=', 'account.invoice.sii')]"/>
+      <field name="model">account.invoice.sii</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_sii_account">
-      <field name="model" search="[('model', '=', 'account.invoice.sii')]"/>
+      <field name="model">account.invoice.sii</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_sii_account_admin">
-      <field name="model" search="[('model', '=', 'account.invoice.sii')]"/>
+      <field name="model">account.invoice.sii</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.cron" id="cron_invoice_send">
```

### Comparing `trytond_account_es_sii-7.0.0/doc/conf.py` & `trytond_account_es_sii-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_es_sii-7.0.0/doc/configuration.rst` & `trytond_account_es_sii-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/doc/design.rst` & `trytond_account_es_sii-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/bg.po` & `trytond_account_es_sii-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/ca.po` & `trytond_account_es_sii-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/cs.po` & `trytond_account_es_sii-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/de.po` & `trytond_account_es_sii-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/es.po` & `trytond_account_es_sii-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/es_419.po` & `trytond_account_es_sii-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/et.po` & `trytond_account_es_sii-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/fa.po` & `trytond_account_es_sii-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/fi.po` & `trytond_account_es_sii-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/fr.po` & `trytond_account_es_sii-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/hu.po` & `trytond_account_es_sii-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/id.po` & `trytond_account_es_sii-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/it.po` & `trytond_account_es_sii-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/lo.po` & `trytond_account_es_sii-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/lt.po` & `trytond_account_es_sii-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/nl.po` & `trytond_account_es_sii-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/pl.po` & `trytond_account_es_sii-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/pt.po` & `trytond_account_es_sii-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/ro.po` & `trytond_account_es_sii-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/ru.po` & `trytond_account_es_sii-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/sl.po` & `trytond_account_es_sii-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/tr.po` & `trytond_account_es_sii-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/uk.po` & `trytond_account_es_sii-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/locale/zh_CN.po` & `trytond_account_es_sii-7.2.0/locale/ro.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #
+#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.configuration,es_sii_environment:"
 msgid "SII Environment"
-msgstr ""
+msgstr "Mediu SII"
 
+#, fuzzy
 msgctxt "field:account.configuration,es_sii_url:"
 msgid "SII URL"
-msgstr ""
+msgstr "URL SII"
 
 msgctxt "field:account.credential.sii,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
+#, fuzzy
 msgctxt "field:account.credential.sii,es_sii_environment:"
 msgid "SII Environment"
-msgstr ""
+msgstr "Mediu SII"
 
 msgctxt "field:account.credential.sii,es_sii_url:"
 msgid "SII URL"
 msgstr ""
 
 msgctxt "field:account.fiscalyear,es_sii_send_invoices:"
 msgid "Send invoices to SII"
```

### Comparing `trytond_account_es_sii-7.0.0/message.xml` & `trytond_account_es_sii-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/party.py` & `trytond_account_es_sii-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/setup.py` & `trytond_account_es_sii-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/tax.xml` & `trytond_account_es_sii-7.2.0/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/tests/scenario_renew_fiscalyear.rst` & `trytond_account_es_sii-7.2.0/tests/scenario_renew_fiscalyear.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ========================================
 Account ES SSI Renew Fiscalyear Scenario
 ========================================
 
 Imports::
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Wizard
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_es_sii')
 
 Create company::
```

### Comparing `trytond_account_es_sii-7.0.0/tests/test_module.py` & `trytond_account_es_sii-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/tox.ini` & `trytond_account_es_sii-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/PKG-INFO` & `trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-es-sii
-Version: 7.0.0
+Name: trytond_account_es_sii
+Version: 7.2.0
 Summary: Tryton module that sends invoices to the Spanish SII webservice
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
@@ -50,20 +50,20 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: zeep
 Requires-Dist: requests
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_es<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_es<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##########################
 Acounts Spanish SII Module
 ##########################
 
 The *Account Spanish SII Module* allow to send invoices to the `SII
 <https://www.agenciatributaria.es/AEAT.internet/Ayuda_P_G417_IVA_Llevanza_libros_registro_SII.shtml>`_
```

### Comparing `trytond_account_es_sii-7.0.0/trytond_account_es_sii.egg-info/SOURCES.txt` & `trytond_account_es_sii-7.2.0/trytond_account_es_sii.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_es_sii-7.0.0/view/tax_form.xml` & `trytond_account_es_sii-7.2.0/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-7.0.0/view/tax_template_form.xml` & `trytond_account_es_sii-7.2.0/view/tax_template_form.xml`

 * *Files identical despite different names*

