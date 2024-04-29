# Comparing `tmp/trytond_account_consolidation-7.0.0.tar.gz` & `tmp/trytond_account_consolidation-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_consolidation-7.0.0.tar", last modified: Mon Oct 30 17:18:45 2023, max compression
+gzip compressed data, was "trytond_account_consolidation-7.2.0.tar", last modified: Mon Apr 29 15:32:08 2024, max compression
```

## Comparing `trytond_account_consolidation-7.0.0.tar` & `trytond_account_consolidation-7.2.0.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:45.862264 trytond_account_consolidation-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:22:48.000000 trytond_account_consolidation-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:01:02.000000 trytond_account_consolidation-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-10-30 17:01:01.000000 trytond_account_consolidation-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2687 2023-10-30 17:18:45.858930 trytond_account_consolidation-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15397 2023-10-07 15:40:36.000000 trytond_account_consolidation-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10785 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    54958 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/consolidation_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:45.858930 trytond_account_consolidation-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:22:48.000000 trytond_account_consolidation-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1272 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:48.000000 trytond_account_consolidation-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1053 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:45.855597 trytond_account_consolidation-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5986 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6125 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6012 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6029 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5985 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5232 2023-10-30 16:47:45.000000 trytond_account_consolidation-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-10-28 12:11:19.000000 trytond_account_consolidation-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:18:45.862264 trytond_account_consolidation-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4782 2023-10-27 17:38:49.000000 trytond_account_consolidation-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:45.855597 trytond_account_consolidation-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6728 2023-10-07 15:40:36.000000 trytond_account_consolidation-7.0.0/tests/scenario_consolidation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1872 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2023-10-07 15:40:36.000000 trytond_account_consolidation-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_consolidation-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2023-10-30 17:00:58.000000 trytond_account_consolidation-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:45.858930 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2687 2023-10-30 17:18:45.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-10-30 17:18:45.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:18:45.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:18:45.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-10-30 17:18:45.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:18:45.000000 trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:45.855597 trytond_account_consolidation-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      810 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/consolidation_balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/consolidation_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/view/consolidation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/view/consolidation_income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/consolidation_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/consolidation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/consolidation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.0.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.0.0/view/move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:08.642443 trytond_account_consolidation-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:13:02.000000 trytond_account_consolidation-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2024-04-29 15:13:02.000000 trytond_account_consolidation-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2678 2024-04-29 15:32:08.642443 trytond_account_consolidation-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15397 2024-01-27 09:58:52.000000 trytond_account_consolidation-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10716 2024-04-27 16:30:39.000000 trytond_account_consolidation-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    54958 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/consolidation_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:08.639109 trytond_account_consolidation-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_account_consolidation-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1272 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:51.000000 trytond_account_consolidation-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1053 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:08.639109 trytond_account_consolidation-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5986 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6125 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6012 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6026 2024-04-29 13:17:17.000000 trytond_account_consolidation-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5985 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5492 2024-04-29 13:17:17.000000 trytond_account_consolidation-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-04-27 16:43:20.000000 trytond_account_consolidation-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:08.642443 trytond_account_consolidation-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4773 2024-04-27 16:30:39.000000 trytond_account_consolidation-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:08.642443 trytond_account_consolidation-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6727 2024-04-22 12:14:36.000000 trytond_account_consolidation-7.2.0/tests/scenario_consolidation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1888 2024-04-22 12:14:36.000000 trytond_account_consolidation-7.2.0/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-01-27 09:58:52.000000 trytond_account_consolidation-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:51.000000 trytond_account_consolidation-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-04-29 15:12:58.000000 trytond_account_consolidation-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:08.642443 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2678 2024-04-29 15:32:08.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2578 2024-04-29 15:32:08.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:08.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:32:08.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-29 15:32:08.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:08.000000 trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:08.642443 trytond_account_consolidation-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      810 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/consolidation_balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/consolidation_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/view/consolidation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/view/consolidation_income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/consolidation_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/consolidation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/consolidation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:14.000000 trytond_account_consolidation-7.2.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_account_consolidation-7.2.0/view/move_list.xml
```

### Comparing `trytond_account_consolidation-7.0.0/COPYRIGHT` & `trytond_account_consolidation-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2021 NaN-tic
-Copyright (C) 2022-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2022-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_consolidation-7.0.0/LICENSE` & `trytond_account_consolidation-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/PKG-INFO` & `trytond_account_consolidation-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_consolidation
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module consolidate accounting of many companies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-consolidation
+Project-URL: Documentation, https://docs.tryton.org/modules-account-consolidation
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account consolidation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_account_consolidation-7.0.0/__init__.py` & `trytond_account_consolidation-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/account.py` & `trytond_account_consolidation-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/account.xml` & `trytond_account_consolidation-7.2.0/account.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_consolidation-7.0.0/account.xml` & `trytond_account_consolidation-7.2.0/account.xml`

```diff
@@ -79,30 +79,30 @@
     <record model="ir.action.act_window.view" id="act_consolidation_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="consolidation_view_form"/>
       <field name="act_window" ref="act_consolidation_list"/>
     </record>
     <menuitem parent="menu_consolidation_tree" action="act_consolidation_list" sequence="10" id="menu_consolidation_list"/>
     <record model="ir.model.access" id="access_consolidation">
