# Comparing `tmp/trytond_account_dunning-7.0.0.tar.gz` & `tmp/trytond_account_dunning-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning-7.0.0.tar", last modified: Mon Oct 30 17:19:22 2023, max compression
+gzip compressed data, was "trytond_account_dunning-7.2.0.tar", last modified: Mon Apr 29 15:32:34 2024, max compression
```

## Comparing `trytond_account_dunning-7.0.0.tar` & `trytond_account_dunning-7.2.0.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:22.115770 trytond_account_dunning-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:22:49.000000 trytond_account_dunning-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2045 2023-10-30 17:01:17.000000 trytond_account_dunning-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:01:16.000000 trytond_account_dunning-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3597 2023-10-30 17:19:22.115770 trytond_account_dunning-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-04-15 07:12:14.000000 trytond_account_dunning-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:22.112437 trytond_account_dunning-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:22:49.000000 trytond_account_dunning-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:49.000000 trytond_account_dunning-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    12757 2023-08-13 15:26:13.000000 trytond_account_dunning-7.0.0/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14406 2023-10-07 15:40:36.000000 trytond_account_dunning-7.0.0/dunning.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:22.109103 trytond_account_dunning-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7968 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6852 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7762 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8040 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7158 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7702 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8263 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6839 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7899 2023-10-30 16:47:45.000000 trytond_account_dunning-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8205 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6706 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8681 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6967 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7909 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6981 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7515 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6646 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7437 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7344 2023-10-30 16:47:45.000000 trytond_account_dunning-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7234 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6493 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2023-10-28 12:11:19.000000 trytond_account_dunning-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1176 2023-08-13 15:26:13.000000 trytond_account_dunning-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:19:22.115770 trytond_account_dunning-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4436 2023-10-27 17:38:49.000000 trytond_account_dunning-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:22.112437 trytond_account_dunning-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8206 2023-06-10 11:39:56.000000 trytond_account_dunning-7.0.0/tests/scenario_account_dunning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2972 2023-06-10 11:39:56.000000 trytond_account_dunning-7.0.0/tests/scenario_account_dunning_final.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:14.000000 trytond_account_dunning-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_dunning-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-10-30 17:01:14.000000 trytond_account_dunning-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:22.115770 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3597 2023-10-30 17:19:21.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2318 2023-10-30 17:19:22.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:19:21.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:19:21.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      136 2023-10-30 17:19:21.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:19:21.000000 trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:22.112437 trytond_account_dunning-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/view/dunning_create_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/view/dunning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_dunning-7.0.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/view/dunning_level_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/view/dunning_level_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/view/dunning_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/view/dunning_procedure_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/view/dunning_procedure_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_dunning-7.0.0/view/dunning_process_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-01-16 14:00:20.000000 trytond_account_dunning-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.351770 trytond_account_dunning-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2146 2024-04-29 15:13:22.000000 trytond_account_dunning-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:13:21.000000 trytond_account_dunning-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3597 2024-04-29 15:32:34.351770 trytond_account_dunning-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-04-15 07:12:14.000000 trytond_account_dunning-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      900 2024-04-27 16:30:39.000000 trytond_account_dunning-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.345104 trytond_account_dunning-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_dunning-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:52.000000 trytond_account_dunning-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    12757 2024-01-27 09:58:52.000000 trytond_account_dunning-7.2.0/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14153 2024-04-27 16:30:39.000000 trytond_account_dunning-7.2.0/dunning.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7436 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7968 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6852 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7762 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8040 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7158 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7702 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8263 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6839 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7899 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8205 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6706 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8681 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6967 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7909 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6981 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7515 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-29 13:17:17.000000 trytond_account_dunning-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7437 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7344 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7234 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6493 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-27 16:43:20.000000 trytond_account_dunning-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-22 12:14:36.000000 trytond_account_dunning-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:34.351770 trytond_account_dunning-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4436 2024-03-17 11:01:36.000000 trytond_account_dunning-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8257 2024-04-22 12:14:36.000000 trytond_account_dunning-7.2.0/tests/scenario_account_dunning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2950 2024-04-22 12:14:36.000000 trytond_account_dunning-7.2.0/tests/scenario_account_dunning_final.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:14.000000 trytond_account_dunning-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:52.000000 trytond_account_dunning-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-04-29 15:13:17.000000 trytond_account_dunning-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3597 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2300 2024-04-29 15:32:34.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      136 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:33.000000 trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:34.348437 trytond_account_dunning-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_create_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_dunning-7.2.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_level_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_level_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_procedure_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/dunning_procedure_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_dunning-7.2.0/view/dunning_process_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-01-16 14:00:20.000000 trytond_account_dunning-7.2.0/view/party_form.xml
```

### Comparing `trytond_account_dunning-7.0.0/CHANGELOG` & `trytond_account_dunning-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_dunning-7.0.0/COPYRIGHT` & `trytond_account_dunning-7.2.0/COPYRIGHT`

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

### Comparing `trytond_account_dunning-7.0.0/LICENSE` & `trytond_account_dunning-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/PKG-INFO` & `trytond_account_dunning-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for account dunning
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
@@ -49,20 +49,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Dunning Module
 ######################
 
 The account_dunning module adds dunning for receivable move lines.
 
 Procedure
