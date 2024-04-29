# Comparing `tmp/trytond_account_dunning_letter-7.0.0.tar.gz` & `tmp/trytond_account_dunning_letter-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning_letter-7.0.0.tar", last modified: Mon Oct 30 17:19:47 2023, max compression
+gzip compressed data, was "trytond_account_dunning_letter-7.2.0.tar", last modified: Mon Apr 29 15:32:52 2024, max compression
```

## Comparing `trytond_account_dunning_letter-7.0.0.tar` & `trytond_account_dunning_letter-7.2.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:47.289223 trytond_account_dunning_letter-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:22:50.000000 trytond_account_dunning_letter-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-10-30 17:01:28.000000 trytond_account_dunning_letter-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:01:28.000000 trytond_account_dunning_letter-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-30 17:19:47.289223 trytond_account_dunning_letter-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:47.289223 trytond_account_dunning_letter-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:22:50.000000 trytond_account_dunning_letter-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:50.000000 trytond_account_dunning_letter-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     5286 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.0.0/dunning.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    60409 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/letter.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:47.285890 trytond_account_dunning_letter-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1029 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1018 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      882 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1018 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      888 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      882 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      882 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1003 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1004 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1010 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      978 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      989 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      939 2023-10-28 12:11:19.000000 trytond_account_dunning_letter-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:19:47.289223 trytond_account_dunning_letter-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4523 2023-10-27 17:38:49.000000 trytond_account_dunning_letter-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:47.285890 trytond_account_dunning_letter-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5556 2023-06-10 11:39:56.000000 trytond_account_dunning_letter-7.0.0/tests/scenario_account_dunning_letter.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_dunning_letter-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2023-10-30 17:01:25.000000 trytond_account_dunning_letter-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:47.289223 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-30 17:19:46.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1659 2023-10-30 17:19:47.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:19:46.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:19:46.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-30 17:19:46.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:19:46.000000 trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:47.289223 trytond_account_dunning_letter-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.0.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.0.0/view/dunning_level_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:52.707957 trytond_account_dunning_letter-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1949 2024-04-29 15:13:36.000000 trytond_account_dunning_letter-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:13:36.000000 trytond_account_dunning_letter-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2816 2024-04-29 15:32:52.707957 trytond_account_dunning_letter-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:52.701290 trytond_account_dunning_letter-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_dunning_letter-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:53.000000 trytond_account_dunning_letter-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     5286 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.2.0/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.2.0/dunning.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    60419 2024-04-29 13:17:17.000000 trytond_account_dunning_letter-7.2.0/letter.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:52.704624 trytond_account_dunning_letter-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1029 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1018 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      882 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1018 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      888 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1065 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      882 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      882 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      895 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1004 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1010 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      978 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      989 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      939 2024-04-27 16:43:20.000000 trytond_account_dunning_letter-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:52.707957 trytond_account_dunning_letter-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4523 2024-03-17 11:01:36.000000 trytond_account_dunning_letter-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:52.704624 trytond_account_dunning_letter-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5536 2024-04-22 12:14:36.000000 trytond_account_dunning_letter-7.2.0/tests/scenario_account_dunning_letter.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:53.000000 trytond_account_dunning_letter-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2024-04-29 15:13:32.000000 trytond_account_dunning_letter-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:52.704624 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2816 2024-04-29 15:32:52.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1641 2024-04-29 15:32:52.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:52.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:32:52.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:32:52.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:52.000000 trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:52.704624 trytond_account_dunning_letter-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.2.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-7.2.0/view/dunning_level_list.xml
```

### Comparing `trytond_account_dunning_letter-7.0.0/CHANGELOG` & `trytond_account_dunning_letter-7.2.0/CHANGELOG`

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

### Comparing `trytond_account_dunning_letter-7.0.0/COPYRIGHT` & `trytond_account_dunning_letter-7.2.0/COPYRIGHT`

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

### Comparing `trytond_account_dunning_letter-7.0.0/LICENSE` & `trytond_account_dunning_letter-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/PKG-INFO` & `trytond_account_dunning_letter-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning_letter
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for account dunning letter
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
-Requires-Dist: trytond_account_dunning<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_dunning<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Dunning Letter Module
 #############################
 
 The account_dunning_letter module generates a dunning letter after the process
 of dunnings for those who are at a level with *Print on Letter* checked.