-      <field name="model" search="[('model', '=', 'account.consolidation')]"/>
+      <field name="model">account.consolidation</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_consolidation_account">
-      <field name="model" search="[('model', '=', 'account.consolidation')]"/>
+      <field name="model">account.consolidation</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_consolidation_account_admin">
-      <field name="model" search="[('model', '=', 'account.consolidation')]"/>
+      <field name="model">account.consolidation</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="consolidation_balance_sheet_view_tree">
```

### Comparing `trytond_account_consolidation-7.0.0/consolidation_statement.fodt` & `trytond_account_consolidation-7.2.0/consolidation_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/doc/conf.py` & `trytond_account_consolidation-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_consolidation-7.0.0/doc/design.rst` & `trytond_account_consolidation-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/doc/usage.rst` & `trytond_account_consolidation-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/bg.po` & `trytond_account_consolidation-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/ca.po` & `trytond_account_consolidation-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/cs.po` & `trytond_account_consolidation-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/de.po` & `trytond_account_consolidation-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/es.po` & `trytond_account_consolidation-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/es_419.po` & `trytond_account_consolidation-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/et.po` & `trytond_account_consolidation-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/fa.po` & `trytond_account_consolidation-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/fi.po` & `trytond_account_consolidation-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/fr.po` & `trytond_account_consolidation-7.2.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:account.consolidation,parent:"
 msgid "Parent"
 msgstr "Parent"
 
 msgctxt "field:account.consolidation,statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Raport"
 
 msgctxt "field:account.consolidation,types:"
 msgid "Types"
 msgstr "Types"
 
 msgctxt "field:account.consolidation.balance_sheet.context,companies:"
 msgid "Companies"
@@ -144,15 +144,15 @@
 
 msgctxt "model:ir.action,name:act_consolidation_tree"
 msgid "Account Consolidations"
 msgstr "Consolidations de compte"
 
 msgctxt "model:ir.action,name:report_consolidation_statement"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Raport"
 
 msgctxt "model:ir.ui.menu,name:menu_consolidation_list"
 msgid "Account Consolidations"
 msgstr "Consolidations de compte"
 
 msgctxt "model:ir.ui.menu,name:menu_consolidation_tree"
 msgid "Account Consolidations"
@@ -192,15 +192,15 @@
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Print Date:"
 msgstr "Date d'impression :"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Raport"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "To"
 msgstr "à"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "User:"
```

### Comparing `trytond_account_consolidation-7.0.0/locale/hu.po` & `trytond_account_consolidation-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/id.po` & `trytond_account_consolidation-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/it.po` & `trytond_account_consolidation-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/lo.po` & `trytond_account_consolidation-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/lt.po` & `trytond_account_consolidation-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/nl.po` & `trytond_account_consolidation-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/pl.po` & `trytond_account_consolidation-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/pt.po` & `trytond_account_consolidation-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/ro.po` & `trytond_account_consolidation-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #
-#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,consolidation:"
 msgid "Consolidation"
 msgstr ""
 