```

### Comparing `trytond_account_dunning-7.0.0/README.rst` & `trytond_account_dunning-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/__init__.py` & `trytond_account_dunning-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/account.py` & `trytond_account_dunning-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/account.xml` & `trytond_account_dunning-7.2.0/account.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_account_dunning-7.0.0/account.xml` & `trytond_account_dunning-7.2.0/account.xml`

```diff
@@ -5,15 +5,15 @@
   <data>
     <record model="ir.ui.view" id="configuration_view_form">
       <field name="model">account.configuration</field>
       <field name="inherit" ref="account.configuration_view_form"/>
       <field name="name">configuration_form</field>
     </record>
     <record model="ir.model.access" id="access_move_line_dunning">
-      <field name="model" search="[('model', '=', 'account.move.line')]"/>
+      <field name="model">account.move.line</field>
       <field name="group" ref="group_dunning"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_account_dunning-7.0.0/doc/conf.py` & `trytond_account_dunning-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_dunning-7.0.0/doc/index.rst` & `trytond_account_dunning-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/dunning.py` & `trytond_account_dunning-7.2.0/dunning.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/dunning.xml` & `trytond_account_dunning-7.2.0/dunning.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_dunning-7.0.0/dunning.xml` & `trytond_account_dunning-7.2.0/dunning.xml`

```diff
@@ -34,30 +34,30 @@
     <record model="ir.action.act_window.view" id="act_dunning_procedure_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="dunning_procedure_view_form"/>
       <field name="act_window" ref="act_dunning_procedure_form"/>
     </record>
     <menuitem parent="menu_dunning_configuration" action="act_dunning_procedure_form" sequence="10" id="menu_dunning_procedure_form"/>
     <record model="ir.model.access" id="access_dunning_procedure">
-      <field name="model" search="[('model', '=', 'account.dunning.procedure')]"/>
+      <field name="model">account.dunning.procedure</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_dunning_procedure_account_admin">
-      <field name="model" search="[('model', '=', 'account.dunning.procedure')]"/>
+      <field name="model">account.dunning.procedure</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_dunning_procedure_dunning">
-      <field name="model" search="[('model', '=', 'account.dunning.procedure')]"/>
+      <field name="model">account.dunning.procedure</field>
       <field name="group" ref="group_dunning"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="dunning_level_view_form">
@@ -74,30 +74,30 @@
     <record model="ir.ui.view" id="dunning_level_view_list_sequence">
       <field name="model">account.dunning.level</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">dunning_level_list_sequence</field>
     </record>
     <record model="ir.model.access" id="access_dunning_level">
-      <field name="model" search="[('model', '=', 'account.dunning.level')]"/>
+      <field name="model">account.dunning.level</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_dunning_level_account_admin">
-      <field name="model" search="[('model', '=', 'account.dunning.level')]"/>
+      <field name="model">account.dunning.level</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_dunning_level_dunning">
-      <field name="model" search="[('model', '=', 'account.dunning.level')]"/>
+      <field name="model">account.dunning.level</field>
       <field name="group" ref="group_dunning"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="dunning_view_form">
