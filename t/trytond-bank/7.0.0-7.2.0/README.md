# Comparing `tmp/trytond_bank-7.0.0.tar.gz` & `tmp/trytond_bank-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_bank-7.0.0.tar", last modified: Mon Oct 30 17:27:32 2023, max compression
+gzip compressed data, was "trytond_bank-7.2.0.tar", last modified: Mon Apr 29 15:38:29 2024, max compression
```

## Comparing `trytond_bank-7.0.0.tar` & `trytond_bank-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.991444 trytond_bank-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-10-22 17:23:00.000000 trytond_bank-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2336 2023-10-30 17:05:06.000000 trytond_bank-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:05:05.000000 trytond_bank-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2023-10-30 17:27:32.991444 trytond_bank-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10615 2023-10-07 15:40:36.000000 trytond_bank-7.0.0/bank.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/bank.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.988111 trytond_bank-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2805 2023-10-22 17:23:00.000000 trytond_bank-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:00.000000 trytond_bank-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.988111 trytond_bank-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/icons/tryton-bank.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.984778 trytond_bank-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3294 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3503 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3518 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3533 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2942 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3337 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3675 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3553 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3108 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3525 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3904 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3513 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3372 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3498 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3464 2023-10-30 16:47:45.000000 trytond_bank-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3536 2023-10-30 16:47:45.000000 trytond_bank-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2881 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3026 2023-10-28 12:11:21.000000 trytond_bank-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1530 2023-08-13 15:26:13.000000 trytond_bank-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1368 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:27:32.991444 trytond_bank-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4361 2023-10-27 17:38:49.000000 trytond_bank-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.988111 trytond_bank-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7283 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_bank-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2023-10-30 17:05:02.000000 trytond_bank-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.991444 trytond_bank-7.0.0/trytond_bank.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2023-10-30 17:27:32.000000 trytond_bank-7.0.0/trytond_bank.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1865 2023-10-30 17:27:32.000000 trytond_bank-7.0.0/trytond_bank.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:27:32.000000 trytond_bank-7.0.0/trytond_bank.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2023-10-30 17:27:32.000000 trytond_bank-7.0.0/trytond_bank.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_bank-7.0.0/trytond_bank.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-10-30 17:27:32.000000 trytond_bank-7.0.0/trytond_bank.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:27:32.000000 trytond_bank-7.0.0/trytond_bank.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:32.988111 trytond_bank-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/view/bank_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/view/bank_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-08-13 15:26:13.000000 trytond_bank-7.0.0/view/bank_account_number_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/view/bank_account_number_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/view/bank_account_number_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/view/bank_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:15.000000 trytond_bank-7.0.0/view/bank_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_bank-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2437 2024-04-29 15:18:15.000000 trytond_bank-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:18:14.000000 trytond_bank-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10477 2024-03-17 11:01:36.000000 trytond_bank-7.2.0/bank.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5803 2024-04-27 16:30:39.000000 trytond_bank-7.2.0/bank.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.212489 trytond_bank-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-27 16:30:39.000000 trytond_bank-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:05.000000 trytond_bank-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.212489 trytond_bank-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/icons/tryton-bank.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.215822 trytond_bank-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3294 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3503 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3518 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3533 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2942 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3337 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3675 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3553 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3108 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3904 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3513 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3498 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3464 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3536 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3026 2024-04-27 16:43:22.000000 trytond_bank-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1530 2024-01-27 09:58:52.000000 trytond_bank-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2024-04-27 16:30:39.000000 trytond_bank-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4361 2024-03-17 11:01:36.000000 trytond_bank-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.215822 trytond_bank-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7283 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:05.000000 trytond_bank-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2024-04-29 15:18:10.000000 trytond_bank-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/trytond_bank.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1847 2024-04-29 15:38:29.000000 trytond_bank-7.2.0/trytond_bank.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_bank-7.2.0/trytond_bank.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:28.000000 trytond_bank-7.2.0/trytond_bank.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:29.219156 trytond_bank-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/view/bank_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-01-27 09:58:52.000000 trytond_bank-7.2.0/view/bank_account_number_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_account_number_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_account_number_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/view/bank_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:15.000000 trytond_bank-7.2.0/view/bank_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_bank-7.2.0/view/party_form.xml
```

### Comparing `trytond_bank-7.0.0/CHANGELOG` & `trytond_bank-7.2.0/CHANGELOG`

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

### Comparing `trytond_bank-7.0.0/COPYRIGHT` & `trytond_bank-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2013-2023 Cédric Krier.
-Copyright (C) 2013-2023 B2CK SPRL.
+Copyright (C) 2013-2024 Cédric Krier.
+Copyright (C) 2013-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_bank-7.0.0/LICENSE` & `trytond_bank-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/PKG-INFO` & `trytond_bank-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_bank
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with banks
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
@@ -50,17 +50,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-stdnum
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: swift
 Requires-Dist: schwifty>=2020.01.0; extra == "swift"
 Provides-Extra: test
 Requires-Dist: schwifty; extra == "test"
 
 Bank Module
 ###########
```

### Comparing `trytond_bank-7.0.0/README.rst` & `trytond_bank-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/bank.py` & `trytond_bank-7.2.0/bank.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,27 +196,36 @@
     @classmethod
     def __setup__(cls):
         cls.number.search_unaccented = False
         cls.number_compact.search_unaccented = False
         super().__setup__()
         table = cls.__table__()
         cls._sql_constraints += [
-            ('number_iban_exclude',
+            ('number_iban_active_exclude',
                 Exclude(table, (table.number_compact, Equal),
-                    where=table.type == 'iban'),
+                    where=(table.type == 'iban') & table.active),
                 'bank.msg_number_iban_unique'),
-            ('account_iban_exclude',
+            ('account_iban_active_exclude',
                 Exclude(table, (table.account, Equal),
-                    where=table.type == 'iban'),
+                    where=(table.type == 'iban') & table.active),
                 'bank.msg_account_iban_unique'),
             ]
         cls.__access__.add('account')
         cls._order.insert(0, ('account', 'ASC'))
 
     @classmethod
