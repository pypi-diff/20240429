# Comparing `tmp/trytond_account_dunning_email-7.0.0.tar.gz` & `tmp/trytond_account_dunning_email-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning_email-7.0.0.tar", last modified: Mon Oct 30 17:19:31 2023, max compression
+gzip compressed data, was "trytond_account_dunning_email-7.2.0.tar", last modified: Mon Apr 29 15:32:40 2024, max compression
```

## Comparing `trytond_account_dunning_email-7.0.0.tar` & `trytond_account_dunning_email-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:31.162480 trytond_account_dunning_email-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:22:49.000000 trytond_account_dunning_email-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-10-30 17:01:21.000000 trytond_account_dunning_email-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:01:20.000000 trytond_account_dunning_email-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2724 2023-10-30 17:19:31.159146 trytond_account_dunning_email-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      604 2023-10-07 15:40:36.000000 trytond_account_dunning_email-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6130 2023-10-07 15:40:36.000000 trytond_account_dunning_email-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1803 2023-10-07 15:40:36.000000 trytond_account_dunning_email-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:31.159146 trytond_account_dunning_email-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:22:49.000000 trytond_account_dunning_email-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:49.000000 trytond_account_dunning_email-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3366 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.0.0/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)     2042 2023-10-07 15:40:36.000000 trytond_account_dunning_email-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:31.155813 trytond_account_dunning_email-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2287 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2178 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2374 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2181 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2288 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1803 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2207 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2225 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1835 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1983 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1851 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2023-10-30 16:47:45.000000 trytond_account_dunning_email-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:19:31.162480 trytond_account_dunning_email-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4383 2023-10-27 17:38:49.000000 trytond_account_dunning_email-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:31.155813 trytond_account_dunning_email-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3664 2023-10-07 15:40:36.000000 trytond_account_dunning_email-7.0.0/tests/scenario_account_dunning_email.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_dunning_email-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_dunning_email-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      117 2023-10-30 17:01:17.000000 trytond_account_dunning_email-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:31.159146 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2724 2023-10-30 17:19:30.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-10-30 17:19:31.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:19:30.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:19:30.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-30 17:19:30.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:19:30.000000 trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:31.155813 trytond_account_dunning_email-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.0.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.0.0/view/dunning_level_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:40.788269 trytond_account_dunning_email-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1448 2024-04-29 15:13:26.000000 trytond_account_dunning_email-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:13:26.000000 trytond_account_dunning_email-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2724 2024-04-29 15:32:40.788269 trytond_account_dunning_email-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      604 2024-02-04 18:51:26.000000 trytond_account_dunning_email-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5452 2024-04-27 16:30:39.000000 trytond_account_dunning_email-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1803 2024-02-04 18:51:26.000000 trytond_account_dunning_email-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:40.784935 trytond_account_dunning_email-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_account_dunning_email-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:52.000000 trytond_account_dunning_email-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3376 2024-04-27 16:30:39.000000 trytond_account_dunning_email-7.2.0/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     2042 2024-02-04 18:51:26.000000 trytond_account_dunning_email-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:40.784935 trytond_account_dunning_email-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2287 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2178 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2374 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2181 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2288 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1803 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2207 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2225 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1835 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1983 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1851 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1781 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1767 2024-04-27 16:43:20.000000 trytond_account_dunning_email-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:40.788269 trytond_account_dunning_email-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4383 2024-03-17 11:01:36.000000 trytond_account_dunning_email-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:40.784935 trytond_account_dunning_email-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3985 2024-04-27 16:30:39.000000 trytond_account_dunning_email-7.2.0/tests/scenario_account_dunning_email.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_dunning_email-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_dunning_email-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:52.000000 trytond_account_dunning_email-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      117 2024-04-29 15:13:22.000000 trytond_account_dunning_email-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:40.788269 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2724 2024-04-29 15:32:40.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1702 2024-04-29 15:32:40.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:40.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:32:40.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:32:40.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:40.000000 trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:40.788269 trytond_account_dunning_email-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.2.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:20.000000 trytond_account_dunning_email-7.2.0/view/dunning_level_list.xml
```

### Comparing `trytond_account_dunning_email-7.0.0/CHANGELOG` & `trytond_account_dunning_email-7.2.0/CHANGELOG`

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
 * Merge email logs into email archives
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_account_dunning_email-7.0.0/COPYRIGHT` & `trytond_account_dunning_email-7.2.0/COPYRIGHT`

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