```

### Comparing `trytond_account_dunning_letter-7.0.0/__init__.py` & `trytond_account_dunning_letter-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/doc/conf.py` & `trytond_account_dunning_letter-7.2.0/doc/conf.py`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_account_dunning_letter-7.0.0/dunning.py` & `trytond_account_dunning_letter-7.2.0/dunning.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/dunning.xml` & `trytond_account_dunning_letter-7.2.0/dunning.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/letter.fodt` & `trytond_account_dunning_letter-7.2.0/letter.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_account_dunning_letter-7.0.0/letter.fodt` & `trytond_account_dunning_letter-7.2.0/letter.fodt`

```diff
@@ -522,15 +522,15 @@
   <office:master-styles>
     <style:master-page style:name="Standard" style:page-layout-name="pm1">
       <style:header>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -542,15 +542,15 @@
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P3">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P3">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P3">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P3">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
```

### Comparing `trytond_account_dunning_letter-7.0.0/locale/bg.po` & `trytond_account_dunning_letter-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/ca.po` & `trytond_account_dunning_letter-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/cs.po` & `trytond_account_dunning_letter-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/de.po` & `trytond_account_dunning_letter-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/es.po` & `trytond_account_dunning_letter-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/es_419.po` & `trytond_account_dunning_letter-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/et.po` & `trytond_account_dunning_letter-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/fa.po` & `trytond_account_dunning_letter-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/fi.po` & `trytond_account_dunning_letter-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/fr.po` & `trytond_account_dunning_letter-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/hu.po` & `trytond_account_dunning_letter-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/id.po` & `trytond_account_dunning_letter-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/it.po` & `trytond_account_dunning_letter-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/lo.po` & `trytond_account_dunning_letter-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/lt.po` & `trytond_account_dunning_letter-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/nl.po` & `trytond_account_dunning_letter-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/pl.po` & `trytond_account_dunning_letter-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/pt.po` & `trytond_account_dunning_letter-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/ro.po` & `trytond_account_dunning_letter-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/ru.po` & `trytond_account_dunning_letter-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/sl.po` & `trytond_account_dunning_letter-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/tr.po` & `trytond_account_dunning_letter-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/uk.po` & `trytond_account_dunning_letter-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/locale/zh_CN.po` & `trytond_account_dunning_letter-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/setup.py` & `trytond_account_dunning_letter-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/tests/scenario_account_dunning_letter.rst` & `trytond_account_dunning_letter-7.2.0/tests/scenario_account_dunning_letter.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Account Dunning Scenario
 ========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import config, Model, Wizard
+
+    >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning_letter')
 
 Create company::
```

### Comparing `trytond_account_dunning_letter-7.0.0/tox.ini` & `trytond_account_dunning_letter-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/PKG-INFO` & `trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-dunning-letter
-Version: 7.0.0
+Name: trytond_account_dunning_letter
+Version: 7.2.0
 Summary: Tryton module for account dunning letter
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
-Requires-Dist: trytond_account_dunning<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_dunning<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Dunning Letter Module
 #############################
 
 The account_dunning_letter module generates a dunning letter after the process
 of dunnings for those who are at a level with *Print on Letter* checked.
```

### Comparing `trytond_account_dunning_letter-7.0.0/trytond_account_dunning_letter.egg-info/SOURCES.txt` & `trytond_account_dunning_letter-7.2.0/trytond_account_dunning_letter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 dunning.py
```