+    def __register__(cls, module):
+        table_h = cls.__table_handler__(module)
+        super().__register__(module)
+
+        # Migration from 7.0: replace iban exclude
+        table_h.drop_constraint('number_iban_exclude')
+        table_h.drop_constraint('account_iban_exclude')
+
+    @classmethod
     def default_type(cls):
         return 'iban'
 
     @classmethod
     def domain_number(cls, domain, tables):
         table, _ = tables[None]
         name, operator, value = domain
@@ -240,28 +249,14 @@
 
     @property
     def compact_iban(self):
         return (iban.compact(self.number) if self.type == 'iban'
             else self.number)
 
     @classmethod
-    def search_rec_name(cls, name, clause):
-        _, operator, operand, *extra = clause
-        if operator.startswith('!') or operator.startswith('not '):
-            bool_op = 'AND'
-        else:
-            bool_op = 'OR'
-        number_value = operand
-        if operator.endswith('like') and is_full_text(operand):
-            number_value = lstrip_wildcard(operand)
-        return [bool_op,
-            ('number', operator, number_value, *extra),
-            ]
-
-    @classmethod
     def create(cls, vlist):
         vlist = [v.copy() for v in vlist]
         for values in vlist:
             if values.get('type') == 'iban' and 'number' in values:
                 values['number'] = iban.format(values['number'])
                 values['number_compact'] = iban.compact(values['number'])
         return super().create(vlist)
```

### Comparing `trytond_bank-7.0.0/bank.xml` & `trytond_bank-7.2.0/bank.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_bank-7.0.0/bank.xml` & `trytond_bank-7.2.0/bank.xml`

```diff
@@ -37,22 +37,22 @@
     <record model="ir.action.act_window.view" id="act_bank_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="bank_view_form"/>
       <field name="act_window" ref="act_bank_form"/>
     </record>
     <menuitem parent="menu_banking" action="act_bank_form" sequence="10" id="menu_bank_form"/>
     <record model="ir.model.access" id="access_bank">
-      <field name="model" search="[('model', '=', 'bank')]"/>
+      <field name="model">bank</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_bank_bank_admin">
-      <field name="model" search="[('model', '=', 'bank')]"/>
+      <field name="model">bank</field>
       <field name="group" ref="group_bank_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="bank_account_view_form">
@@ -77,22 +77,22 @@
     <record model="ir.action.act_window.view" id="act_bank_account_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="bank_account_view_form"/>
       <field name="act_window" ref="act_bank_account_form"/>
     </record>
     <menuitem parent="menu_banking" action="act_bank_account_form" sequence="20" id="menu_bank_account_form"/>
     <record model="ir.model.access" id="access_account">
-      <field name="model" search="[('model', '=', 'bank.account')]"/>
+      <field name="model">bank.account</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_bank_admin">
-      <field name="model" search="[('model', '=', 'bank.account')]"/>
+      <field name="model">bank.account</field>
       <field name="group" ref="group_bank_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="bank_account_number_view_form">
```

### Comparing `trytond_bank-7.0.0/doc/conf.py` & `trytond_bank-7.2.0/doc/conf.py`

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

### Comparing `trytond_bank-7.0.0/doc/index.rst` & `trytond_bank-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/icons/LICENSE` & `trytond_bank-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/bg.po` & `trytond_bank-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/ca.po` & `trytond_bank-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/cs.po` & `trytond_bank-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/de.po` & `trytond_bank-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/es.po` & `trytond_bank-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/es_419.po` & `trytond_bank-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/et.po` & `trytond_bank-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/fa.po` & `trytond_bank-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/fi.po` & `trytond_bank-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/fr.po` & `trytond_bank-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/hu.po` & `trytond_bank-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/id.po` & `trytond_bank-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/it.po` & `trytond_bank-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/lo.po` & `trytond_bank-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/lt.po` & `trytond_bank-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/nl.po` & `trytond_bank-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/pl.po` & `trytond_bank-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/pt.po` & `trytond_bank-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/ro.po` & `trytond_bank-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/ru.po` & `trytond_bank-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/sl.po` & `trytond_bank-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/tr.po` & `trytond_bank-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/uk.po` & `trytond_bank-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/locale/zh_CN.po` & `trytond_bank-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/message.xml` & `trytond_bank-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/party.py` & `trytond_bank-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/setup.py` & `trytond_bank-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/tests/test_module.py` & `trytond_bank-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/tox.ini` & `trytond_bank-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/trytond_bank.egg-info/PKG-INFO` & `trytond_bank-7.2.0/trytond_bank.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-bank
-Version: 7.0.0
+Name: trytond_bank
+Version: 7.2.0
 Summary: Tryton module with banks
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
@@ -50,17 +50,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-stdnum
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: swift
 Requires-Dist: schwifty>=2020.01.0; extra == "swift"
 Provides-Extra: test
 Requires-Dist: schwifty; extra == "test"
 
 Bank Module
 ###########
```

### Comparing `trytond_bank-7.0.0/trytond_bank.egg-info/SOURCES.txt` & `trytond_bank-7.2.0/trytond_bank.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 bank.py
```

### Comparing `trytond_bank-7.0.0/view/bank_account_form.xml` & `trytond_bank-7.2.0/view/bank_account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-7.0.0/view/bank_account_number_form.xml` & `trytond_bank-7.2.0/view/bank_account_number_form.xml`

 * *Files identical despite different names*