### Comparing `trytond_account_dunning_email-7.0.0/LICENSE` & `trytond_account_dunning_email-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/PKG-INFO` & `trytond_account_dunning_email-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning_email
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for account dunning email
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_dunning<7.1,>=7.0
-Requires-Dist: trytond_account_dunning_letter<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_dunning<7.3,>=7.2
+Requires-Dist: trytond_account_dunning_letter<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Dunning Email Module
 ############################
 
 The account_dunning_email module sends a dunning email to the party email
 contact after the process of dunnings for those which are at a level with *Send
 Email* checked.
```

### Comparing `trytond_account_dunning_email-7.0.0/__init__.py` & `trytond_account_dunning_email-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/account.py` & `trytond_account_dunning_email-7.2.0/account.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from email.header import Header
-from email.utils import formataddr, getaddresses
 
 from trytond.config import config
 from trytond.model import fields
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval
 from trytond.report import get_email
-from trytond.sendmail import SMTPDataManager, sendmail_transactional
-from trytond.tools.email_ import convert_ascii_email, set_from_header
+from trytond.sendmail import SMTPDataManager, send_message_transactional
+from trytond.tools.email_ import format_address, has_rcpt, set_from_header
 from trytond.transaction import Transaction
 from trytond.wizard import StateTransition
 
 
