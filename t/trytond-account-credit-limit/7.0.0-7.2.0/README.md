# Comparing `tmp/trytond_account_credit_limit-7.0.0.tar.gz` & `tmp/trytond_account_credit_limit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_credit_limit-7.0.0.tar", last modified: Mon Oct 30 17:18:53 2023, max compression
+gzip compressed data, was "trytond_account_credit_limit-7.2.0.tar", last modified: Mon Apr 29 15:32:14 2024, max compression
```

## Comparing `trytond_account_credit_limit-7.0.0.tar` & `trytond_account_credit_limit-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:53.558967 trytond_account_credit_limit-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:22:48.000000 trytond_account_credit_limit-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1776 2023-10-30 17:01:05.000000 trytond_account_credit_limit-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:01:05.000000 trytond_account_credit_limit-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2023-10-30 17:18:53.558967 trytond_account_credit_limit-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1964 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-04-15 07:12:15.000000 trytond_account_credit_limit-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:53.558967 trytond_account_credit_limit-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:22:48.000000 trytond_account_credit_limit-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:48.000000 trytond_account_credit_limit-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:53.555634 trytond_account_credit_limit-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2800 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3345 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2652 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3233 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3393 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2860 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3270 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3768 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2652 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3436 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3261 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2885 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3654 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2804 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3286 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2668 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3378 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2747 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2023-10-30 16:47:45.000000 trytond_account_credit_limit-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2652 2023-10-28 12:11:19.000000 trytond_account_credit_limit-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5720 2023-08-13 15:26:13.000000 trytond_account_credit_limit-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:18:53.558967 trytond_account_credit_limit-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4475 2023-10-27 17:38:49.000000 trytond_account_credit_limit-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:53.555634 trytond_account_credit_limit-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3367 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_credit_limit-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      159 2023-10-30 17:01:02.000000 trytond_account_credit_limit-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:53.558967 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2023-10-30 17:18:53.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1683 2023-10-30 17:18:53.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:18:53.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:18:53.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      136 2023-10-30 17:18:53.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:18:53.000000 trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:53.558967 trytond_account_credit_limit-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.0.0/view/dunning_level_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      542 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:14.652285 trytond_account_credit_limit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1877 2024-04-29 15:13:07.000000 trytond_account_credit_limit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:13:07.000000 trytond_account_credit_limit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-04-29 15:32:14.652285 trytond_account_credit_limit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1964 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2575 2024-04-27 16:30:39.000000 trytond_account_credit_limit-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:14.645619 trytond_account_credit_limit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_account_credit_limit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:51.000000 trytond_account_credit_limit-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:14.648952 trytond_account_credit_limit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2800 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3345 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3233 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3393 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3270 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3768 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3436 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3261 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2885 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3654 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2804 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3286 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2668 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3378 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3268 2024-04-29 13:17:17.000000 trytond_account_credit_limit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2820 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-27 16:43:20.000000 trytond_account_credit_limit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5720 2024-01-27 09:58:52.000000 trytond_account_credit_limit-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1202 2024-04-27 16:30:39.000000 trytond_account_credit_limit-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:14.652285 trytond_account_credit_limit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4475 2024-03-17 11:01:36.000000 trytond_account_credit_limit-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:14.648952 trytond_account_credit_limit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3367 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:51.000000 trytond_account_credit_limit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      159 2024-04-29 15:13:03.000000 trytond_account_credit_limit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:14.648952 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-04-29 15:32:14.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1665 2024-04-29 15:32:14.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:14.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:32:14.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      136 2024-04-29 15:32:14.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:14.000000 trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:14.648952 trytond_account_credit_limit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.2.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account_credit_limit-7.2.0/view/dunning_level_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      542 2023-01-16 14:00:20.000000 trytond_account_credit_limit-7.2.0/view/party_form.xml
```

### Comparing `trytond_account_credit_limit-7.0.0/CHANGELOG` & `trytond_account_credit_limit-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_account_credit_limit-7.0.0/COPYRIGHT` & `trytond_account_credit_limit-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2011-2023 Cédric Krier.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 Cédric Krier.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_credit_limit-7.0.0/LICENSE` & `trytond_account_credit_limit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/PKG-INFO` & `trytond_account_credit_limit-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_credit_limit
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for account credit limit
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
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_account_dunning<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_account_dunning<7.3,>=7.2; extra == "test"
 
 Account Credit Limit
 ####################
 
 The account_credit_limit module manages credit limit of parties. A "Credit
 Limit Amount" is added on Party. The module allows to check for a party:
```

### Comparing `trytond_account_credit_limit-7.0.0/__init__.py` & `trytond_account_credit_limit-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/account.py` & `trytond_account_credit_limit-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/account.xml` & `trytond_account_credit_limit-7.2.0/account.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account_credit_limit-7.0.0/account.xml` & `trytond_account_credit_limit-7.2.0/account.xml`

```diff
@@ -12,20 +12,22 @@
     </record>
     <record model="ir.ui.view" id="configuration_view_form">
       <field name="model">account.configuration</field>
       <field name="inherit" ref="account.configuration_view_form"/>
       <field name="name">configuration_form</field>
     </record>
     <record model="ir.model.field.access" id="model_field_access_default_credit_limit_amount">
-      <field name="field" search="[('model.model', '=', 'account.configuration'), ('name', '=', 'default_credit_limit_amount')]"/>
+      <field name="model">account.configuration</field>
+      <field name="field">default_credit_limit_amount</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="model_field_access_default_credit_limit_amount_group_credit_limit">
-      <field name="field" search="[('model.model', '=', 'account.configuration'), ('name', '=', 'default_credit_limit_amount')]"/>
+      <field name="model">account.configuration</field>
+      <field name="field">default_credit_limit_amount</field>
       <field name="group" ref="group_credit_limit"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
   <data depends="account_dunning">
     <record model="ir.ui.view" id="dunning_level_view_form">
```

### Comparing `trytond_account_credit_limit-7.0.0/doc/conf.py` & `trytond_account_credit_limit-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_account_credit_limit-7.0.0/locale/bg.po` & `trytond_account_credit_limit-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/ca.po` & `trytond_account_credit_limit-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/cs.po` & `trytond_account_credit_limit-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/de.po` & `trytond_account_credit_limit-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/es.po` & `trytond_account_credit_limit-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/es_419.po` & `trytond_account_credit_limit-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/et.po` & `trytond_account_credit_limit-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/fa.po` & `trytond_account_credit_limit-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/fi.po` & `trytond_account_credit_limit-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/fr.po` & `trytond_account_credit_limit-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/hu.po` & `trytond_account_credit_limit-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/id.po` & `trytond_account_credit_limit-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/it.po` & `trytond_account_credit_limit-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/lo.po` & `trytond_account_credit_limit-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/lt.po` & `trytond_account_credit_limit-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/nl.po` & `trytond_account_credit_limit-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/pl.po` & `trytond_account_credit_limit-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/pt.po` & `trytond_account_credit_limit-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/ro.po` & `trytond_account_credit_limit-7.2.0/locale/sl.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,default_credit_limit_amount:"
 msgid "Default Credit Limit Amount"
-msgstr ""
+msgstr "Privzeti znesek odobrenega limita"
 
 msgctxt "field:account.configuration,default_credit_limit_amount_digits:"
 msgid "Currency Digits"
-msgstr "Zecimale valută"
+msgstr "Decimalke"
 
 msgctxt "field:account.configuration.default_credit_limit_amount,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Družba"
 
 msgctxt ""
 "field:account.configuration.default_credit_limit_amount,default_credit_limit_amount:"
 msgid "Default Credit Limit Amount"
-msgstr ""
+msgstr "Privzeti znesek odobrenega limita"
 
 msgctxt ""
 "field:account.configuration.default_credit_limit_amount,default_credit_limit_amount_digits:"
 msgid "Currency Digits"
-msgstr "Zecimale valută"
+msgstr "Decimalke"
 
 msgctxt "field:account.dunning.level,credit_limit:"
 msgid "Credit Limit"
-msgstr "Limita de credit"
+msgstr "Odobreni limit"
 
 msgctxt "field:party.party,credit_amount:"
 msgid "Credit Amount"
-msgstr "Suma de credit"
+msgstr "Odobreni limit"
 
 msgctxt "field:party.party,credit_limit_amount:"
 msgid "Credit Limit Amount"
-msgstr ""
+msgstr "Znesek odobrenega limita"
 
 msgctxt "field:party.party,credit_limit_amounts:"
 msgid "Credit Limit Amounts"
-msgstr ""
+msgstr "Znesek odobrenega limita"
 
 msgctxt "field:party.party,credit_limit_digits:"
 msgid "Currency Digits"
-msgstr "Zecimale valută"
+msgstr "Decimalke"
 
 msgctxt "field:party.party.credit_limit_amount,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Družba"
 
 msgctxt "field:party.party.credit_limit_amount,credit_limit_amount:"
 msgid "Credit Limit Amount"