@@ -129,15 +128,15 @@
 
 msgctxt "model:account.consolidation.income_statement.context,name:"
 msgid "Consolidation Income Statement Context"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_consolidation_balance_sheet_tree"
 msgid "Consolidated Balance Sheet"
-msgstr "Bilanţ Prescurtat"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_consolidation_income_statement_tree"
 msgid "Consolidated Income Statement"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_consolidation_list"
 msgid "Account Consolidations"
@@ -157,27 +156,27 @@
 
 msgctxt "model:ir.ui.menu,name:menu_consolidation_tree"
 msgid "Account Consolidations"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_open_consolidation_balance_sheet"
 msgid "Consolidated Balance Sheet"
-msgstr "Bilanţ Prescurtat"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_open_consolidation_income_statement"
 msgid "Consolidated Income Statement"
 msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "/"
 msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Balance Sheet"
-msgstr "Bilanţ"
+msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Companies:"
 msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Date:"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_consolidation-7.0.0/locale/ru.po` & `trytond_account_consolidation-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/sl.po` & `trytond_account_consolidation-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/tr.po` & `trytond_account_consolidation-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/uk.po` & `trytond_account_consolidation-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/locale/zh_CN.po` & `trytond_account_consolidation-7.2.0/locale/ro.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,103 +4,106 @@
 
 msgctxt "field:account.account.type,consolidation:"
 msgid "Consolidation"
 msgstr ""
 
 msgctxt "field:account.consolidation,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:account.consolidation,amount_cmp:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:account.consolidation,assets:"
 msgid "Assets"
-msgstr ""
+msgstr "Active"
 
 msgctxt "field:account.consolidation,children:"
 msgid "Children"
 msgstr ""
 
 msgctxt "field:account.consolidation,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:account.consolidation,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nume"
 
 msgctxt "field:account.consolidation,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:account.consolidation,statement:"
 msgid "Statement"
 msgstr ""
 
 msgctxt "field:account.consolidation,types:"
 msgid "Types"
-msgstr ""
+msgstr "Tipuri"
 
 msgctxt "field:account.consolidation.balance_sheet.context,companies:"
 msgid "Companies"
-msgstr ""
+msgstr "Companii"
 
 msgctxt "field:account.consolidation.balance_sheet.context,comparison:"
 msgid "Comparison"
-msgstr ""
+msgstr "Comparatie"
 
 msgctxt "field:account.consolidation.balance_sheet.context,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
 msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
-msgstr ""
+msgstr "Companii"
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
 msgid "Comparison"
-msgstr ""
+msgstr "Comparatie"
 
 msgctxt "field:account.consolidation.income_statement.context,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
+#, fuzzy
 msgctxt "field:account.consolidation.income_statement.context,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "De la Data"
 
+#, fuzzy
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
-msgstr ""
+msgstr "De la Data"
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
 msgid "Posted Moves"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Pana in Prezent"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
 msgid "To Date"
-msgstr ""
+msgstr "Pana in Prezent"
 
 msgctxt "field:account.invoice,consolidation_company:"
 msgid "Consolidation Company"
 msgstr ""
 
 msgctxt "field:account.move,consolidation_company:"
 msgid "Consolidation Company"
@@ -128,15 +131,15 @@
 
 msgctxt "model:account.consolidation.income_statement.context,name:"
 msgid "Consolidation Income Statement Context"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_consolidation_balance_sheet_tree"
 msgid "Consolidated Balance Sheet"
-msgstr ""
+msgstr "Bilanţ Prescurtat"
 
 msgctxt "model:ir.action,name:act_consolidation_income_statement_tree"
 msgid "Consolidated Income Statement"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_consolidation_list"
 msgid "Account Consolidations"
@@ -156,72 +159,74 @@
 
 msgctxt "model:ir.ui.menu,name:menu_consolidation_tree"
 msgid "Account Consolidations"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_open_consolidation_balance_sheet"
 msgid "Consolidated Balance Sheet"
-msgstr ""
+msgstr "Bilanţ Prescurtat"
 
 msgctxt "model:ir.ui.menu,name:menu_open_consolidation_income_statement"
 msgid "Consolidated Income Statement"
 msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "/"
