# Comparing `tmp/trytond_account_dunning_fee-7.0.0.tar.gz` & `tmp/trytond_account_dunning_fee-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning_fee-7.0.0.tar", last modified: Mon Oct 30 17:19:39 2023, max compression
+gzip compressed data, was "trytond_account_dunning_fee-7.2.0.tar", last modified: Mon Apr 29 15:32:46 2024, max compression
```

## Comparing `trytond_account_dunning_fee-7.0.0.tar` & `trytond_account_dunning_fee-7.2.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:39.179185 trytond_account_dunning_fee-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-22 17:22:49.000000 trytond_account_dunning_fee-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1367 2023-10-30 17:01:24.000000 trytond_account_dunning_fee-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:01:24.000000 trytond_account_dunning_fee-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3196 2023-10-30 17:19:39.179185 trytond_account_dunning_fee-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:14.000000 trytond_account_dunning_fee-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:39.175851 trytond_account_dunning_fee-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-22 17:22:49.000000 trytond_account_dunning_fee-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:49.000000 trytond_account_dunning_fee-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     6783 2023-08-13 15:26:13.000000 trytond_account_dunning_fee-7.0.0/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6128 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/dunning.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:39.172518 trytond_account_dunning_fee-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1929 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2059 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1947 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1846 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2687 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1813 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2113 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1917 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2081 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2072 2023-10-30 16:47:45.000000 trytond_account_dunning_fee-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2117 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1859 2023-10-28 12:11:19.000000 trytond_account_dunning_fee-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:19:39.179185 trytond_account_dunning_fee-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4443 2023-10-27 17:38:49.000000 trytond_account_dunning_fee-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:39.175851 trytond_account_dunning_fee-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4956 2023-06-10 11:39:56.000000 trytond_account_dunning_fee-7.0.0/tests/scenario_account_dunning_fee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_dunning_fee-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_dunning_fee-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:01:21.000000 trytond_account_dunning_fee-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:39.179185 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3196 2023-10-30 17:19:38.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1974 2023-10-30 17:19:39.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:19:38.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:19:38.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-10-30 17:19:38.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:19:38.000000 trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:39.175851 trytond_account_dunning_fee-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/view/dunning_fee_dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.0.0/view/dunning_fee_dunning_level_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-07 15:40:36.000000 trytond_account_dunning_fee-7.0.0/view/dunning_fee_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-08-05 19:39:37.000000 trytond_account_dunning_fee-7.0.0/view/dunning_fee_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.0.0/view/dunning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.0.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.0.0/view/dunning_level_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1468 2024-04-29 15:13:31.000000 trytond_account_dunning_fee-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:13:31.000000 trytond_account_dunning_fee-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3196 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:14.000000 trytond_account_dunning_fee-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:46.844777 trytond_account_dunning_fee-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_account_dunning_fee-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:52.000000 trytond_account_dunning_fee-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6783 2024-01-27 09:58:52.000000 trytond_account_dunning_fee-7.2.0/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5926 2024-04-27 16:30:39.000000 trytond_account_dunning_fee-7.2.0/dunning.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2082 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2097 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1929 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2059 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1947 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1846 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2091 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2687 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1813 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2113 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1834 2024-04-29 13:17:17.000000 trytond_account_dunning_fee-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2081 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2072 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2117 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1859 2024-04-27 16:43:20.000000 trytond_account_dunning_fee-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4443 2024-03-17 11:01:36.000000 trytond_account_dunning_fee-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4935 2024-04-22 12:14:36.000000 trytond_account_dunning_fee-7.2.0/tests/scenario_account_dunning_fee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_dunning_fee-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:52.000000 trytond_account_dunning_fee-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-29 15:13:27.000000 trytond_account_dunning_fee-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3196 2024-04-29 15:32:46.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2024-04-29 15:32:46.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:46.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:32:46.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-04-29 15:32:46.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:46.000000 trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:46.848110 trytond_account_dunning_fee-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/view/dunning_fee_dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-7.2.0/view/dunning_fee_dunning_level_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2024-02-04 18:51:26.000000 trytond_account_dunning_fee-7.2.0/view/dunning_fee_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-08-05 19:39:37.000000 trytond_account_dunning_fee-7.2.0/view/dunning_fee_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.2.0/view/dunning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.2.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-7.2.0/view/dunning_level_list.xml
```

### Comparing `trytond_account_dunning_fee-7.0.0/CHANGELOG` & `trytond_account_dunning_fee-7.2.0/CHANGELOG`

 * *Files 18% similar despite different names*

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

### Comparing `trytond_account_dunning_fee-7.0.0/COPYRIGHT` & `trytond_account_dunning_fee-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2016-2023 Cédric Krier
-Copyright (C) 2016-2023 B2CK
+Copyright (C) 2016-2024 Cédric Krier
+Copyright (C) 2016-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_dunning_fee-7.0.0/LICENSE` & `trytond_account_dunning_fee-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/PKG-INFO` & `trytond_account_dunning_fee-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning_fee
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for account dunning fee
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
@@ -46,20 +46,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_dunning<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_dunning<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_dunning_letter<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_dunning_letter<7.3,>=7.2; extra == "test"
 
 Account Dunning Fee Module
 ##########################
 
 The account_dunning_fee module allows to generate accounting moves as fees when
 processing dunning which are at a level with a *Fee* defined.