-msgstr ""
+msgstr "Znesek odobrenega limita"
 
 msgctxt "field:party.party.credit_limit_amount,credit_limit_digits:"
 msgid "Currency Digits"
-msgstr "Zecimale valută"
+msgstr "Decimalke"
 
 msgctxt "field:party.party.credit_limit_amount,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Partner"
 
 msgctxt "help:account.configuration,default_credit_limit_amount:"
 msgid "The default credit limit amount for new customers."
 msgstr ""
 
 msgctxt ""
 "help:account.configuration.default_credit_limit_amount,default_credit_limit_amount:"
 msgid "The default credit limit amount for new customers."
 msgstr ""
 
 msgctxt "help:account.dunning.level,credit_limit:"
 msgid "Has reached the credit limit."
-msgstr ""
+msgstr "Kreditni limit presežen."
 
 msgctxt "model:account.configuration.default_credit_limit_amount,name:"
 msgid "Account Configuration Default Credit Limit Amount"
-msgstr ""
+msgstr "Konfiguracija privzetega odobrenega limita"
 
 msgctxt "model:ir.message,text:msg_party_credit_limit_amount"
 msgid "Party \"%(party)s\" has reached their credit limit of %(limit)s."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_credit_limit_dunning"
 msgid "Party \"%(party)s\" has reached the credit limit level of %(dunning)s."
 msgstr ""
 
 msgctxt "model:party.party.credit_limit_amount,name:"
 msgid "Party Credit Limit Amount"
-msgstr ""
+msgstr "Partnerjev odobreni limit"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_credit_limit"
 msgid "Account Credit Limit"
-msgstr ""
+msgstr "Account Credit Limit"
 
 msgctxt "view:account.configuration:"
 msgid "Credit Limit"
-msgstr ""
+msgstr "Odobreni limit"
 
 msgctxt "view:party.party:"
 msgid "Credit Limit"
-msgstr ""
+msgstr "Odobreni limit"
```

### Comparing `trytond_account_credit_limit-7.0.0/locale/ru.po` & `trytond_account_credit_limit-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/sl.po` & `trytond_account_credit_limit-7.2.0/locale/tr.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,default_credit_limit_amount:"
 msgid "Default Credit Limit Amount"
-msgstr "Privzeti znesek odobrenega limita"
+msgstr "Öntanımlı Kredi Limit Miktarı"
 
 msgctxt "field:account.configuration,default_credit_limit_amount_digits:"
 msgid "Currency Digits"
-msgstr "Decimalke"
+msgstr "Para Birimi Basamakları"
 
 msgctxt "field:account.configuration.default_credit_limit_amount,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Şirket"
 
 msgctxt ""
 "field:account.configuration.default_credit_limit_amount,default_credit_limit_amount:"
 msgid "Default Credit Limit Amount"
-msgstr "Privzeti znesek odobrenega limita"
+msgstr "Öntanımlı Kredi Limit Miktarı"
 
 msgctxt ""
 "field:account.configuration.default_credit_limit_amount,default_credit_limit_amount_digits:"
 msgid "Currency Digits"
-msgstr "Decimalke"
+msgstr "Para Birimi Basamakları"
 
 msgctxt "field:account.dunning.level,credit_limit:"
 msgid "Credit Limit"
-msgstr "Odobreni limit"
+msgstr "Kredi Limiti"
 
 msgctxt "field:party.party,credit_amount:"
 msgid "Credit Amount"
-msgstr "Odobreni limit"
+msgstr "Kredi Miktarı"
 
 msgctxt "field:party.party,credit_limit_amount:"
 msgid "Credit Limit Amount"
-msgstr "Znesek odobrenega limita"
+msgstr "Kredi Limit Miktarı"
 
 msgctxt "field:party.party,credit_limit_amounts:"
 msgid "Credit Limit Amounts"
-msgstr "Znesek odobrenega limita"
+msgstr "Kredi Limit Miktarları"
 
 msgctxt "field:party.party,credit_limit_digits:"
 msgid "Currency Digits"
-msgstr "Decimalke"
+msgstr "Para Birimi Basamakları"
 
 msgctxt "field:party.party.credit_limit_amount,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Şirket"
 
 msgctxt "field:party.party.credit_limit_amount,credit_limit_amount:"
 msgid "Credit Limit Amount"
-msgstr "Znesek odobrenega limita"
+msgstr "Kredi Limit Miktarı"
 
 msgctxt "field:party.party.credit_limit_amount,credit_limit_digits:"
 msgid "Currency Digits"
