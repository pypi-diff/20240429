# Comparing `tmp/trytond_account_fr_chorus-7.0.0.tar.gz` & `tmp/trytond_account_fr_chorus-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_fr_chorus-7.0.0.tar", last modified: Mon Oct 30 17:20:28 2023, max compression
+gzip compressed data, was "trytond_account_fr_chorus-7.2.0.tar", last modified: Mon Apr 29 15:33:27 2024, max compression
```

## Comparing `trytond_account_fr_chorus-7.0.0.tar` & `trytond_account_fr_chorus-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:28.966089 trytond_account_fr_chorus-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-22 17:22:51.000000 trytond_account_fr_chorus-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1281 2023-10-30 17:01:47.000000 trytond_account_fr_chorus-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:01:47.000000 trytond_account_fr_chorus-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_fr_chorus-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-10-30 17:20:28.966089 trytond_account_fr_chorus-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      778 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14108 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5356 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:28.966089 trytond_account_fr_chorus-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-22 17:22:51.000000 trytond_account_fr_chorus-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:51.000000 trytond_account_fr_chorus-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1313 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/edocument.py
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      542 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:28.962756 trytond_account_fr_chorus-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5005 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5009 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4785 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5157 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5072 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4320 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4220 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4237 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4957 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4240 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4207 2023-10-30 16:47:45.000000 trytond_account_fr_chorus-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:20.000000 trytond_account_fr_chorus-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:20:28.966089 trytond_account_fr_chorus-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4727 2023-10-27 17:38:49.000000 trytond_account_fr_chorus-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:28.962756 trytond_account_fr_chorus-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5058 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/tests/scenario_account_fr_chorus_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      580 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_fr_chorus-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-10-30 17:01:44.000000 trytond_account_fr_chorus-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:28.966089 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-10-30 17:20:28.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1908 2023-10-30 17:20:28.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:20:28.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-10-30 17:20:28.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:20:28.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:20:28.000000 trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:28.962756 trytond_account_fr_chorus-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      845 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/view/invoice_chorus_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-24 07:56:52.000000 trytond_account_fr_chorus-7.0.0/view/invoice_chorus_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_account_fr_chorus-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:27.587045 trytond_account_fr_chorus-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1382 2024-04-29 15:14:08.000000 trytond_account_fr_chorus-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:14:08.000000 trytond_account_fr_chorus-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_fr_chorus-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3013 2024-04-29 15:33:27.587045 trytond_account_fr_chorus-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      778 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14108 2024-03-25 13:26:54.000000 trytond_account_fr_chorus-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5264 2024-04-27 16:30:39.000000 trytond_account_fr_chorus-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:27.580378 trytond_account_fr_chorus-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_account_fr_chorus-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:54.000000 trytond_account_fr_chorus-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1313 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/edocument.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2024-03-25 13:26:54.000000 trytond_account_fr_chorus-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      542 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:27.583711 trytond_account_fr_chorus-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4985 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5005 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5009 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4785 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5157 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5072 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4320 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4220 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4237 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4957 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4240 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4207 2024-04-27 16:43:20.000000 trytond_account_fr_chorus-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2024-03-25 13:26:54.000000 trytond_account_fr_chorus-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:20.000000 trytond_account_fr_chorus-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:27.587045 trytond_account_fr_chorus-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4718 2024-04-27 16:30:39.000000 trytond_account_fr_chorus-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:27.583711 trytond_account_fr_chorus-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5043 2024-04-22 12:14:36.000000 trytond_account_fr_chorus-7.2.0/tests/scenario_account_fr_chorus_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_account_fr_chorus-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      580 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:54.000000 trytond_account_fr_chorus-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2024-04-29 15:14:03.000000 trytond_account_fr_chorus-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:27.583711 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3013 2024-04-29 15:33:27.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1890 2024-04-29 15:33:27.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:27.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:33:27.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-29 15:33:27.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:27.000000 trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:27.583711 trytond_account_fr_chorus-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      845 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/view/invoice_chorus_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-02-04 18:51:26.000000 trytond_account_fr_chorus-7.2.0/view/invoice_chorus_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_account_fr_chorus-7.2.0/view/party_form.xml
```

### Comparing `trytond_account_fr_chorus-7.0.0/CHANGELOG` & `trytond_account_fr_chorus-7.2.0/CHANGELOG`

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
 * Update to PISTE API
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_account_fr_chorus-7.0.0/COPYRIGHT` & `trytond_account_fr_chorus-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_fr_chorus-7.0.0/LICENSE` & `trytond_account_fr_chorus-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/PKG-INFO` & `trytond_account_fr_chorus-7.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_fr_chorus
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to communicate with Chorus
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-fr-chorus
+Project-URL: Documentation, https://docs.tryton.org/modules-account-fr-chorus
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton chorus
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -50,24 +50,24 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
 Requires-Dist: requests_oauthlib
 Requires-Dist: oauthlib
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_party_siret<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_party_siret<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_fr<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_edocument_uncefact<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_fr<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_edocument_uncefact<7.3,>=7.2; extra == "test"
 
 ############################
 Account French Chorus Module
 ############################
 
 The *Account French Chorus Module* allows to send invoices through the `Chorus
 Pro <https://chorus-pro.gouv.fr/>`_ portal.
```

### Comparing `trytond_account_fr_chorus-7.0.0/__init__.py` & `trytond_account_fr_chorus-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/account.py` & `trytond_account_fr_chorus-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/account.xml` & `trytond_account_fr_chorus-7.2.0/account.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_account_fr_chorus-7.0.0/account.xml` & `trytond_account_fr_chorus-7.2.0/account.xml`

```diff
@@ -57,37 +57,37 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_invoice_chorus_form"/>
     </record>
     <menuitem parent="account_invoice.menu_invoice_out_form" action="act_invoice_chorus_form" sequence="50" id="menu_invoice_chorus_form"/>
     <record model="ir.model.access" id="access_invoice_chorus">