@@ -174,48 +174,48 @@
     </record>
     <record model="ir.action-res.group" id="act_dunning_party-group_dunning">
       <field name="action" ref="act_dunning_party"/>
       <field name="group" ref="group_dunning"/>
     </record>
     <record model="ir.rule.group" id="rule_group_dunning_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.dunning')]"/>
+      <field name="model">account.dunning</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_dunning_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_dunning_companies"/>
     </record>
     <record model="ir.model.access" id="access_dunning">
-      <field name="model" search="[('model', '=', 'account.dunning')]"/>
+      <field name="model">account.dunning</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_dunning_account_admin">
-      <field name="model" search="[('model', '=', 'account.dunning')]"/>
+      <field name="model">account.dunning</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_dunning_dunning">
-      <field name="model" search="[('model', '=', 'account.dunning')]"/>
+      <field name="model">account.dunning</field>
       <field name="group" ref="group_dunning"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="dunning_reschedule_button">
+      <field name="model">account.dunning</field>
       <field name="name">reschedule</field>
       <field name="string">Reschedule</field>
-      <field name="model" search="[('model', '=', 'account.dunning')]"/>
     </record>
     <record model="ir.ui.view" id="dunning_create_start_view_form">
       <field name="model">account.dunning.create.start</field>
       <field name="type">form</field>
       <field name="name">dunning_create_start_form</field>
     </record>
     <record model="ir.action.wizard" id="wizard_dunning_create">
```

### Comparing `trytond_account_dunning-7.0.0/locale/bg.po` & `trytond_account_dunning-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/ca.po` & `trytond_account_dunning-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/cs.po` & `trytond_account_dunning-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/de.po` & `trytond_account_dunning-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/es.po` & `trytond_account_dunning-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/es_419.po` & `trytond_account_dunning-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/et.po` & `trytond_account_dunning-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/fa.po` & `trytond_account_dunning-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/fi.po` & `trytond_account_dunning-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/fr.po` & `trytond_account_dunning-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/hu.po` & `trytond_account_dunning-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/id.po` & `trytond_account_dunning-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/it.po` & `trytond_account_dunning-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/lo.po` & `trytond_account_dunning-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/lt.po` & `trytond_account_dunning-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/nl.po` & `trytond_account_dunning-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/pl.po` & `trytond_account_dunning-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/pt.po` & `trytond_account_dunning-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/ro.po` & `trytond_account_dunning-7.2.0/locale/uk.po`

 * *Files 3% similar despite different names*

```diff
@@ -17,69 +17,67 @@
 
 msgctxt "field:account.dunning,age:"
 msgid "Age"
 msgstr ""
 
 msgctxt "field:account.dunning,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.dunning,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
 msgctxt "field:account.dunning,blocked:"
 msgid "Blocked"
 msgstr ""
 
 msgctxt "field:account.dunning,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.dunning,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.dunning,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.dunning,level:"
 msgid "Level"
-msgstr "Nivel"
+msgstr ""
 
 msgctxt "field:account.dunning,line:"
 msgid "Line"
-msgstr "Rând"
+msgstr ""
 
 msgctxt "field:account.dunning,maturity_date:"
 msgid "Maturity Date"
-msgstr "Data scadenței"
+msgstr ""
 
 msgctxt "field:account.dunning,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.dunning,procedure:"
 msgid "Procedure"
-msgstr "Procedură"
+msgstr ""
 
 msgctxt "field:account.dunning,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda Secondara"
+msgstr ""
 
 msgctxt "field:account.dunning,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.dunning.create.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.dunning.level,overdue:"
 msgid "Overdue"
 msgstr ""
 
 msgctxt "field:account.dunning.level,procedure:"
 msgid "Procedure"