```

### Comparing `trytond_account_dunning_fee-7.0.0/README.rst` & `trytond_account_dunning_fee-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/__init__.py` & `trytond_account_dunning_fee-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/doc/conf.py` & `trytond_account_dunning_fee-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_dunning_fee-7.0.0/doc/index.rst` & `trytond_account_dunning_fee-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/dunning.py` & `trytond_account_dunning_fee-7.2.0/dunning.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/dunning.xml` & `trytond_account_dunning_fee-7.2.0/dunning.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account_dunning_fee-7.0.0/dunning.xml` & `trytond_account_dunning_fee-7.2.0/dunning.xml`

```diff
@@ -25,30 +25,30 @@
     <record model="ir.action.act_window.view" id="act_dunning_fee_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="dunning_fee_view_form"/>
       <field name="act_window" ref="act_dunning_fee_form"/>
     </record>
     <menuitem parent="account_dunning.menu_dunning_configuration" action="act_dunning_fee_form" sequence="20" id="menu_dunning_fee_form"/>
     <record model="ir.model.access" id="access_dunning_fee">
-      <field name="model" search="[('model', '=', 'account.dunning.fee')]"/>
+      <field name="model">account.dunning.fee</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_dunning_fee_account_admin">
-      <field name="model" search="[('model', '=', 'account.dunning.fee')]"/>
+      <field name="model">account.dunning.fee</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_dunning_fee_dunning">
-      <field name="model" search="[('model', '=', 'account.dunning.fee')]"/>
+      <field name="model">account.dunning.fee</field>
       <field name="group" ref="account_dunning.group_dunning"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="dunning_level_view_form">
@@ -78,30 +78,30 @@
     </record>
     <record model="ir.ui.view" id="dunning_fee_dunning_level_view_list">
       <field name="model">account.dunning.fee.dunning_level</field>
       <field name="type">tree</field>
       <field name="name">dunning_fee_dunning_level_list</field>
     </record>
     <record model="ir.model.access" id="access_dunning_fee_dunning_level">