-msgstr ""
+msgstr "/"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Balance Sheet"
-msgstr ""
+msgstr "Bilanţ"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Companies:"
-msgstr ""
+msgstr "Companii:"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Date:"
-msgstr ""
+msgstr "Data:"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "From Date:"
-msgstr ""
+msgstr "De la Data:"
 
+#, fuzzy
 msgctxt "report:account.consolidation.statement:"
 msgid "Income Statement"
-msgstr ""
+msgstr "Adeverinta de Venit"
 
+#, fuzzy
 msgctxt "report:account.consolidation.statement:"
 msgid "Print Date:"
-msgstr ""
+msgstr "Data Tiparirii:"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "Statement"
 msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "To"
 msgstr ""
 
 msgctxt "report:account.consolidation.statement:"
 msgid "User:"
-msgstr ""
+msgstr "Utilizator:"
 
 msgctxt "report:account.consolidation.statement:"
 msgid "at"
-msgstr ""
+msgstr "la"
 
 msgctxt "selection:account.consolidation,statement:"
 msgid "Balance"
 msgstr ""
 
 msgctxt "selection:account.consolidation,statement:"
 msgid "Income"
-msgstr ""
+msgstr "Venit"
 
 msgctxt "selection:account.consolidation,statement:"
 msgid "Off-Balance"
 msgstr ""
 
 msgctxt "view:account.consolidation:"
 msgid "Comparison"
-msgstr ""
+msgstr "Comparatie"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_consolidation-7.0.0/setup.py` & `trytond_account_consolidation-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-consolidation'),
+            'https://docs.tryton.org/modules-account-consolidation'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account consolidation',
     package_dir={'trytond.modules.account_consolidation': '.'},
     packages=(
         ['trytond.modules.account_consolidation']
```

### Comparing `trytond_account_consolidation-7.0.0/tests/scenario_consolidation.rst` & `trytond_account_consolidation-7.2.0/tests/scenario_consolidation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 ==============================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Report
-
-    >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
-    >>> from trytond.modules.currency.tests.tools import get_currency
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, set_user
 
 Activate modules::
 
     >>> config = activate_modules(['account_consolidation'])
 
     >>> Company = Model.get('company.company')
     >>> Consolidation = Model.get('account.consolidation')
```

### Comparing `trytond_account_consolidation-7.0.0/tests/scenario_invoice.rst` & `trytond_account_consolidation-7.2.0/tests/scenario_invoice.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 ================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['account_consolidation', 'account_invoice'])
 
     >>> Company = Model.get('company.company')
     >>> Invoice = Model.get('account.invoice')
@@ -57,11 +56,9 @@
     >>> line.unit_price = Decimal('10.0000')
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
 
 Check consolidation company::
 
-    >>> invoice.consolidation_company == saber
-    True
-    >>> invoice.move.consolidation_company == saber
-    True
+    >>> assertEqual(invoice.consolidation_company, saber)
+    >>> assertEqual(invoice.move.consolidation_company, saber)
```

### Comparing `trytond_account_consolidation-7.0.0/tests/test_module.py` & `trytond_account_consolidation-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/tox.ini` & `trytond_account_consolidation-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/PKG-INFO` & `trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-consolidation
-Version: 7.0.0
+Name: trytond_account_consolidation
+Version: 7.2.0
 Summary: Tryton module consolidate accounting of many companies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-consolidation
+Project-URL: Documentation, https://docs.tryton.org/modules-account-consolidation
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account consolidation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_account_consolidation-7.0.0/trytond_account_consolidation.egg-info/SOURCES.txt` & `trytond_account_consolidation-7.2.0/trytond_account_consolidation.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_consolidation-7.0.0/view/consolidation_balance_sheet_context_form.xml` & `trytond_account_consolidation-7.2.0/view/consolidation_balance_sheet_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/view/consolidation_form.xml` & `trytond_account_consolidation-7.2.0/view/consolidation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-7.0.0/view/consolidation_income_statement_context_form.xml` & `trytond_account_consolidation-7.2.0/view/consolidation_income_statement_context_form.xml`

 * *Files identical despite different names*