@@ -107,15 +105,15 @@
 
 msgctxt "field:party.party.dunning_procedure,dunning_procedure:"
 msgid "Dunning Procedure"
 msgstr ""
 
 msgctxt "field:party.party.dunning_procedure,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "help:account.configuration,default_dunning_procedure:"
 msgid "The default dunning procedure for new customers."
 msgstr ""
 
 msgctxt ""
 "help:account.configuration.default_dunning_procedure,default_dunning_procedure:"
@@ -182,18 +180,17 @@
 msgid "Dunnings"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_dunning_party"
 msgid "Dunnings"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_dunning_procedure_form"
 msgid "Procedures"
-msgstr "Procedură"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_reschedule_dunning_wizard"
 msgid "Reschedule Dunning"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_dunning_create"
 msgid "Create Dunnings"
@@ -240,18 +237,17 @@
 msgid "Create Dunnings"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_dunning_form"
 msgid "Dunnings"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_dunning_procedure_form"
 msgid "Procedures"
-msgstr "Procedură"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_dunnings"
 msgid "Dunnings"
 msgstr ""
 
 msgctxt "model:party.party.dunning_procedure,name:"
 msgid "Party Dunning Procedure"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_dunning-7.0.0/locale/ru.po` & `trytond_account_dunning-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/sl.po` & `trytond_account_dunning-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/tr.po` & `trytond_account_dunning-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/locale/uk.po` & `trytond_account_dunning-7.2.0/locale/zh_CN.po`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 msgstr ""
 
 msgctxt ""
 "field:account.configuration.default_dunning_procedure,default_dunning_procedure:"
 msgid "Default Dunning Procedure"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.dunning,active:"
 msgid "Active"
-msgstr ""
+msgstr "启用"
 
 msgctxt "field:account.dunning,age:"
 msgid "Age"
 msgstr ""
 
 msgctxt "field:account.dunning,amount:"
 msgid "Amount"
@@ -35,21 +36,23 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.dunning,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.dunning,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:account.dunning,level:"
 msgid "Level"
-msgstr ""
+msgstr "层级"
 
 msgctxt "field:account.dunning,line:"
 msgid "Line"
 msgstr ""
 
 msgctxt "field:account.dunning,maturity_date:"
 msgid "Maturity Date"
@@ -63,53 +66,61 @@
 msgid "Procedure"
 msgstr ""
 
 msgctxt "field:account.dunning,second_currency:"
 msgid "Second Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.dunning,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
+#, fuzzy
 msgctxt "field:account.dunning.create.start,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.dunning.level,overdue:"
 msgid "Overdue"
 msgstr ""
 
 msgctxt "field:account.dunning.level,procedure:"
 msgid "Procedure"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.dunning.procedure,levels:"
 msgid "Levels"
-msgstr ""
+msgstr "层级"
 
+#, fuzzy
 msgctxt "field:account.dunning.procedure,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
+#, fuzzy
 msgctxt "field:account.move.line,dunnings:"
 msgid "Dunnings"
-msgstr ""
+msgstr "Dunnings"
 
+#, fuzzy
 msgctxt "field:party.party,dunning_procedure:"
 msgid "Dunning Procedure"
-msgstr ""
+msgstr "Dunning Procedures"
 
+#, fuzzy
 msgctxt "field:party.party,dunning_procedures:"
 msgid "Dunning Procedures"
-msgstr ""
+msgstr "Dunning Procedures"
 
+#, fuzzy
 msgctxt "field:party.party.dunning_procedure,dunning_procedure:"
 msgid "Dunning Procedure"
-msgstr ""
+msgstr "Dunning Procedures"
 
 msgctxt "field:party.party.dunning_procedure,party:"
 msgid "Party"
 msgstr ""
 
 msgctxt "help:account.configuration,default_dunning_procedure:"
 msgid "The default dunning procedure for new customers."
@@ -174,43 +185,46 @@
 
 msgctxt "model:account.dunning.process.start,name:"
 msgid "Create Account Dunning"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_dunning_form"
 msgid "Dunnings"
-msgstr ""
+msgstr "Dunnings"
 
 msgctxt "model:ir.action,name:act_dunning_party"
 msgid "Dunnings"
-msgstr ""
+msgstr "Dunnings"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_dunning_procedure_form"
 msgid "Procedures"
-msgstr ""
+msgstr "Dunning Procedures"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reschedule_dunning_wizard"
 msgid "Reschedule Dunning"
-msgstr ""
+msgstr "Create Dunnings"
 
 msgctxt "model:ir.action,name:wizard_dunning_create"
 msgid "Create Dunnings"
-msgstr ""
+msgstr "Create Dunnings"
 
 msgctxt "model:ir.action,name:wizard_dunning_process"
 msgid "Process Dunning"
-msgstr ""
+msgstr "Process Dunning"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_dunning_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "全部"
 
 msgctxt "model:ir.action.act_window.domain,name:act_dunning_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.action.act_window.domain,name:act_dunning_form_domain_final"
 msgid "Final"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_dunning_form_domain_waiting"
@@ -227,76 +241,83 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_dunning_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_dunning_configuration"
 msgid "Dunnings"
-msgstr ""
+msgstr "Dunnings"
 
 msgctxt "model:ir.ui.menu,name:menu_dunning_create"
 msgid "Create Dunnings"
-msgstr ""
+msgstr "Create Dunnings"
 
 msgctxt "model:ir.ui.menu,name:menu_dunning_form"
 msgid "Dunnings"
-msgstr ""
+msgstr "Dunnings"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_dunning_procedure_form"
 msgid "Procedures"
-msgstr ""
+msgstr "Dunning Procedures"
 
 msgctxt "model:ir.ui.menu,name:menu_dunnings"
 msgid "Dunnings"
-msgstr ""
+msgstr "Dunnings"
 
 msgctxt "model:party.party.dunning_procedure,name:"
 msgid "Party Dunning Procedure"
 msgstr ""
 
 msgctxt "model:res.group,name:group_dunning"
 msgid "Dunning"
-msgstr ""
+msgstr "Dunning"
 
+#, fuzzy
 msgctxt "selection:account.dunning,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "selection:account.dunning,state:"
 msgid "Final"
 msgstr ""
 
 msgctxt "selection:account.dunning,state:"
 msgid "Waiting"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Dunning"
-msgstr ""
+msgstr "Dunning"
 
 msgctxt "view:account.dunning.create.start:"
 msgid "Create Dunning for date"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.dunning.process.start:"
 msgid "Process Dunning?"
-msgstr ""
+msgstr "Process Dunning"
 
+#, fuzzy
 msgctxt "view:party.party:"
 msgid "Dunning"
-msgstr ""
+msgstr "Dunning"
 
 msgctxt "wizard_button:account.dunning.create,start,create_:"
 msgid "Create"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:account.dunning.create,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:account.dunning.process,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 msgctxt "wizard_button:account.dunning.process,start,process:"
 msgid "Process"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_dunning-7.0.0/party.py` & `trytond_account_dunning-7.2.0/party.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.model import ModelSQL, ValueMixin, fields
 from trytond.pool import Pool, PoolMeta
 
 dunning_procedure = fields.Many2One(
-    'account.dunning.procedure', "Dunning Procedure")
+    'account.dunning.procedure', "Dunning Procedure", ondelete='RESTRICT')
 
 
 class Party(metaclass=PoolMeta):
     __name__ = 'party.party'
     dunning_procedure = fields.MultiValue(dunning_procedure)
     dunning_procedures = fields.One2Many(
         'party.party.dunning_procedure', 'party', "Dunning Procedures")
```