-      <field name="model" search="[('model', '=', 'account.invoice.chorus')]"/>
+      <field name="model">account.invoice.chorus</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_account_chorus">
-      <field name="model" search="[('model', '=', 'account.invoice.chorus')]"/>
+      <field name="model">account.invoice.chorus</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="invoice_chorus_send_button">
+      <field name="model">account.invoice.chorus</field>
       <field name="name">send</field>
       <field name="string">Send</field>
-      <field name="model" search="[('model', '=', 'account.invoice.chorus')]"/>
     </record>
     <record model="ir.model.button" id="invoice_chorus_update_button">
+      <field name="model">account.invoice.chorus</field>
       <field name="name">update</field>
       <field name="string">Update</field>
-      <field name="model" search="[('model', '=', 'account.invoice.chorus')]"/>
     </record>
     <record model="ir.cron" id="cron_invoice_send">
       <field name="method">account.invoice.chorus|send</field>
       <field name="interval_number" eval="15"/>
       <field name="interval_type">minutes</field>
     </record>
     <record model="ir.cron" id="cron_invoice_update">
```

### Comparing `trytond_account_fr_chorus-7.0.0/doc/conf.py` & `trytond_account_fr_chorus-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_fr_chorus-7.0.0/doc/design.rst` & `trytond_account_fr_chorus-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/doc/setup.rst` & `trytond_account_fr_chorus-7.2.0/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/doc/usage.rst` & `trytond_account_fr_chorus-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/edocument.py` & `trytond_account_fr_chorus-7.2.0/edocument.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/ir.py` & `trytond_account_fr_chorus-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/bg.po` & `trytond_account_fr_chorus-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/ca.po` & `trytond_account_fr_chorus-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/cs.po` & `trytond_account_fr_chorus-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/de.po` & `trytond_account_fr_chorus-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/es.po` & `trytond_account_fr_chorus-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/es_419.po` & `trytond_account_fr_chorus-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/et.po` & `trytond_account_fr_chorus-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/fa.po` & `trytond_account_fr_chorus-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/fi.po` & `trytond_account_fr_chorus-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/fr.po` & `trytond_account_fr_chorus-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/hu.po` & `trytond_account_fr_chorus-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/id.po` & `trytond_account_fr_chorus-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/it.po` & `trytond_account_fr_chorus-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/lo.po` & `trytond_account_fr_chorus-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/lt.po` & `trytond_account_fr_chorus-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/nl.po` & `trytond_account_fr_chorus-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/pl.po` & `trytond_account_fr_chorus-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/pt.po` & `trytond_account_fr_chorus-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/ro.po` & `trytond_account_fr_chorus-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/ru.po` & `trytond_account_fr_chorus-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/sl.po` & `trytond_account_fr_chorus-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/tr.po` & `trytond_account_fr_chorus-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/uk.po` & `trytond_account_fr_chorus-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/locale/zh_CN.po` & `trytond_account_fr_chorus-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/message.xml` & `trytond_account_fr_chorus-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/setup.py` & `trytond_account_fr_chorus-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-fr-chorus'),
+            'https://docs.tryton.org/modules-account-fr-chorus'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton chorus',
     package_dir={'trytond.modules.account_fr_chorus': '.'},
     packages=(
         ['trytond.modules.account_fr_chorus']
```

### Comparing `trytond_account_fr_chorus-7.0.0/tests/scenario_account_fr_chorus_invoice.rst` & `trytond_account_fr_chorus-7.2.0/tests/scenario_account_fr_chorus_invoice.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 Imports::
 
     >>> import datetime as dt
     >>> import os
     >>> import time
     >>> import uuid
     >>> from decimal import Decimal
+    >>> from unittest.mock import patch
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.modules.party.party import Identifier
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Patch SIRET validation::
 
-    >>> from unittest.mock import patch
-    >>> from trytond.modules.party.party import Identifier
     >>> mock = patch.object(
     ...     Identifier, 'check_code',
     ...     return_value=None).start()
 
 Activate modules::
 
     >>> config = activate_modules([
```

### Comparing `trytond_account_fr_chorus-7.0.0/tests/test_scenario.py` & `trytond_account_fr_chorus-7.2.0/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/tox.ini` & `trytond_account_fr_chorus-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/PKG-INFO` & `trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-fr-chorus
-Version: 7.0.0
+Name: trytond_account_fr_chorus
+Version: 7.2.0
 Summary: Tryton module to communicate with Chorus
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-fr-chorus
+Project-URL: Documentation, https://docs.tryton.org/modules-account-fr-chorus
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton chorus
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -50,24 +50,24 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
 Requires-Dist: requests_oauthlib
 Requires-Dist: oauthlib
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_party_siret<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_party_siret<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_fr<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_edocument_uncefact<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_fr<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_edocument_uncefact<7.3,>=7.2; extra == "test"
 
 ############################
 Account French Chorus Module
 ############################
 
 The *Account French Chorus Module* allows to send invoices through the `Chorus
 Pro <https://chorus-pro.gouv.fr/>`_ portal.
```

### Comparing `trytond_account_fr_chorus-7.0.0/trytond_account_fr_chorus.egg-info/SOURCES.txt` & `trytond_account_fr_chorus-7.2.0/trytond_account_fr_chorus.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_fr_chorus-7.0.0/view/configuration_form.xml` & `trytond_account_fr_chorus-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr_chorus-7.0.0/view/invoice_chorus_form.xml` & `trytond_account_fr_chorus-7.2.0/view/invoice_chorus_form.xml`

 * *Files identical despite different names*