-def _formataddr(pair):
-    name, address = pair
-    if name:
-        name = str(Header(name, 'utf-8'))
-    return formataddr((name, convert_ascii_email(address)))
-
-
 class Configuration(metaclass=PoolMeta):
     __name__ = 'account.configuration'
 
     dunning_email_fallback = fields.Many2One(
         'res.user', "Fall-back User",
         domain=[
             ('email', '!=', None),
@@ -122,55 +113,45 @@
 
         from_ = config.get('email', 'from')
         to = []
         contact = self.party.contact_mechanism_get(
             'email', usage=self.level.email_contact_mechanism)
         if contact and contact.email:
             name = contact.name or self.party.rec_name
-            to.append(_formataddr((name, contact.email)))
+            to.append(format_address(contact.email, name))
         elif account_config.dunning_email_fallback:
             user = account_config.get_multivalue(
                 'dunning_email_fallback', company=self.company.id)
-            to.append(_formataddr((self.party.rec_name, user.email)))
+            to.append(format_address(user.email, self.party.rec_name))
         cc = []
         bcc = []
         languages = set()
         if self.party.lang:
             languages.add(self.party.lang)
         else:
             lang, = Lang.search([
                     ('code', '=', Configuration.get_language()),
                     ], limit=1)
             languages.add(lang)
 
-        msg, title = self._email(from_, to, cc, bcc, languages)
-        to_addrs = [e for _, e in getaddresses(to + cc + bcc)]
-        if to_addrs:
-            if not pool.test:
-                sendmail_transactional(
-                    from_, to_addrs, msg, datamanager=datamanager)
-            return Email(
-                recipients=', '.join(to),
-                recipients_secondary=', '.join(cc),
-                recipients_hidden=', '.join(bcc),
-                addresses=[{'address': a} for a in to_addrs],
-                subject=title,
-                resource=self,
-                dunning_level=self.level,
-                )
+        msg = self._email(from_, to, cc, bcc, languages)
+        if has_rcpt(msg):
+            send_message_transactional(msg, datamanager=datamanager)
+            return Email.from_message(
+                msg, resource=self, dunning_level=self.level)
 
     def _email(self, sender, to, cc, bcc, languages):
         # TODO order languages to get default as last one for title
         msg, title = get_email(self.level.email_template, self, languages)
         language = list(languages)[-1]
         from_ = sender
         with Transaction().set_context(language=language.code):
             dunning = self.__class__(self.id)
             if dunning.level.email_from:
                 from_ = dunning.level.email_from
         set_from_header(msg, sender, from_)
-        msg['To'] = ', '.join(to)
-        msg['Cc'] = ', '.join(cc)
-        msg['Bcc'] = ', '.join(bcc)
-        msg['Subject'] = Header(title, 'utf-8')
+        msg['To'] = to
+        msg['Cc'] = cc
+        msg['Bcc'] = bcc
+        msg['Subject'] = title
         msg['Auto-Submitted'] = 'auto-generated'
-        return msg, title
+        return msg
```

### Comparing `trytond_account_dunning_email-7.0.0/account.xml` & `trytond_account_dunning_email-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/doc/conf.py` & `trytond_account_dunning_email-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_dunning_email-7.0.0/email.html` & `trytond_account_dunning_email-7.2.0/email.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <title>Reminder Notice</title>
     </head>
     <body>
         <py:for each="party, letter in letters.items()">
         <header style="text-align: center">
             <h3>${company.rec_name}</h3>
             <py:if test="company.header">
-            <p py:for="line in company.header.splitlines()">${line}</p>
+            <p py:for="line in company.header_used.splitlines()">${line}</p>
             </py:if>
         </header>
         <h1 style="text-align: center">Reminder Notice</h1>
         <p>Date: ${format_date(today, data.language)}</p>
         <p py:if="letter.fees">Fees:
         ${', '.join(format_currency(amount, data['language'], cur)
         for cur, amount in letter.fees.items())}
@@ -70,13 +70,13 @@
                     </td>
                 </tr>
             </tbody>
             </py:if>
         </table>
         <footer style="text-align: center">
             <py:if test="company.footer">
-            <p py:for="line in company.footer.splitlines()">${line}</p>
+            <p py:for="line in company.footer_used.splitlines()">${line}</p>
             </py:if>
         </footer>
         </py:for>
     </body>
 </html>
```

### Comparing `trytond_account_dunning_email-7.0.0/ir.py` & `trytond_account_dunning_email-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/bg.po` & `trytond_account_dunning_email-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/ca.po` & `trytond_account_dunning_email-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/cs.po` & `trytond_account_dunning_email-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/de.po` & `trytond_account_dunning_email-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/es.po` & `trytond_account_dunning_email-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/es_419.po` & `trytond_account_dunning_email-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/et.po` & `trytond_account_dunning_email-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/fa.po` & `trytond_account_dunning_email-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/fi.po` & `trytond_account_dunning_email-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/fr.po` & `trytond_account_dunning_email-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/hu.po` & `trytond_account_dunning_email-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/id.po` & `trytond_account_dunning_email-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/it.po` & `trytond_account_dunning_email-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/lo.po` & `trytond_account_dunning_email-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/lt.po` & `trytond_account_dunning_email-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/nl.po` & `trytond_account_dunning_email-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/pl.po` & `trytond_account_dunning_email-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/pt.po` & `trytond_account_dunning_email-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/ro.po` & `trytond_account_dunning_email-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/ru.po` & `trytond_account_dunning_email-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/sl.po` & `trytond_account_dunning_email-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/tr.po` & `trytond_account_dunning_email-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/uk.po` & `trytond_account_dunning_email-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/locale/zh_CN.po` & `trytond_account_dunning_email-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/setup.py` & `trytond_account_dunning_email-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/tests/scenario_account_dunning_email.rst` & `trytond_account_dunning_email-7.2.0/tests/scenario_account_dunning_email.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 Account Dunning Email Scenario
 ==============================
 
 Imports::
 
     >>> import datetime
     >>> from decimal import Decimal
+    >>> from unittest.mock import patch
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_dunning_email import account
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
+Patch send_message_transactional::
+
+    >>> smtp_calls = patch.object(
+    ...     account, 'send_message_transactional').start()
+    >>> manager = patch.object(
+    ...     account, 'SMTPDataManager').start()
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning_email')
 
     >>> Email = Model.get('ir.email')
 
@@ -121,11 +129,9 @@
     'waiting'
 
     >>> email, = Email.find([])
     >>> email.recipients
     'Customer <customer@example.com>'
     >>> email.subject
     'Dunning Email'
-    >>> email.resource == dunning
-    True
-    >>> email.dunning_level == level
-    True
+    >>> assertEqual(email.resource, dunning)
+    >>> assertEqual(email.dunning_level, level)
```

### Comparing `trytond_account_dunning_email-7.0.0/tox.ini` & `trytond_account_dunning_email-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/PKG-INFO` & `trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-dunning-email
-Version: 7.0.0
+Name: trytond_account_dunning_email
+Version: 7.2.0
 Summary: Tryton module for account dunning email
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_dunning<7.1,>=7.0
-Requires-Dist: trytond_account_dunning_letter<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_dunning<7.3,>=7.2
+Requires-Dist: trytond_account_dunning_letter<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Dunning Email Module
 ############################
 
 The account_dunning_email module sends a dunning email to the party email
 contact after the process of dunnings for those which are at a level with *Send
 Email* checked.
```

### Comparing `trytond_account_dunning_email-7.0.0/trytond_account_dunning_email.egg-info/SOURCES.txt` & `trytond_account_dunning_email-7.2.0/trytond_account_dunning_email.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_dunning_email-7.0.0/view/dunning_level_form.xml` & `trytond_account_dunning_email-7.2.0/view/dunning_level_form.xml`

 * *Files identical despite different names*