### Comparing `trytond_account_dunning-7.0.0/setup.py` & `trytond_account_dunning-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/tests/scenario_account_dunning.rst` & `trytond_account_dunning-7.2.0/tests/scenario_account_dunning.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 ========================
 Account Dunning Scenario
 ========================
 
 Imports::
 
     >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
+    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import (
+    ...     activate_modules, assertEqual, assertTrue, set_user)
+
     >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning')
 
 Create company::
@@ -161,38 +164,32 @@
 
 Create dunnings on 5 days::
 
     >>> create_dunning = Wizard('account.dunning.create')
     >>> create_dunning.form.date = period.start_date + relativedelta(days=5)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
-    >>> dunning.procedure == procedure
-    True
-    >>> dunning.level == procedure.levels[0]
-    True
+    >>> assertEqual(dunning.procedure, procedure)
+    >>> assertEqual(dunning.level, procedure.levels[0])
     >>> dunning.state
     'draft'
-    >>> dunning.line == dunning_line
-    True
+    >>> assertEqual(dunning.line, dunning_line)
 
 Create dunnings on 30 days with draft dunning::
 
     >>> create_dunning = Wizard('account.dunning.create')
     >>> create_dunning.form.date = period.start_date + relativedelta(days=30)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
-    >>> dunning.procedure == procedure
-    True
-    >>> dunning.level == procedure.levels[0]
-    True
+    >>> assertEqual(dunning.procedure, procedure)
+    >>> assertEqual(dunning.level, procedure.levels[0])
     >>> dunning.state
     'draft'
     >>> dunning.date