-      <field name="model" search="[('model', '=', 'account.dunning.fee.dunning_level')]"/>
+      <field name="model">account.dunning.fee.dunning_level</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_dunning_fee_dunning_level_account_admin">
-      <field name="model" search="[('model', '=', 'account.dunning.fee.dunning_level')]"/>
+      <field name="model">account.dunning.fee.dunning_level</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_dunning_fee_dunning_level_dunning">
-      <field name="model" search="[('model', '=', 'account.dunning.fee.dunning_level')]"/>
+      <field name="model">account.dunning.fee.dunning_level</field>
       <field name="group" ref="account_dunning.group_dunning"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_account_dunning_fee-7.0.0/locale/bg.po` & `trytond_account_dunning_fee-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/ca.po` & `trytond_account_dunning_fee-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/cs.po` & `trytond_account_dunning_fee-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/de.po` & `trytond_account_dunning_fee-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/es.po` & `trytond_account_dunning_fee-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/es_419.po` & `trytond_account_dunning_fee-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/et.po` & `trytond_account_dunning_fee-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/fa.po` & `trytond_account_dunning_fee-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/fi.po` & `trytond_account_dunning_fee-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/fr.po` & `trytond_account_dunning_fee-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/hu.po` & `trytond_account_dunning_fee-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/id.po` & `trytond_account_dunning_fee-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/it.po` & `trytond_account_dunning_fee-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/lo.po` & `trytond_account_dunning_fee-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/lt.po` & `trytond_account_dunning_fee-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/nl.po` & `trytond_account_dunning_fee-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/pl.po` & `trytond_account_dunning_fee-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/pt.po` & `trytond_account_dunning_fee-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/ro.po` & `trytond_account_dunning_fee-7.2.0/locale/ro.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 msgctxt "field:account.dunning,fees:"
 msgid "Fees"
 msgstr ""
 
 msgctxt "field:account.dunning.fee,compute_method:"
 msgid "Compute Method"
-msgstr ""
+msgstr "Metoda de Calcul"
 
 msgctxt "field:account.dunning.fee,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "field:account.dunning.fee,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nume"
 
 msgctxt "field:account.dunning.fee,percentage:"
 msgid "Percentage"
-msgstr ""
+msgstr "Procentaj"
 
 msgctxt "field:account.dunning.fee,product:"
 msgid "Product"
 msgstr "Produs"
 
 msgctxt "field:account.dunning.fee.dunning_level,amount:"
 msgid "Amount"
```

### Comparing `trytond_account_dunning_fee-7.0.0/locale/ru.po` & `trytond_account_dunning_fee-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/sl.po` & `trytond_account_dunning_fee-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/tr.po` & `trytond_account_dunning_fee-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/uk.po` & `trytond_account_dunning_fee-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/locale/zh_CN.po` & `trytond_account_dunning_fee-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/setup.py` & `trytond_account_dunning_fee-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/tests/scenario_account_dunning_fee.rst` & `trytond_account_dunning_fee-7.2.0/tests/scenario_account_dunning_fee.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Account Dunning Fee Scenario
 ============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import config, Model, Wizard
+
+    >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning_fee')
 
 Create company::
 
@@ -103,15 +103,15 @@
 Create move::
 
     >>> Move = Model.get('account.move')
     >>> move = Move()
     >>> move.period = period
     >>> move.journal = journal_revenue
     >>> move.date = period.start_date
-    >>> line  = move.lines.new()
+    >>> line = move.lines.new()
     >>> line.account = revenue
     >>> line.credit = Decimal(100)
     >>> line = move.lines.new()
     >>> line.account = receivable
     >>> line.debit = Decimal(100)
     >>> line.party = customer
     >>> line.maturity_date = period.start_date
```

### Comparing `trytond_account_dunning_fee-7.0.0/tox.ini` & `trytond_account_dunning_fee-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/PKG-INFO` & `trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-dunning-fee
-Version: 7.0.0
+Name: trytond_account_dunning_fee
+Version: 7.2.0
 Summary: Tryton module for account dunning fee
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
@@ -46,20 +46,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_dunning<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_dunning<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_dunning_letter<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_dunning_letter<7.3,>=7.2; extra == "test"
 
 Account Dunning Fee Module
 ##########################
 
 The account_dunning_fee module allows to generate accounting moves as fees when
 processing dunning which are at a level with a *Fee* defined.
```

### Comparing `trytond_account_dunning_fee-7.0.0/trytond_account_dunning_fee.egg-info/SOURCES.txt` & `trytond_account_dunning_fee-7.2.0/trytond_account_dunning_fee.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_dunning_fee-7.0.0/view/dunning_fee_form.xml` & `trytond_account_dunning_fee-7.2.0/view/dunning_fee_form.xml`

 * *Files identical despite different names*