-msgstr "Decimalke"
+msgstr "Para Birimi Basamakları"
 
 msgctxt "field:party.party.credit_limit_amount,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr ""
 
 msgctxt "help:account.configuration,default_credit_limit_amount:"
 msgid "The default credit limit amount for new customers."
 msgstr ""
 
 msgctxt ""
 "help:account.configuration.default_credit_limit_amount,default_credit_limit_amount:"
 msgid "The default credit limit amount for new customers."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:account.dunning.level,credit_limit:"
 msgid "Has reached the credit limit."
-msgstr "Kreditni limit presežen."
+msgstr "Kredi limitine erişilmiştir"
 
 msgctxt "model:account.configuration.default_credit_limit_amount,name:"
 msgid "Account Configuration Default Credit Limit Amount"
-msgstr "Konfiguracija privzetega odobrenega limita"
+msgstr "Hesap Düzenleme Öntanımlı Kredi Limit Miktarı"
 
 msgctxt "model:ir.message,text:msg_party_credit_limit_amount"
 msgid "Party \"%(party)s\" has reached their credit limit of %(limit)s."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_credit_limit_dunning"
 msgid "Party \"%(party)s\" has reached the credit limit level of %(dunning)s."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:party.party.credit_limit_amount,name:"
 msgid "Party Credit Limit Amount"
-msgstr "Partnerjev odobreni limit"
+msgstr "Öntanımlı Kredi Limit Miktarı"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_credit_limit"
 msgid "Account Credit Limit"
 msgstr "Account Credit Limit"
 
 msgctxt "view:account.configuration:"
 msgid "Credit Limit"
-msgstr "Odobreni limit"
+msgstr "Kredi Limiti"
 
 msgctxt "view:party.party:"
 msgid "Credit Limit"
-msgstr "Odobreni limit"
+msgstr "Kredi Limiti"
```

### Comparing `trytond_account_credit_limit-7.0.0/locale/tr.po` & `trytond_account_credit_limit-7.2.0/locale/ro.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,103 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,default_credit_limit_amount:"
 msgid "Default Credit Limit Amount"
-msgstr "Öntanımlı Kredi Limit Miktarı"
+msgstr "Limita de Credit Implicita"
 
 msgctxt "field:account.configuration,default_credit_limit_amount_digits:"
 msgid "Currency Digits"
-msgstr "Para Birimi Basamakları"
+msgstr "Zecimale valută"
 
 msgctxt "field:account.configuration.default_credit_limit_amount,company:"
 msgid "Company"
-msgstr "Şirket"
+msgstr "Companie"
 
 msgctxt ""
 "field:account.configuration.default_credit_limit_amount,default_credit_limit_amount:"
 msgid "Default Credit Limit Amount"
-msgstr "Öntanımlı Kredi Limit Miktarı"
+msgstr "Valoarea Limita de Credit Implicita"
 
 msgctxt ""
 "field:account.configuration.default_credit_limit_amount,default_credit_limit_amount_digits:"
 msgid "Currency Digits"
-msgstr "Para Birimi Basamakları"
+msgstr "Zecimale valută"
 
 msgctxt "field:account.dunning.level,credit_limit:"
 msgid "Credit Limit"
-msgstr "Kredi Limiti"
+msgstr "Limita de credit"
 
 msgctxt "field:party.party,credit_amount:"
 msgid "Credit Amount"
-msgstr "Kredi Miktarı"
+msgstr "Suma de credit"
 
 msgctxt "field:party.party,credit_limit_amount:"
 msgid "Credit Limit Amount"
-msgstr "Kredi Limit Miktarı"
+msgstr "Suma Limita de Credit"
 
 msgctxt "field:party.party,credit_limit_amounts:"
 msgid "Credit Limit Amounts"
-msgstr "Kredi Limit Miktarları"
+msgstr "Sume Limita de Credit"
 
 msgctxt "field:party.party,credit_limit_digits:"
 msgid "Currency Digits"
-msgstr "Para Birimi Basamakları"
+msgstr "Zecimale valută"
 
 msgctxt "field:party.party.credit_limit_amount,company:"
 msgid "Company"
-msgstr "Şirket"
+msgstr "Companie"
 
 msgctxt "field:party.party.credit_limit_amount,credit_limit_amount:"
 msgid "Credit Limit Amount"
-msgstr "Kredi Limit Miktarı"
+msgstr "Suma Limita de Credit"
 
 msgctxt "field:party.party.credit_limit_amount,credit_limit_digits:"
 msgid "Currency Digits"