-    >>> dunning.line == dunning_line
-    True
+    >>> assertEqual(dunning.line, dunning_line)
 
 Process dunning::
 
     >>> process_dunning = Wizard('account.dunning.process',
     ...     [dunning])
     >>> process_dunning.execute('process')
     >>> dunning.reload()
@@ -205,42 +202,35 @@
 
     >>> dunning.blocked = True
     >>> dunning.save()
     >>> create_dunning = Wizard('account.dunning.create')
     >>> create_dunning.form.date = period.start_date + relativedelta(days=30)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
-    >>> dunning.procedure == procedure
-    True
-    >>> dunning.level == procedure.levels[0]
-    True
+    >>> assertEqual(dunning.procedure, procedure)
+    >>> assertEqual(dunning.level, procedure.levels[0])
     >>> dunning.state
     'waiting'
-    >>> dunning.line == dunning_line
-    True
-    >>> bool(dunning.blocked)
-    True
+    >>> assertEqual(dunning.line, dunning_line)
+    >>> assertTrue(dunning.blocked)
     >>> dunning.blocked = False
     >>> dunning.save()
 
 Create dunnings on 30 days::
 
     >>> create_dunning = Wizard('account.dunning.create')
     >>> create_dunning.form.date = period.start_date + relativedelta(days=30)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
-    >>> dunning.procedure == procedure
-    True
-    >>> dunning.level == procedure.levels[1]
-    True
+    >>> assertEqual(dunning.procedure, procedure)
+    >>> assertEqual(dunning.level, procedure.levels[1])
     >>> dunning.state
     'draft'
     >>> dunning.date
-    >>> dunning.line == dunning_line
-    True
+    >>> assertEqual(dunning.line, dunning_line)
 
 Pay dunning::
 
     >>> set_user(account_user)
     >>> MoveLine = Model.get('account.move.line')
     >>> move = Move()
     >>> move.period = period
```

### Comparing `trytond_account_dunning-7.0.0/tests/scenario_account_dunning_final.rst` & `trytond_account_dunning-7.2.0/tests/scenario_account_dunning_final.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Account Dunning Final Scenario
 ==============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning')
 
 Create company::
```

### Comparing `trytond_account_dunning-7.0.0/tox.ini` & `trytond_account_dunning-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/PKG-INFO` & `trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-dunning
-Version: 7.0.0
+Name: trytond_account_dunning
+Version: 7.2.0
 Summary: Tryton module for account dunning
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
@@ -49,20 +49,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Dunning Module
 ######################
 
 The account_dunning module adds dunning for receivable move lines.
 
 Procedure
```

### Comparing `trytond_account_dunning-7.0.0/trytond_account_dunning.egg-info/SOURCES.txt` & `trytond_account_dunning-7.2.0/trytond_account_dunning.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_dunning-7.0.0/view/dunning_form.xml` & `trytond_account_dunning-7.2.0/view/dunning_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-7.0.0/view/dunning_list.xml` & `trytond_account_dunning-7.2.0/view/dunning_list.xml`

 * *Files identical despite different names*