-msgstr "Para Birimi Basamakları"
+msgstr "Zecimale valută"
 
 msgctxt "field:party.party.credit_limit_amount,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "help:account.configuration,default_credit_limit_amount:"
 msgid "The default credit limit amount for new customers."
-msgstr ""
+msgstr "Suma limita de credit implicita pentru clienti noi."
 
 msgctxt ""
 "help:account.configuration.default_credit_limit_amount,default_credit_limit_amount:"
 msgid "The default credit limit amount for new customers."
-msgstr ""
+msgstr "Valoarea limita de credit implicita pentru clienti noi."
 
-#, fuzzy
 msgctxt "help:account.dunning.level,credit_limit:"
 msgid "Has reached the credit limit."
-msgstr "Kredi limitine erişilmiştir"
+msgstr "A atins limita de credit."
 
+#, fuzzy
 msgctxt "model:account.configuration.default_credit_limit_amount,name:"
 msgid "Account Configuration Default Credit Limit Amount"
-msgstr "Hesap Düzenleme Öntanımlı Kredi Limit Miktarı"
+msgstr "Limita de Credit Implicita a Configuratiei Contului"
 
 msgctxt "model:ir.message,text:msg_party_credit_limit_amount"
 msgid "Party \"%(party)s\" has reached their credit limit of %(limit)s."
-msgstr ""
+msgstr "Partea \"%(party)s\" a atins limita de credit de %(limit)s."
 
 msgctxt "model:ir.message,text:msg_party_credit_limit_dunning"
 msgid "Party \"%(party)s\" has reached the credit limit level of %(dunning)s."
-msgstr ""
+msgstr "Partea \"%(party)s\" a atins limita de credit %(dunning)s."
 
-#, fuzzy
 msgctxt "model:party.party.credit_limit_amount,name:"
 msgid "Party Credit Limit Amount"
-msgstr "Öntanımlı Kredi Limit Miktarı"
+msgstr "Suma Limita de Credit a Partii"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_credit_limit"
 msgid "Account Credit Limit"
-msgstr "Account Credit Limit"
+msgstr "Limita de Credit a Contului"
 
 msgctxt "view:account.configuration:"
 msgid "Credit Limit"
-msgstr "Kredi Limiti"
+msgstr "Limita de Credit"
 
 msgctxt "view:party.party:"
 msgid "Credit Limit"
-msgstr "Kredi Limiti"
+msgstr "Limita de Credit"
```

### Comparing `trytond_account_credit_limit-7.0.0/locale/uk.po` & `trytond_account_credit_limit-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/locale/zh_CN.po` & `trytond_account_credit_limit-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/message.xml` & `trytond_account_credit_limit-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/party.py` & `trytond_account_credit_limit-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/party.xml` & `trytond_account_credit_limit-7.2.0/party.xml`

 * *Files 24% similar despite different names*

#### Comparing `trytond_account_credit_limit-7.0.0/party.xml` & `trytond_account_credit_limit-7.2.0/party.xml`

```diff
@@ -5,19 +5,21 @@
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="model_field_access_credit_limit_amount">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'credit_limit_amount')]"/>
+      <field name="model">party.party</field>
+      <field name="field">credit_limit_amount</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="model_field_access_credit_limit_amount_group_credit_limit">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'credit_limit_amount')]"/>
+      <field name="model">party.party</field>
+      <field name="field">credit_limit_amount</field>
       <field name="group" ref="group_credit_limit"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_credit_limit-7.0.0/setup.py` & `trytond_account_credit_limit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/tests/test_module.py` & `trytond_account_credit_limit-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/tox.ini` & `trytond_account_credit_limit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/PKG-INFO` & `trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-credit-limit
-Version: 7.0.0
+Name: trytond_account_credit_limit
+Version: 7.2.0
 Summary: Tryton module for account credit limit
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
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_account_dunning<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_account_dunning<7.3,>=7.2; extra == "test"
 
 Account Credit Limit
 ####################
 
 The account_credit_limit module manages credit limit of parties. A "Credit
 Limit Amount" is added on Party. The module allows to check for a party:
```

### Comparing `trytond_account_credit_limit-7.0.0/trytond_account_credit_limit.egg-info/SOURCES.txt` & `trytond_account_credit_limit-7.2.0/trytond_account_credit_limit.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_credit_limit-7.0.0/view/party_form.xml` & `trytond_account_credit_limit-7.2.0/view/party_form.xml`

 * *Files identical despite different names*

