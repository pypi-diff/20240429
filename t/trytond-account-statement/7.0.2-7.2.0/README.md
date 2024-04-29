# Comparing `tmp/trytond_account_statement-7.0.2.tar.gz` & `tmp/trytond_account_statement-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement-7.0.2.tar", last modified: Sun Mar  3 12:24:25 2024, max compression
+gzip compressed data, was "trytond_account_statement-7.2.0.tar", last modified: Mon Apr 29 15:35:41 2024, max compression
```

## Comparing `trytond_account_statement-7.0.2.tar` & `trytond_account_statement-7.2.0.tar`

### file list

```diff
@@ -1,80 +1,85 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:25.466122 trytond_account_statement-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     4589 2024-03-03 12:24:22.000000 trytond_account_statement-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-03-03 12:24:22.000000 trytond_account_statement-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5151 2024-03-03 12:24:25.466122 trytond_account_statement-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2450 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1403 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:25.459455 trytond_account_statement-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2450 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3213 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3173 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:25.462788 trytond_account_statement-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14581 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15024 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13136 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15442 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15054 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13292 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13822 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16096 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13110 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15171 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14008 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13166 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13813 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15025 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13320 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15371 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13092 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14027 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12747 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14451 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13790 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13322 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12423 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13338 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2828 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:24:25.466122 trytond_account_statement-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4482 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51346 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/statement.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    44363 2024-02-29 11:38:35.000000 trytond_account_statement-7.0.2/statement.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18942 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/statement.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:25.462788 trytond_account_statement-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15105 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/tests/scenario_account_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3029 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/tests/scenario_statement_origin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/tests/scenario_statement_origin_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2024-02-15 18:37:37.000000 trytond_account_statement-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:25.466122 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5151 2024-03-03 12:24:25.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2024-03-03 12:24:25.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:24:25.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-03-03 12:24:25.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:38.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-03-03 12:24:25.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:24:25.000000 trytond_account_statement-7.0.2/trytond_account_statement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:25.466122 trytond_account_statement-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      597 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/line_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/line_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1732 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/view/statement_import_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/view/statement_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/view/statement_journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      839 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/statement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/statement_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/statement_line_tree_editable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/statement_origin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2024-02-05 16:24:27.000000 trytond_account_statement-7.0.2/view/statement_origin_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-10-30 17:06:38.000000 trytond_account_statement-7.0.2/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5399 2024-04-29 15:15:49.000000 trytond_account_statement-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:15:49.000000 trytond_account_statement-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1403 2024-03-17 11:01:36.000000 trytond_account_statement-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/bank.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.326880 trytond_account_statement-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      748 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_statement-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3680 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3104 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.326880 trytond_account_statement-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16002 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16529 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14452 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16967 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14608 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15240 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17386 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14426 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16728 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15409 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14586 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15204 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16521 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16889 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14408 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15437 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15067 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15872 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15199 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14638 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14654 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3474 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51356 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/statement.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    47460 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/statement.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18593 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/statement.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.326880 trytond_account_statement-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14862 2024-04-22 12:14:36.000000 trytond_account_statement-7.2.0/tests/scenario_account_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2553 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/tests/scenario_account_statement_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/tests/scenario_account_statement_second_currency_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2992 2024-04-22 12:14:36.000000 trytond_account_statement-7.2.0/tests/scenario_statement_origin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-22 12:14:36.000000 trytond_account_statement-7.2.0/tests/scenario_statement_origin_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_statement-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2024-04-29 15:15:45.000000 trytond_account_statement-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2872 2024-04-29 15:35:41.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/line_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/line_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1732 2024-02-04 18:51:26.000000 trytond_account_statement-7.2.0/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_account_statement-7.2.0/view/statement_import_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-02-04 18:51:26.000000 trytond_account_statement-7.2.0/view/statement_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/view/statement_journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_line_tree_editable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_origin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_origin_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/view/statement_tree.xml
```

### Comparing `trytond_account_statement-7.0.2/CHANGELOG` & `trytond_account_statement-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 
-Version 7.0.2 - 2024-03-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-02-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Allow RPC on get_by_bank_account of statement journal
+* Search statement journal by bank account and currency
+* Support second currency on statement line
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
@@ -24,132 +21,160 @@
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Require party on statement line if account requires one
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use reference field for statement line relation
 * Create default statement journal
 * Add support for Python 3.10
 * Remove support for Python 3.6
 
 Version 6.2.0 - 2021-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow statement journals to be deactivated
 
 Version 6.0.0 - 2021-05-03
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Warn user when posting a statement with cancelled or paid invoices
 * Fill move line's origin with statement line
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 * Rename statement state from cancel to cancelled
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Prevent posting move from statement that is not posted
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Require fresh session to post a statement
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use invoice amount to pay as line amount when creating lines from origins
 * Rename Origin field informations to information
 
 Version 5.0.0 - 2018-10-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use single account for statement journal
 * Remove support for Python 2.7
 
 Version 4.8.0 - 2018-04-23
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Do not check amount to pay when reconcile move lines
 * Remove line split by invoice in non company currency
 * Use new API for Line.reconcile
 * Add button to reconcile statement
 
 Version 4.6.0 - 2017-10-30
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add generic wizard to import statement from files
 * Add statement origins
 * Unreconcile lines when cancelling statement
 
 Version 4.4.0 - 2017-05-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add statement line number as move description
 * Set description on statement account line if unique
 
 Version 4.2.0 - 2016-11-28
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Manage readonly state on Statement Line
 
 Version 4.0.0 - 2016-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add Python3 support
 
 Version 3.8.0 - 2015-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove states on statement's date
 
 Version 3.6.0 - 2015-04-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for PyPy
 * Add line group model
 * Create Move by grouped lines (number, date, party)
 
 Version 3.4.0 - 2014-10-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add different validation type on journal
 * Add explicit name on statement
 * Add report to statement
 * Add number and sequence on statement line
 * Switch journal debit/credit account usage
 
 Version 3.2.0 - 2014-04-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Append new line under the original one
 * Prevent usage of paid invoice in draft statements
 
 Version 3.0.0 - 2013-10-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow to use invoice to fill party and account on statement line
 * Replace move_lines by a relate
 
 Version 2.8.0 - 2013-04-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.6.0 - 2012-10-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow to use credit note on statement line
 
 Version 2.4.0 - 2012-04-23
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Don't deactivate payment wizard on invoice
 
 Version 2.2.0 - 2011-10-24
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.0.0 - 2011-04-27
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add company on statement
 
 Version 1.8.0 - 2010-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.6.0 - 2010-05-13
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.4.0 - 2009-10-19
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Fix digits of start and end balance
 
 Version 1.2.0 - 2009-04-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.0.0 - 2009-05-01
+--------------------------
 * Initial release
```

### Comparing `trytond_account_statement-7.0.2/COPYRIGHT` & `trytond_account_statement-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.0.2/LICENSE` & `trytond_account_statement-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.0.2/__init__.py` & `trytond_account_statement-7.2.0/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.pool import Pool
 
-from . import account, journal, party, statement
+from . import account, bank, journal, party, statement
 
 
 def register():
     Pool.register(
+        bank.Account,
         journal.Journal,
         statement.Statement,
         statement.Line,
         statement.LineGroup,
         account.Journal,
         account.Move,
         account.MoveLine,
```

### Comparing `trytond_account_statement-7.0.2/account.py` & `trytond_account_statement-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.0.2/doc/conf.py` & `trytond_account_statement-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_statement-7.0.2/journal.py` & `trytond_account_statement-7.2.0/journal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.model import DeactivableMixin, ModelSQL, ModelView, Unique, fields
 from trytond.pool import Pool
 from trytond.pyson import Eval
+from trytond.rpc import RPC
 from trytond.transaction import Transaction
 
 
 class Journal(DeactivableMixin, ModelSQL, ModelView):
     'Statement Journal'
     __name__ = 'account.statement.journal'
     name = fields.Char('Name', required=True)
@@ -32,15 +33,18 @@
             ('amount', 'Amount'),
             ('number_of_lines', 'Number of Lines'),
             ], 'Validation Type', required=True)
     bank_account = fields.Many2One(
         'bank.account', "Bank Account",
         domain=[
             ('owners.id', '=', Eval('company_party', -1)),
-            ('currency', '=', Eval('currency', -1)),
+            ['OR',
+                ('currency', '=', Eval('currency', -1)),
+                ('currency', '=', None),
+                ],
             ])
     account = fields.Many2One('account.account', "Account", required=True,
         domain=[
             ('type', '!=', None),
             ('closed', '!=', True),
             ('company', '=', Eval('company')),
             ('party_required', '=', False),
@@ -52,14 +56,18 @@
         cls._order.insert(0, ('name', 'ASC'))
         t = cls.__table__()
         cls._sql_constraints = [
             ('bank_account_unique',
                 Unique(t, t.bank_account, t.company),
                 'account_statement.msg_journal_bank_account_unique'),
             ]
+        cls.__rpc__.update(
+            get_by_bank_account=RPC(
+                result=lambda r: int(r) if r is not None else None),
+            )
 
     @staticmethod
     def default_currency():
         if Transaction().context.get('company'):
             Company = Pool().get('company.company')
             company = Company(Transaction().context['company'])
             return company.currency.id
@@ -73,18 +81,24 @@
         return self.company.party if self.company else None
 
     @staticmethod
     def default_validation():
         return 'balance'
 
     @classmethod
-    def get_by_bank_account(cls, company, number):
-        journals = cls.search([
-                ('company', '=', company),
-                ['OR',
-                    ('bank_account.numbers.number', '=', number),
-                    ('bank_account.numbers.number_compact', '=', number),
-                    ],
-                ])
+    def get_by_bank_account(cls, company, number, currency=None):
+        domain = [
+            ('company', '=', company),
+            ['OR',
+                ('bank_account.numbers.number', '=', number),
+                ('bank_account.numbers.number_compact', '=', number),
+                ],
+            ]
+        if currency:
+            domain.append(['OR',
+                    ('currency.code', '=', currency),
+                    ('currency.numeric_code', '=', currency),
+                    ])
+        journals = cls.search(domain)
         if journals:
             journal, = journals
             return journal
```

### Comparing `trytond_account_statement-7.0.2/journal.xml` & `trytond_account_statement-7.2.0/journal.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_account_statement-7.0.2/journal.xml` & `trytond_account_statement-7.2.0/journal.xml`

```diff
@@ -25,31 +25,31 @@
     <record model="ir.action.act_window.view" id="act_statement_journal_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="statement_journal_view_form"/>
       <field name="act_window" ref="act_statement_journal_form"/>
     </record>
     <menuitem parent="menu_statement_configuration" action="act_statement_journal_form" sequence="10" id="menu_statement_journal_form"/>
     <record model="ir.model.access" id="access_statement_journal">
-      <field name="model" search="[('model', '=', 'account.statement.journal')]"/>
+      <field name="model">account.statement.journal</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_statement_journal_admin">
-      <field name="model" search="[('model', '=', 'account.statement.journal')]"/>
+      <field name="model">account.statement.journal</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_statement_journal_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.statement.journal')]"/>
+      <field name="model">account.statement.journal</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_statement_journal_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_statement_journal_companies"/>
     </record>
   </data>
```

### Comparing `trytond_account_statement-7.0.2/locale/bg.po` & `trytond_account_statement-7.2.0/locale/bg.po`

 * *Files 3% similar despite different names*

```diff
@@ -125,20 +125,29 @@
 msgid "Account"
 msgstr "Сметка"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Сума"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Фирма"
 
 #, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Валута"
+
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Валута"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Дата"
@@ -169,27 +178,36 @@
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Валута"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Отчет"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Сума"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Управление на валути"
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,date:"
@@ -213,34 +231,48 @@
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Управление на партньор"
 
 #, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Валута"
+
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Отчет"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "Сметка"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Сума"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Фирма"
 
 #, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Валута"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Валута"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
@@ -271,14 +303,19 @@
 msgstr "Партньор"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Валута"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Отчет"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -396,23 +433,23 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Проверен"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -425,14 +462,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
```

### Comparing `trytond_account_statement-7.0.2/locale/ca.po` & `trytond_account_statement-7.2.0/locale/ro.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,590 +1,643 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr "Sold"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Companie"
 
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
 msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Saldo final"
+msgstr "Balanță Finală"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Diari"
+msgstr "Jurnal"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Línies"
+msgstr "Rânduri"
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Nume"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Nombre de línies"
+msgstr "Numărul de rânduri"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Fitxer origen"
+msgstr "Fișierul de origine"
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr "Identificador fitxer origen"
+msgstr "ID-ul fișierului de origine"
 
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Orígens"
+msgstr "Origini"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Saldo inicial"
+msgstr "Sold Initial"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Stare"
 
+#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Per conciliar"
+msgstr "De Reconciliat"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Import total"
+msgstr "Suma Totală"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Validació"
+msgstr "Validare"
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Companie"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Fitxer"
+msgstr "Fişier"
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Format del fitxer"
+msgstr "Format Fişier"
 
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Cont"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Compte bancari"
+msgstr "Cont Bancar"
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Companie"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Tercer de l'empresa"
+msgstr ""
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Diari"
+msgstr "Jurnal"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Nume"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Tipus de validació"
+msgstr "Tip de validare"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Cont"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Suma"
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Companie"
+
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Valută"
 
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Descripció"
+msgstr "Descriere"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Assentament comptable"
+msgstr "Mişcare Cont"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Número"
+msgstr "Număr"
 
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origen"
+msgstr "Origine"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Parte"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
-msgstr "Tercer obligatori"
+msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
-msgstr "Relacionat amb"
+msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valută"
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Extracte"
+msgstr "Extras de cont"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Estat de l'extracte"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Suma"
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Diari"
+msgstr "Jurnal"
 
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Assentament"
+msgstr "Miscare"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Número"
+msgstr "Număr"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Parte"
+
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Valută"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Extracte"
+msgstr ""
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Cont"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Suma"
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Companie"
+
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Valută"
 
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Descripció"
+msgstr "Descriere"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Informació"
+msgstr "Informație"
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Línies"
+msgstr "Rânduri"
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Número"
+msgstr "Număr"
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Parte"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Import pendent"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Valută"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Extracte"
+msgstr ""
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "ID del Extracte"
+msgstr ""
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Estat de l'extracte"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Extracte"
+msgstr "Extras de cont"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Extracte bancari"
+msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr "Inici importació extracte"
+msgstr ""
 
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Diari d'extracte"
+msgstr ""
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Línia d'extracte bancari"
+msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Grup de línies d'extracte"
+msgstr ""
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Origen Extracte"
+msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr "Informació origen extracte"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Grups de línies"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Grups de línies"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Apunts"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Assentaments"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Concilia extractes"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Extractes"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Diaris d'extracte"
+msgstr "Extras de cont"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Línies d'extracte"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Línies d'extracte"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Orígens"
+msgstr "Origini"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Extracte"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Importa extracte"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
 msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Ciornă"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Comptabilitzat"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validat"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
-"Per importar l'extracte heu de crear un diari per al compte \"%(account)s\"."
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
-"Per importar el extracte el diari \"%(journal)s\" ha de tenir la moneda "
-"\"%(currency)s\" en comptes de \"%(journal_currency)s\"."
+"Pentru a importa extrasul, trebuie să creați un jurnal pentru contul "
+"\"%(account)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr "Només es permet un diari per compte bancari."
+msgstr "Este permis un singur jurnal pentru fiecare cont bancar."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
-"Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
-"l'extracte \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
-msgstr "Per eliminar el extracte \"%(statement)s\" primer l'heu de cancel·lar."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
-"La validació dels extractes eliminarà de les línies dels extractes les "
-"factures ja pagades o cancel·lades."
+
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
-"La validació dels extractes eliminarà les factures pagades en altres "
-"extractes."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
-"Por comptabilitzar l'extracte \"%(statement)s\" heu de crear línies per "
-"l'import \"%(amount)s\" pendent de l'origen \"%(origin)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_end_balance"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have end "
 "balance of %(end_balance)s instead of %(amount)s."
 msgstr ""
-"Per validar l'extracte \"%(statement)s\" heu de canviar les seves línies per"
-" a tenir un balanç final de %(end_balance)s en comptes de %(amount)s."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_add"
 msgid "To validate statement \"%(statement)s\" you must add %(n)s line(s)."
-msgstr "Per validar el extracte \"%(statement)s\" heu d'afegir %(n)s línie(s)."
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_remove"
 msgid "To validate statement \"%(statement)s\" you must remove %(n)s line(s)."
-msgstr "Per validar el extracte \"%(statement)s\" heu d'eliminar %(n)s línie(s)."
+msgstr ""
+"Pentru a valida extrasul \"%(statement)s\" trebuie să eliminați rândurile "
+"%(n)s."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_wrong_total_amount"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have total "
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
-"Per validar l'extracte \"%(statement)s\" heu de canviar les seves línies per"
-" a tenir un import total de %(total_amount)s en comptes de %(amount)s."
+"Pentru a valida extrasul \"%(statement)s\" trebuie să modificați rândurile "
+"pentru a avea o cantitate totală de %(total_amount)s în loc de %(amount)s."
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr "Esteu segurs que voleu comptabilitzar l'extracte?"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancel·la"
+msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Ciornă"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Comptabilitza"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Concilia"
+msgstr "Reconciliere"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Valida"
+msgstr "Validare"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr "Usuari a les empreses"
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr "Usuari a les empreses"
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Grups de línies"
+msgstr "Grupuri de rânduri"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Extractes"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Extractes"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Importa extracte"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Diaris d'extracte"
+msgstr "Extras de cont"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Extractes"
+msgstr ""
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Extracte"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Suma"
 
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Cancel·lat"
+msgstr "Anulat"
 
 msgctxt "report:account.statement:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "report:account.statement:"
 msgid "Date:"
 msgstr "Data:"
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Descripció"
+msgstr "Descriere"
 
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Ciornă"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Diari:"
+msgstr "Jurnal:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Número"
+msgstr "Număr"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Parte"
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Extracte"
+msgstr "Extras de cont"
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr "Total"
 
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Extracte"
+msgstr ""
 
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Cancel·lat"
+msgstr "Anulat"
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Ciornă"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Comptabilitzat"
+msgstr ""
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
 msgstr "Validat"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Suma"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr "Sold"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Nombre de línies"
+msgstr "Numărul de rânduri"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Informació addicional"
+msgstr "Alte Informaţii"
 
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Línies extracte"
+msgstr ""
 
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Cancel·la"
+msgstr "Anulare"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Importa"
+msgstr "Import"
```

### Comparing `trytond_account_statement-7.0.2/locale/cs.po` & `trytond_account_statement-7.2.0/locale/cs.po`

 * *Files 8% similar despite different names*

```diff
@@ -122,18 +122,26 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr ""
@@ -163,27 +171,35 @@
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr ""
@@ -201,31 +217,43 @@
 msgid "Number"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr ""
@@ -250,14 +278,18 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
@@ -368,23 +400,23 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -397,14 +429,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
```

### Comparing `trytond_account_statement-7.0.2/locale/de.po` & `trytond_account_statement-7.2.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,27 @@
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Unternehmen"
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Datum"
@@ -158,26 +167,35 @@
 msgid "Party Required"
 msgstr "Partei erforderlich"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr "Zugeordnet zu"
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Währung"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Kontoauszug"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr "Kontoauszugsstatus"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Datum"
@@ -194,30 +212,44 @@
 msgid "Number"
 msgstr "Nummer"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Partei"
 
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Währung"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Kontoauszug"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Unternehmen"
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "Datum"
@@ -242,14 +274,19 @@
 msgid "Party"
 msgstr "Partei"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "Ausstehender Betrag"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Währung"
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Kontoauszug"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
 msgstr "Kontoauszug ID"
@@ -353,30 +390,27 @@
 msgstr "Festgeschrieben"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Geprüft"
 
+msgctxt "model:ir.message,text:msg_bank_account_currency"
+msgid ""
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "Um den Kontoauszug importieren zu können, muss ein Journal für Konto "
 "\"%(account)s\" erstellt werden."
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
-msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
-msgstr ""
-"Um den Kontoauszug importieren zu können, muss für das Journal "
-"\"%(journal)s\" die Währung \"%(currency)s\" verwendet werden anstatt "
-"\"%(journal_currency)s\"."
-
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Es ist nur ein Journal pro Bankkonto erlaubt."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
@@ -393,14 +427,36 @@
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 "Die Validierung der Kontoauszüge wird bereits bezahlte oder stornierte "
 "Rechnungen von den Kontoauszugspositionen entfernen."
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Damit der Buchungssatz \"%(move)s\" festgeschrieben werden kann, muss zuerst"
+" der Auszug \"%(statement)s\" festgeschrieben werden."
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Damit der Buchungssatz \"%(move)s\" festgeschrieben werden kann, muss zuerst"
+" der Auszug \"%(statement)s\" festgeschrieben werden."
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 "Die Validierung des Kontoauszugs wird bezahlte Rechnungen von anderen "
 "Kontoauszügen entfernen."
```

### Comparing `trytond_account_statement-7.0.2/locale/es.po` & `trytond_account_statement-7.2.0/locale/ca.po`

 * *Files 7% similar despite different names*

```diff
@@ -12,580 +12,636 @@
 
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Data"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
 msgstr "Saldo final"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Diari"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Líneas"
+msgstr "Línies"
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Número de líneas"
+msgstr "Nombre de línies"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Archivo origen"
+msgstr "Fitxer origen"
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr "Identificador archivo origen"
+msgstr "Identificador fitxer origen"
 
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Orígenes"
+msgstr "Orígens"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
 msgstr "Saldo inicial"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Estat"
 
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Por conciliar"
+msgstr "Per conciliar"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Importe total"
+msgstr "Import total"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Validación"
+msgstr "Validació"
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Archivo"
+msgstr "Fitxer"
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Formato del archivo"
+msgstr "Format del fitxer"
 
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Compte"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Cuenta bancaria"
+msgstr "Compte bancari"
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Tercero de la empresa"
+msgstr "Tercer de l'empresa"
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Diari"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Tipo de validación"
+msgstr "Tipus de validació"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Compte"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Import"
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Empresa"
 
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Tercer de l'empresa"
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Data"
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Descripció"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Asiento contable"
+msgstr "Assentament comptable"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
 msgstr "Número"
 
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
 msgstr "Origen"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tercer"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
-msgstr "Tercero obligatorio"
+msgstr "Tercer obligatori"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
-msgstr "Relacionado con"
+msgstr "Relacionat amb"
+
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Moneda"
 
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Estado del extracto"
+msgstr "Estat de l'extracte"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Import"
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Data"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Diari"
 
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Asiento"
+msgstr "Assentament"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
 msgstr "Número"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tercer"
+
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Moneda"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Compte"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Import"
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Empresa"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Tercer de l'empresa"
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Data"
 
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Descripció"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Información"
+msgstr "Informació"
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Líneas"
+msgstr "Línies"
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
 msgstr "Número"
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tercer"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Importe pendiente"
+msgstr "Import pendent"
+
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Moneda"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "ID del Extracto"
+msgstr "ID del Extracte"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Estado del extracto"
+msgstr "Estat de l'extracte"
 
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Extracto bancario"
+msgstr "Extracte bancari"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr "Inicio importación extracto"
+msgstr "Inici importació extracte"
 
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Diario de extracto"
+msgstr "Diari d'extracte"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Línea de extracto bancario"
+msgstr "Línia d'extracte bancari"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Grupo de líneas de extracto"
+msgstr "Grup de línies d'extracte"
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Origen extracto"
+msgstr "Origen Extracte"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr "Información origen extracto"
+msgstr "Informació origen extracte"
 
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Grupos de líneas"
+msgstr "Grups de línies"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Grupos de líneas"
+msgstr "Grups de línies"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Apuntes"
+msgstr "Apunts"
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Asientos"
+msgstr "Assentaments"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Conciliar extractos"
+msgstr "Concilia extractes"
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Extractes"
 
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Diarios de extracto"
+msgstr "Diaris d'extracte"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Líneas de extracto"
+msgstr "Línies d'extracte"
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Líneas de extracto"
+msgstr "Línies d'extracte"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Orígenes"
+msgstr "Orígens"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Importar extracto"
+msgstr "Importa extracte"
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Esborrany"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Contabilizado"
+msgstr "Comptabilitzat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Validado"
+msgstr "Validat"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
-"Para importar extractos, debe crear un diario para la cuenta "
-"\"%(account)s\"."
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
-"Para importar extractos, el diario \"%(journal)s\" debe tener la moneda "
-"\"%(currency)s\" en lugar de \"%(journal_currency)s\"."
+"Per importar l'extracte heu de crear un diari per al compte \"%(account)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr "Solo se permite un diario por cuenta bancaria."
+msgstr "Només es permet un diari per compte bancari."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
-"Para contabilizar el asiento \"%(move)s\" teneis que contabilizar el "
-"extracto \"%(statement)s\"."
+"Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
+"l'extracte \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
-msgstr "Para eliminar el extracto \"%(statement)s\" debe cancelarlo."
+msgstr "Per eliminar el extracte \"%(statement)s\" primer l'heu de cancel·lar."
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
-"La validación de los extractos eliminará de las líneas de los extractos las "
-"facturas ya pagadas o canceladas."
+"La validació dels extractes eliminarà de les línies dels extractes les "
+"factures ja pagades o cancel·lades."
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
+"l'extracte \"%(statement)s\"."
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
+"l'extracte \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
-"La validación de los extractos eliminará las facturas pagadas en otros "
-"extractos."
+"La validació dels extractes eliminarà les factures pagades en altres "
+"extractes."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
-"Para contabilizar el extracto \"%(statement)s\" debe crear líneas por "
-"%(amount)s pendiente del origen \"%(origin)s\"."
+"Por comptabilitzar l'extracte \"%(statement)s\" heu de crear línies per "
+"l'import \"%(amount)s\" pendent de l'origen \"%(origin)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_end_balance"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have end "
 "balance of %(end_balance)s instead of %(amount)s."
 msgstr ""
-"Para validar el extracto \"%(statement)s\" debe modificar las líneas para "
-"tener un saldo final de %(end_balance)s en lugar de %(amount)s."
+"Per validar l'extracte \"%(statement)s\" heu de canviar les seves línies per"
+" a tenir un balanç final de %(end_balance)s en comptes de %(amount)s."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_add"
 msgid "To validate statement \"%(statement)s\" you must add %(n)s line(s)."
-msgstr "Para validar el extracto \"%(statement)s\" debe añadir %(n)s línea(s)."
+msgstr "Per validar el extracte \"%(statement)s\" heu d'afegir %(n)s línie(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_remove"
 msgid "To validate statement \"%(statement)s\" you must remove %(n)s line(s)."
-msgstr "Para validar el extracto \"%(statement)s\" debe eliminar %(n)s línea(s)."
+msgstr "Per validar el extracte \"%(statement)s\" heu d'eliminar %(n)s línie(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_total_amount"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have total "
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
-"Para validar el extracto \"%(statement)s\" debe modificar las líneas para "
-"tener un importe total de %(total_amount)s en lugar de %(amount)s."
+"Per validar l'extracte \"%(statement)s\" heu de canviar les seves línies per"
+" a tenir un import total de %(total_amount)s en comptes de %(amount)s."
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr "¿Estás seguro que quieres contabilizar el extracto?"
+msgstr "Esteu segurs que voleu comptabilitzar l'extracte?"
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Cancel·la"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Esborrany"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Contabilizar"
+msgstr "Comptabilitza"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Conciliar"
+msgstr "Concilia"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Validar"
+msgstr "Valida"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Grupos de líneas"
+msgstr "Grups de línies"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Extractes"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Extractes"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Importar extracto"
+msgstr "Importa extracte"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Diarios de extracto"
+msgstr "Diaris d'extracte"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Extractes"
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Import"
 
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Cancel·lat"
 
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Data"
 
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Fecha:"
+msgstr "Data:"
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Descripció"
 
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Esborrany"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Diario:"
+msgstr "Diari:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
 msgstr "Número"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tercer"
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr "Total"
 
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Extracte"
 
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Cancel·lat"
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Esborrany"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Contabilizado"
+msgstr "Comptabilitzat"
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validado"
+msgstr "Validat"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Import"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Número de líneas"
+msgstr "Nombre de línies"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Información adicional"
+msgstr "Informació addicional"
 
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Líneas de extracto"
+msgstr "Línies extracte"
 
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Cancel·la"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Importar"
+msgstr "Importa"
```

### Comparing `trytond_account_statement-7.0.2/locale/es_419.po` & `trytond_account_statement-7.2.0/locale/fi.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
@@ -16,19 +16,19 @@
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Saldo Final"
+msgstr ""
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Libro diario"
+msgstr ""
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
@@ -42,29 +42,31 @@
 msgid "Origin File"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr ""
+msgstr "Origins"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Saldo Inicial"
+msgstr ""
 
 msgctxt "field:account.statement,state:"
 msgid "State"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr ""
+msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
 msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
@@ -100,15 +102,15 @@
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Libro diario"
+msgstr ""
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
@@ -118,18 +120,26 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr ""
@@ -142,83 +152,106 @@
 msgid "Account Move"
 msgstr ""
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origins"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
 msgstr ""
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Estado del estado de cuenta"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Libro diario"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
 msgstr "Moves"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr ""
@@ -243,145 +276,145 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Estado del estado de cuenta"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Estado de cuenta"
+msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Libro diario de estado de cuenta"
+msgstr "Statement Journals"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Línea de estado de cuenta"
+msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Grupo de líneas de estado de cuenta"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Línea de estado de cuenta"
+msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr ""
+msgstr "Line Groups"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr ""
+msgstr "Line Groups"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr ""
+msgstr "Move Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
 msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr ""
+msgstr "Reconcile Statements"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Estado de cuenta"
+msgstr "Statements"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Libro diario de estado de cuenta"
+msgstr "Statement Journals"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Líneas de estado de cuenta"
+msgstr "Statement Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Líneas de estado de cuenta"
+msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr ""
+msgstr "Origins"
 
-#, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr ""
+msgstr "Import Statement"
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr ""
+msgstr "Posted"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr ""
+msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -394,14 +427,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -430,169 +479,171 @@
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Anular"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr ""
+msgstr "Post"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr ""
+msgstr "Reconcile"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr ""
+msgstr "Validate"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr ""
+msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Estado de cuenta"
+msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Estado de cuenta"
+msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr ""
+msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Libro diario de estado de cuenta"
+msgstr "Statement Journals"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Estado de cuenta"
+msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
-msgstr ""
+msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
 msgstr ""
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Anulado"
+msgstr "Cancel"
 
 msgctxt "report:account.statement:"
 msgid "Date"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Description"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Libro diario:"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Number"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Estado de cuenta"
+msgstr "Statement"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Anulado"
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr ""
+msgstr "Posted"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr ""
+msgstr "Validate"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
 msgstr ""
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Líneas de estado de cuenta"
+msgstr "Statement Lines"
 
 #, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Anular"
+msgstr "Cancel"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_statement-7.0.2/locale/et.po` & `trytond_account_statement-7.2.0/locale/pl.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,406 +1,460 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Ettevõte"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr ""
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Kuupäev"
+msgstr ""
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Lõppsaldo"
+msgstr ""
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Andmik"
+msgstr ""
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Read"
+msgstr ""
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Nimetus"
+msgstr ""
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Ridade arv"
+msgstr ""
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Algfail"
+msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr "Algfaili ID"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Päritolu"
+msgstr "Origins"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Algsaldo"
+msgstr ""
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Olek"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Nettimiseks"
+msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Koguväärtus"
+msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Valideerimine"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Ettevõte"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Fail"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Faili formaat"
+msgstr ""
 
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Pangakonto"
+msgstr ""
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Ettevõte"
+msgstr ""
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Ettevõtte osapool"
+msgstr ""
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr ""
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Andmik"
+msgstr ""
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Nimetus"
+msgstr ""
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Valideerimise tüüp"
+msgstr ""
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Väärtus"
+msgstr ""
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Ettevõte"
+msgstr ""
+
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr ""
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Kuupäev"
+msgstr ""
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Kirjeldus"
+msgstr ""
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Konto kanne"
+msgstr ""
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Number"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Päritolu"
+msgstr "Origins"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr ""
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Aruande staatus"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Väärtus"
+msgstr ""
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Kuupäev"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Andmik"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Kanne"
+msgstr "Moves"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Number"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Osapoole"
+msgstr ""
+
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Väärtus"
+msgstr ""
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Ettevõte"
+msgstr ""
+
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr ""
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Kuupäev"
+msgstr ""
 
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Kirjeldus"
+msgstr ""
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Informatsioon"
+msgstr ""
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Read"
+msgstr ""
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Number"
+msgstr ""
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Avatud väärtus"
+msgstr ""
+
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Aruande ID"
+msgstr "Statement"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Aruande staatus"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Konto aruanne"
+msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr "Aruande impordi käivitus"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Aruande andmik"
+msgstr "Statement Journals"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Konto aruande rida"
+msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Konto aruande rea grupp"
+msgstr ""
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Konto aruand sisend"
+msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr "Aruande sisendinformatisoon"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Rea grupid"
+msgstr "Line Groups"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Rea grupid"
+msgstr "Line Groups"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Kande read"
+msgstr "Move Lines"
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Kanded"
+msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Neti aruanded"
+msgstr "Reconcile Statements"
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Aruanded"
+msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Aruande andmikud"
+msgstr "Statement Journals"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Aruande read"
+msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Aruande read"
+msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Päritolu"
+msgstr "Origins"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Impordi aruanne"
+msgstr "Import Statement"
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "Kõik"
+msgstr "All"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Mustand"
+msgstr "Draft"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Positatud"
+msgstr "Posted"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Valideeritud"
+msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
-msgstr "Aruande valideerimine eemaldab taustud arved teistest aruannetest."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
-msgstr "Aruande valideerimine eemaldab taustud arved teistest aruannetest."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
 
@@ -426,161 +480,168 @@
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Tühista"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Mustand"
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Postita"
+msgstr "Post"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Saldeeri"
+msgstr "Reconcile"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Kinnita"
+msgstr "Validate"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr "Kasutaja ettevõttes"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr "Kasutaja ettevõttes"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Rea grupid"
+msgstr "Line Groups"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Aruanded"
+msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Aruanded"
+msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Impordi aruanded"
+msgstr "Import Statement"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Aruande andmik"
+msgstr "Statement Journals"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Aruanded"
+msgstr "Statements"
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 msgctxt "report:account.statement:"
 msgid "#"
-msgstr "#"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Summa"
+msgstr ""
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Tühistatud"
+msgstr "Cancel"
 
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Kuupäev"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Kuupäev:"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Kirjeldus"
+msgstr ""
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Mustand"
+msgstr "Draft"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Andmik:"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Number"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Osapool"
+msgstr ""
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Kokku"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Aruanne"
+msgstr "Statement"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Tühistatud"
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Mustand"
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Postitatud"
+msgstr "Posted"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Valideeri"
+msgstr "Validated"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Summa"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Ridade arv"
+msgstr ""
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Muu info"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Aruande read"
+msgstr "Statement Lines"
 
+#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Tühista"
+msgstr "Cancel"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Import"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_statement-7.0.2/locale/fa.po` & `trytond_account_statement-7.2.0/locale/fa.po`

 * *Files 9% similar despite different names*

```diff
@@ -119,19 +119,28 @@
 msgid "Account"
 msgstr "حساب"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "مقدار"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "شرکت"
 
 #, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "شرکت نهاد/سازمان"
+
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "واحد پول"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "تاریخ"
@@ -160,26 +169,35 @@
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "واحد پول"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "بیانیه"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr "وضعیت بیانیه"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "مقدار"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "واحد پول"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "تاریخ"
@@ -196,31 +214,45 @@
 msgid "Number"
 msgstr "شماره"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "نهاد/سازمان"
 
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "واحد پول"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "بیانیه"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "حساب"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "مقدار"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "شرکت"
 
 #, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "شرکت نهاد/سازمان"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "واحد پول"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "تاریخ"
@@ -246,14 +278,19 @@
 msgid "Party"
 msgstr "نهاد/سازمان"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "مقدار معلق"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "واحد پول"
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "بیانیه"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
 msgstr "شناسه بیانیه"
@@ -359,29 +396,27 @@
 msgstr "ارسال شده"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "تایید شده"
 
+msgctxt "model:ir.message,text:msg_bank_account_currency"
+msgid ""
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "برای وارد کردن اضهارنامه، باید یک روزنامه برای حساب: \"%(account)s\" ایجاد "
 "کنید."
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
-msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
-msgstr ""
-"برای وارد کردن اضهارنامه، روزنامه : \"%(journal)s\" باید دارای ارز : "
-"\"%(currency)s\"بجای: \"%(journal_currency)s\" باشد."
-
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "در هر حساب بانکی تنها یک روزنامه مجاز است."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
@@ -395,14 +430,30 @@
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 "اعتبار این اظهارانامه، صورتحساب های پرداخت شده را از اظهارنامه های دیگر حذف "
 "خواهد کرد."
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 "اعتبار این اظهارانامه، صورتحساب های پرداخت شده را از اظهارنامه های دیگر حذف "
 "خواهد کرد."
```

### Comparing `trytond_account_statement-7.0.2/locale/fi.po` & `trytond_account_statement-7.2.0/locale/tr.po`

 * *Files 11% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Yevmiye Defteri:"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
@@ -100,17 +101,18 @@
 msgid "Company Party"
 msgstr ""
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Yevmiye Defteri:"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
@@ -120,18 +122,26 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr ""
@@ -140,90 +150,115 @@
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr ""
+msgstr "Sayı"
 
 #, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
 msgstr "Origins"
 
+#, fuzzy
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parti"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Yevmiye Defteri:"
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
 msgstr "Moves"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr ""
+msgstr "Sayı"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
+msgstr "Parti"
+
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr ""
@@ -236,44 +271,50 @@
 msgid "Information"
 msgstr ""
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr ""
+msgstr "Sayı"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parti"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Statement"
+msgstr "Açıklama"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
 msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
@@ -317,19 +358,19 @@
 msgid "Moves"
 msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
 msgstr "Reconcile Statements"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Açıklama"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
 msgstr "Statement Lines"
@@ -338,17 +379,18 @@
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
 msgstr "Origins"
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
@@ -366,23 +408,23 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -395,14 +437,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -464,40 +522,42 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Açıklama"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Açıklama"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Açıklama"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
 msgstr ""
@@ -522,37 +582,36 @@
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr ""
+msgstr "Yevmiye Defteri:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr ""
+msgstr "Sayı"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr ""
+msgstr "Parti"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Açıklama"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
 msgstr "Cancel"
 
 #, fuzzy
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_statement-7.0.2/locale/fr.po` & `trytond_account_statement-7.2.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,27 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Montant"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Société"
 
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Tiers de la société"
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Date"
@@ -158,26 +167,35 @@
 msgid "Party Required"
 msgstr "Tiers requis"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr "Relative à"
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Devise"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Relevé"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr "État du relevé"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Montant"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Date"
@@ -194,30 +212,44 @@
 msgid "Number"
 msgstr "Numéro"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Tiers"
 
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Devise"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Relevé"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Montant"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Société"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Tiers de la société"
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Devise"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "Date"
@@ -242,14 +274,19 @@
 msgid "Party"
 msgstr "Tiers"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "Montant en attente"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Devise"
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Relevé"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
 msgstr "ID du relevé"
@@ -353,29 +390,27 @@
 msgstr "Comptabilisés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validés"
 
+msgctxt "model:ir.message,text:msg_bank_account_currency"
+msgid ""
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "Pour importer le relevé, vous devez créer un journal pour le compte "
 "« %(account)s »."
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
-msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
-msgstr ""
-"Pour importer le relevé, le journal « %(journal)s » doit avoir la devise "
-"« %(currency)s » au lieu de « %(journal_currency)s »."
-
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Seulement un journal est permis par compte bancaire."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
@@ -390,14 +425,34 @@
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 "La validation des relevés enlèvera les factures déjà payées ou annulées des "
 "lignes des relevés."
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Pour supprimer la ligne « %(line)s », vous devez annuler ou réinitialiser à "
+"l'état brouillon le relevé « %(statement)s »."
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Pour supprimer l'origine « %(origin)s », vous devez annuler ou réinitialiser"
+" à l'état brouillon le relevé « %(statement)s »."
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 "La validation des relevés enlèvera les factures payées des autres relevés."
```

### Comparing `trytond_account_statement-7.0.2/locale/hu.po` & `trytond_account_statement-7.2.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,405 +1,459 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Egyenlegkülönbség"
+msgstr "Saldo"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Cég"
+msgstr "Ettevõte"
 
+#, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Kuupäev"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Záró egyenleg"
+msgstr "Lõppsaldo"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Számlakivonat napló"
+msgstr "Andmik"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Sorok"
+msgstr "Read"
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Név"
+msgstr "Nimetus"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Sorok száma"
+msgstr "Ridade arv"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Forrásfájl"
+msgstr "Algfail"
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr ""
+msgstr "Algfaili ID"
 
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Forrásadatok"
+msgstr "Päritolu"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Nyitó egyenleg"
+msgstr "Algsaldo"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Állapot"
+msgstr "Olek"
 
-#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Reconcile"
+msgstr "Nettimiseks"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Sorok összege"
+msgstr "Koguväärtus"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr ""
+msgstr "Valideerimine"
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Cég"
+msgstr "Ettevõte"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Fájl"
+msgstr "Fail"
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Formátum"
+msgstr "Faili formaat"
 
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Könyvviteli számla"
+msgstr "Konto"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Bankszámlaszám"
+msgstr "Pangakonto"
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Cég"
+msgstr "Ettevõte"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr ""
+msgstr "Ettevõtte osapool"
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Pénzügyi napló"
+msgstr "Andmik"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Név"
+msgstr "Nimetus"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Ellenőrzés módja"
+msgstr "Valideerimise tüüp"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Könyvviteli számla"
+msgstr "Konto"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Összeg"
+msgstr "Väärtus"
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Cég"
+msgstr "Ettevõte"
 
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Ettevõtte osapool"
+
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Kuupäev"
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Megjegyzés"
+msgstr "Kirjeldus"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Bizonylat"
+msgstr "Konto kanne"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Szám"
+msgstr "Number"
 
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Eredet"
+msgstr "Päritolu"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Ügyfél"
+msgstr "Osapool"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valuuta"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Aruande staatus"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Összeg"
+msgstr "Väärtus"
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Kuupäev"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Számlakivonat napló"
+msgstr "Andmik"
 
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Bizonylat"
+msgstr "Kanne"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Szám"
+msgstr "Number"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Ügyfél"
+msgstr "Osapoole"
+
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Könyvviteli számla"
+msgstr "Konto"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Összeg"
+msgstr "Väärtus"
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Cég"
+msgstr "Ettevõte"
+
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Ettevõtte osapool"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Kuupäev"
 
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Megjegyzés"
+msgstr "Kirjeldus"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Információk"
+msgstr "Informatsioon"
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Sorok"
+msgstr "Read"
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Szám"
+msgstr "Number"
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Ügyfél"
+msgstr "Osapool"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Fennmaradó összeg"
+msgstr "Avatud väärtus"
+
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Valuuta"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Statement"
+msgstr "Aruande ID"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Aruande staatus"
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Konto aruanne"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr ""
+msgstr "Aruande impordi käivitus"
 
-#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Statement Journals"
+msgstr "Aruande andmik"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Bankszámlakivonat sor"
+msgstr "Konto aruande rida"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr ""
+msgstr "Konto aruande rea grupp"
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr ""
+msgstr "Konto aruand sisend"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr ""
+msgstr "Aruande sisendinformatisoon"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Csoportosított számlakivonat sorok"
+msgstr "Rea grupid"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Csoportosított számlakivonat sorok"
+msgstr "Rea grupid"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Könyvelési tételek"
+msgstr "Kande read"
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Bizonylatok"
+msgstr "Kanded"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Reconcile Statements"
+msgstr "Neti aruanded"
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Bankszámlakivonatok"
+msgstr "Aruanded"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Aruande andmikud"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Számlakivonat sorok"
+msgstr "Aruande read"
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Számlakivonat sorok"
+msgstr "Aruande read"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Forrásadatok"
+msgstr "Päritolu"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Bankszámlakivonat beolvasása"
+msgstr "Impordi aruanne"
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "összes"
+msgstr "Kõik"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "vázlat"
+msgstr "Mustand"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "lekönyvelt"
+msgstr "Positatud"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "jóváhagyott"
+msgstr "Valideeritud"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
+msgstr "Aruande valideerimine eemaldab taustud arved teistest aruannetest."
+
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
-msgstr ""
+msgstr "Aruande valideerimine eemaldab taustud arved teistest aruannetest."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
 
@@ -421,161 +475,165 @@
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have total "
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr "Biztos, hogy rögzíteni akarja a bankszámlakivonatot?"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Érvénytelenítés"
+msgstr "Tühista"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "vázlat"
+msgstr "Mustand"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Rögzítés"
+msgstr "Postita"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Egyeztetés"
+msgstr "Saldeeri"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Jóváhagyás"
+msgstr "Kinnita"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Kasutaja ettevõttes"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Kasutaja ettevõttes"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Csoportosított számlakivonat sorok"
+msgstr "Rea grupid"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Bankszámlakivonatok"
+msgstr "Aruanded"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Bankszámlakivonatok"
+msgstr "Aruanded"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Bankszámlakivonat beolvasása"
+msgstr "Impordi aruanded"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Aruande andmik"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Bankszámlakivonatok"
+msgstr "Aruanded"
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Összeg"
+msgstr "Summa"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "érvénytelen"
+msgstr "Tühistatud"
 
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Kuupäev"
 
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Dátum:"
+msgstr "Kuupäev:"
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Leírás"
+msgstr "Kirjeldus"
 
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "vázlat"
+msgstr "Mustand"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Számlakivonat napló:"
+msgstr "Andmik:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Szám"
+msgstr "Number"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Ügyfél"
+msgstr "Osapool"
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Összesen"
+msgstr "Kokku"
 
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Bankszámlakivonat"
+msgstr "Aruanne"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "érvénytelen"
+msgstr "Tühistatud"
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "vázlat"
+msgstr "Mustand"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "lekönyvelt"
+msgstr "Postitatud"
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "jóváhagyott"
+msgstr "Valideeri"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "sorok összege alapján"
+msgstr "Summa"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "záróegyenleg alapján"
+msgstr "Saldo"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "sorok száma alapján"
+msgstr "Ridade arv"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Egyéb info"
+msgstr "Muu info"
 
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Számlakivonat sorok"
+msgstr "Aruande read"
 
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Mégse"
+msgstr "Tühista"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Beolvasás"
+msgstr "Import"
```

### Comparing `trytond_account_statement-7.0.2/locale/id.po` & `trytond_account_statement-7.2.0/locale/id.po`

 * *Files 11% similar despite different names*

```diff
@@ -118,18 +118,27 @@
 msgid "Account"
 msgstr "Akun"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Jumlah"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Pihak Perusahaan"
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Tanggal"
@@ -158,26 +167,35 @@
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Mata Uang"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Pernyataan"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Jumlah"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Tanggal"
@@ -194,30 +212,44 @@
 msgid "Number"
 msgstr "Nomor"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Pihak"
 
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Mata Uang"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Pernyataan"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "Akun"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Jumlah"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Perusahaan"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Pihak Perusahaan"
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "Tanggal"
@@ -242,14 +274,19 @@
 msgid "Party"
 msgstr "Pihak"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Mata Uang"
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Pernyataan"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
 msgstr ""
@@ -356,23 +393,23 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -385,14 +422,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
```

### Comparing `trytond_account_statement-7.0.2/locale/it.po` & `trytond_account_statement-7.2.0/locale/pt.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,313 +4,339 @@
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Empresa"
 
 #, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Moeda"
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Saldo finale"
+msgstr "Saldo Final"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Registro"
+msgstr "Diário"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Righe"
+msgstr "Linhas"
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Numero di Righe"
+msgstr "Número de linhas"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr ""
+msgstr "Arquido de origem"
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr ""
+msgstr "ID do Arquivo de Origem"
 
-#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Origins"
+msgstr "Origens"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Saldo iniziale"
+msgstr "Saldo Inicial"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Stato"
+msgstr "Estado"
 
 #, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
 msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Importo Totale"
+msgstr "Montante Total"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Convalida"
+msgstr "Validação"
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Empresa"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr ""
+msgstr "Arquivo"
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr ""
+msgstr "Formato do arquivo"
 
 #, fuzzy
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Conto"
+msgstr "Contas"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr ""
+msgstr "Conta Bancária"
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Empresa"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr ""
+msgstr "Pessoa da Empresa"
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Moeda"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Registro"
+msgstr "Diário"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
 msgstr "Nome"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Metodo convalida"
+msgstr "Tipo de Validação"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Conto"
+msgstr "Contas"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Quantidade"
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Empresa"
+
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Pessoa da Empresa"
 
 #, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Moeda"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Descrição"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Movimento contabile"
+msgstr "Lançamento Contábil"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Numero"
+msgstr "Número"
 
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr "Origem"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Parceiro"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Moeda"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Situazione"
+msgstr "Extrato"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Stato del documento"
+msgstr "Estado do Extrato"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Quantidade"
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Moeda"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Registro"
+msgstr "Diário"
 
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Movimento"
+msgstr "Lançamento"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Numero"
+msgstr "Número"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Parceiro"
+
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Moeda"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Registro"
+msgstr "Extrato"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Conto"
+msgstr "Conta"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Quantidade"
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Empresa"
+
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Pessoa da Empresa"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Moeda"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Descrição"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr ""
+msgstr "Informações"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Righe"
+msgstr "Linhas"
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Numero"
+msgstr "Número"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Pessoa"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr ""
+msgstr "Montante Pendente"
 
 #, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Moeda"
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Situazione"
+msgstr "Extrato"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Situazione"
+msgstr "ID do Extrato"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Stato del documento"
+msgstr "Estado do Extrato"
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Situazione"
+msgstr "Extrato"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Estratto Conto"
+msgstr "Extrato Bancário"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr ""
+msgstr "Iniciar Importação do Extrato"
 
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Estratto Registro"
+msgstr "Diário de Extratos"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Riga estratto conto"
+msgstr "Linha de Extrato Bancário"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Raggruppamento righe estratto conto"
+msgstr "Grupo de Linhas do Extrato"
 
-#, fuzzy
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Riga estratto conto"
+msgstr "Origem do Extrato Bancário"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr ""
+msgstr "Informação da Origem do Extrato"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
 #, fuzzy
@@ -319,17 +345,18 @@
 msgstr "Line Groups"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
 msgstr "Move Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Movimenti"
+msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
 msgstr "Reconcile Statements"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
@@ -347,23 +374,25 @@
 msgstr "Statement Lines"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
 msgstr "Origins"
 
 #, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
 msgstr "Statement"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
@@ -383,28 +412,29 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr ""
+msgstr "Apenas um diário é permitido por conta bancária."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
@@ -412,14 +442,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -450,15 +496,15 @@
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
@@ -466,15 +512,15 @@
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
 msgstr "Reconcile"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Verifica"
+msgstr "Validate"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
@@ -491,22 +537,23 @@
 msgstr "Statements"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Registri documenti"
+msgstr "Statement Journals"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
 msgstr "Statements"
 
 #, fuzzy
@@ -516,99 +563,99 @@
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Quantidade"
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr "Cancelado"
 
 msgctxt "report:account.statement:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "report:account.statement:"
 msgid "Date:"
 msgstr "Data:"
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Descrição"
 
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Bozza"
+msgstr "Rascunho"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Registro:"
+msgstr "Diário:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Numero"
+msgstr "Número"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Parceiro"
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Situazione"
+msgstr "Extrato"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Totale"
+msgstr "Total"
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Situazione"
+msgstr "Extrato"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr "Cancelado"
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Bozza"
+msgstr "Rascunho"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Defnitivo"
+msgstr "Confirmado"
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validato"
+msgstr "Validado"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Quantidade"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Numero di righe"
+msgstr "Número de linhas"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Altre info"
+msgstr "Outras informações"
 
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Righe situazione"
+msgstr "Linhas do Extrato"
 
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancelar"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr ""
+msgstr "Importar"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_statement-7.0.2/locale/lo.po` & `trytond_account_statement-7.2.0/locale/lo.po`

 * *Files 6% similar despite different names*

```diff
@@ -125,20 +125,29 @@
 msgid "Account"
 msgstr "ບັນຊີ"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "ມູນຄ່າ"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "ຫ້ອງການ/ສຳນັກງານ"
 
 #, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 #, fuzzy
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
@@ -174,27 +183,36 @@
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "ມູນຄ່າ"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,date:"
@@ -218,34 +236,48 @@
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "ພາກສ່ວນ"
 
 #, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "ບັນຊີ"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "ມູນຄ່າ"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "ຫ້ອງການ/ສຳນັກງານ"
 
 #, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "ສະກຸນເງິນ"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
@@ -276,14 +308,19 @@
 msgstr "ພາກສ່ວນ"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "ສະກຸນເງິນ"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -396,23 +433,23 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "ກວດສອບແລ້ວ"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -425,14 +462,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
```

### Comparing `trytond_account_statement-7.0.2/locale/lt.po` & `trytond_account_statement-7.2.0/locale/lt.po`

 * *Files 8% similar despite different names*

```diff
@@ -123,19 +123,28 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 #, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Organizacija"
+
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Valiuta"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr ""
@@ -166,26 +175,35 @@
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valiuta"
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Valiuta"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr ""
@@ -204,31 +222,45 @@
 msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Kontrahentas"
 
 #, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Valiuta"
+
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Organizacija"
 
 #, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Organizacija"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Valiuta"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr ""
@@ -254,14 +286,19 @@
 msgstr "Kontrahentas"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Valiuta"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Statement"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -371,23 +408,23 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -400,14 +437,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
```

### Comparing `trytond_account_statement-7.0.2/locale/nl.po` & `trytond_account_statement-7.2.0/locale/nl.po`

 * *Files 8% similar despite different names*

```diff
@@ -118,18 +118,27 @@
 msgid "Account"
 msgstr "Grootboekrekening"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Bedrag"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Bedrijf relatie"
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Datum"
@@ -158,26 +167,35 @@
 msgid "Party Required"
 msgstr "Relatie verplicht"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr "Gerelateerd aan"
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Bankafschrift"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr "Bankafschrift status"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Bedrag"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Datum"
@@ -194,30 +212,44 @@
 msgid "Number"
 msgstr "Nummer"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Relatie"
 
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Bankafschrift"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "Grootboekrekening"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Bedrag"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Bedrijf relatie"
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr "Datum"
@@ -242,14 +274,19 @@
 msgid "Party"
 msgstr "Relatie"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "Bedrag in afwachting"
 
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Bankafschrift"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
 msgstr "Bankafschrift ID"
@@ -353,29 +390,27 @@
 msgstr "Geboekt"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Gevalideerd"
 
+msgctxt "model:ir.message,text:msg_bank_account_currency"
+msgid ""
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "Om bankafschrift te importeren, moet u een dagboek aanmaken voor "
 "bankrekening \"%(account)s\"."
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
-msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
-msgstr ""
-"Om een bankafschrift te importeren, moet het dagboek \"%(journal)s\" de "
-"valuta \"%(currency)s\" hebben in plaats van \"%(journal_currency)s\"."
-
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Per bankrekening is slechts één dagboek toegestaan."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
@@ -392,14 +427,34 @@
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 "De validatie van de bankafschriften zal reeds betaalde of geannuleerde "
 "facturen uit de bankafschriften regels verwijderen."
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Om regel \"%(line)s\" te verwijderen moet u eerst het afschrift "
+"\"%(statement)s\" annuleren of resetten naar concept."
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+"Om de bron \"%(origin)s\" te verwijderen moet u eerst het bankafschrift "
+"\"%(statement)s\" annuleren of terugzetten naar concept."
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 "Validatie van bankafschriften verwijdert betaalde facturen uit andere "
 "bankafschriften."
```

### Comparing `trytond_account_statement-7.0.2/locale/pl.po` & `trytond_account_statement-7.2.0/locale/uk.po`

 * *Files 10% similar despite different names*

```diff
@@ -42,31 +42,29 @@
 msgid "Origin File"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Origins"
+msgstr ""
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
 msgstr ""
 
 msgctxt "field:account.statement,state:"
 msgid "State"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Reconcile"
+msgstr ""
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
 msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
@@ -120,18 +118,26 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr ""
@@ -144,86 +150,102 @@
 msgid "Account Move"
 msgstr ""
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origins"
+msgstr ""
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
 msgstr ""
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Moves"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr ""
@@ -248,45 +270,45 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
 msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Statement Journals"
+msgstr ""
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
 msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
@@ -296,92 +318,90 @@
 msgid "Account Statement Origin"
 msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Move Lines"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Moves"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Reconcile Statements"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Statements"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Origins"
+msgstr ""
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Import Statement"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Posted"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Validated"
+msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -394,14 +414,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -432,145 +468,135 @@
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Post"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Reconcile"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Validate"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Statements"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Statements"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Import Statement"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Statements"
+msgstr ""
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Amount"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Date"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Description"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Number"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Party"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Statement"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Posted"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validated"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
@@ -580,20 +606,18 @@
 msgid "Number of Lines"
 msgstr ""
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
 msgstr ""
```

### Comparing `trytond_account_statement-7.0.2/locale/pt.po` & `trytond_account_statement-7.2.0/locale/zh_CN.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,403 +1,435 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期格式"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Saldo Final"
+msgstr ""
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Diário"
+msgstr ""
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Linhas"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "纳木"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Número de linhas"
+msgstr ""
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Arquido de origem"
+msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr "ID do Arquivo de Origem"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Origens"
+msgstr "Origins"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Saldo Inicial"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "状态"
 
 #, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
 msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Montante Total"
+msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Validação"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Arquivo"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Formato do arquivo"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Contas"
+msgstr ""
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Conta Bancária"
+msgstr ""
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Pessoa da Empresa"
+msgstr ""
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr ""
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Diário"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "纳木"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Tipo de Validação"
+msgstr ""
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Contas"
+msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Quantidade"
+msgstr ""
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
+
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Descrição"
+msgstr "描述"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Lançamento Contábil"
+msgstr ""
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Número"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origem"
+msgstr "Origins"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Parceiro"
+msgstr ""
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Extrato"
+msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Estado do Extrato"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Quantidade"
+msgstr ""
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期格式"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Diário"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Lançamento"
+msgstr "Moves"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Número"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Parceiro"
+msgstr ""
 
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Extrato"
+msgstr "Statement"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Conta"
+msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Quantidade"
+msgstr ""
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
+
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Descrição"
+msgstr "描述"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Informações"
+msgstr ""
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Linhas"
+msgstr ""
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Número"
+msgstr ""
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Pessoa"
+msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Montante Pendente"
+msgstr ""
+
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Extrato"
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "ID do Extrato"
+msgstr "Statement"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Estado do Extrato"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Extrato"
+msgstr "Statement"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Extrato Bancário"
+msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr "Iniciar Importação do Extrato"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Diário de Extratos"
+msgstr "Statement Journals"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Linha de Extrato Bancário"
+msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Grupo de Linhas do Extrato"
+msgstr ""
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Origem do Extrato Bancário"
+msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr "Informação da Origem do Extrato"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
 msgstr "Move Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
 msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
 msgstr "Reconcile Statements"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
 msgstr "Origins"
 
-#, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
 msgstr "Statement"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
 msgstr "Posted"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr "Apenas um diário é permitido por conta bancária."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
@@ -405,14 +437,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -474,135 +522,141 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
 msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
 msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
 msgstr "Statement"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Quantidade"
+msgstr ""
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "取消"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Data:"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Descrição"
+msgstr "描述"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Rascunho"
+msgstr "Draft"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Diário:"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Número"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Parceiro"
+msgstr ""
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Extrato"
+msgstr "Statement"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Total"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Extrato"
+msgstr "Statement"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "取消"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Rascunho"
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Confirmado"
+msgstr "Posted"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validado"
+msgstr "Validate"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Quantidade"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Número de linhas"
+msgstr ""
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Outras informações"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Linhas do Extrato"
+msgstr "Statement Lines"
 
+#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "取消"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Importar"
+msgstr ""
```

### Comparing `trytond_account_statement-7.0.2/locale/ro.po` & `trytond_account_statement-7.2.0/locale/ru.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,283 +1,369 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Sold"
+msgstr "Баланс"
 
+#, fuzzy
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Учет.орг."
 
+#, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "Дата"
 
+#, fuzzy
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr ""
+msgstr "Конец баланса"
 
+#, fuzzy
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr "Журнал"
 
+#, fuzzy
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Строки"
 
+#, fuzzy
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr ""
+msgstr "Правило оплаты"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr ""
+msgstr "Origins"
 
+#, fuzzy
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Sold Initial"
+msgstr "Начальный баланс"
 
+#, fuzzy
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr ""
+msgstr "Статус"
 
+#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr ""
+msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
 msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Учет.орг."
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
 msgstr ""
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr "Счет"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Учет.орг."
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr "Журнал"
 
+#, fuzzy
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr ""
+msgstr "Наименование"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr "Счет"
 
+#, fuzzy
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Сумма"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Учет.орг."
+
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "Дата"
 
+#, fuzzy
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr "Описание"
 
+#, fuzzy
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr ""
+msgstr "Проводка"
 
+#, fuzzy
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr ""
+msgstr "Номер"
 
+#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr "Origins"
 
+#, fuzzy
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Организации"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Валюты"
+
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr ""
+msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Сумма"
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "Дата"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr "Журнал"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr ""
+msgstr "Перемещение"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr ""
+msgstr "Номер"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Организации"
+
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr ""
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr "Счет"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Сумма"
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Учет.орг."
+
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "Дата"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr "Описание"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Informație"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Строки"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr ""
+msgstr "Номер"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Организации"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Валюты"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr ""
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr ""
+msgstr "Statement"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Extras de cont"
+msgstr "Statement"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
 msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr ""
+msgstr "Statement Journals"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
 msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
@@ -287,91 +373,96 @@
 msgid "Account Statement Origin"
 msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr ""
+msgstr "Line Groups"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr ""
+msgstr "Line Groups"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr ""
+msgstr "Move Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr ""
+msgstr "Перемещения"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr ""
+msgstr "Reconcile Statements"
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr ""
+msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Extras de cont"
+msgstr "Statement Journals"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr ""
+msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr ""
+msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr ""
+msgstr "Origins"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr ""
+msgstr "Statement"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr ""
+msgstr "Import Statement"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "Все"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Черновик"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr ""
+msgstr "Проведен"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr ""
+msgstr "Утвержденный"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -384,14 +475,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -422,157 +529,179 @@
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr ""
+msgstr "Post"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr ""
+msgstr "Reconcile"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr ""
+msgstr "Validate"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr ""
+msgstr "Line Groups"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr ""
+msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr ""
+msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr ""
+msgstr "Import Statement"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Extras de cont"
+msgstr "Statement Journals"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr ""
+msgstr "Statements"
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr ""
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
-msgstr ""
+msgstr "#"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Сумма"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Отменено"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Data"
+msgstr "Дата"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Data:"
+msgstr "Дата:"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Descriere"
+msgstr "Описание"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr ""
+msgstr "Черновик"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr ""
+msgstr "Журнал"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr ""
+msgstr "Номер"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Организации"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Extras de cont"
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr ""
+msgstr "Итого"
 
+#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr ""
+msgstr "Statement"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Отменено"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Черновик"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr ""
+msgstr "Проведен"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr ""
+msgstr "Утвержденный"
 
+#, fuzzy
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Сумма"
 
+#, fuzzy
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Sold"
+msgstr "Баланс"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr ""
+msgstr "Другая информация"
 
+#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr ""
+msgstr "Statement Lines"
 
+#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Отменить"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Import"
+msgstr ""
```

### Comparing `trytond_account_statement-7.0.2/locale/ru.po` & `trytond_account_statement-7.2.0/locale/it.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,431 +1,442 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Баланс"
+msgstr "Saldo"
 
-#, fuzzy
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Azienda"
 
 #, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr "Valuta"
 
-#, fuzzy
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Конец баланса"
+msgstr "Saldo finale"
 
-#, fuzzy
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Журнал"
+msgstr "Registro"
 
-#, fuzzy
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Строки"
+msgstr "Righe"
 
-#, fuzzy
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Правило оплаты"
+msgstr "Nome"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr ""
+msgstr "Numero di Righe"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
 msgstr "Origins"
 
-#, fuzzy
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Начальный баланс"
+msgstr "Saldo iniziale"
 
-#, fuzzy
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Статус"
+msgstr "Stato"
 
 #, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
 msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr ""
+msgstr "Importo Totale"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr ""
+msgstr "Convalida"
 
-#, fuzzy
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Azienda"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
 msgstr ""
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Счет"
+msgstr "Conto"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Azienda"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr "Valuta"
 
-#, fuzzy
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Журнал"
+msgstr "Registro"
 
-#, fuzzy
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Nome"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr ""
+msgstr "Metodo convalida"
 
-#, fuzzy
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Счет"
+msgstr "Conto"
 
-#, fuzzy
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Importo"
+
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Azienda"
+
+#, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr "Valuta"
 
-#, fuzzy
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Описание"
+msgstr "Descrizione"
 
-#, fuzzy
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Проводка"
+msgstr "Movimento contabile"
 
-#, fuzzy
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Номер"
+msgstr "Numero"
 
-#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origins"
+msgstr "Origine"
 
-#, fuzzy
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Организации"
+msgstr "Controparte"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Situazione"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Stato del documento"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Importo"
+
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr "Valuta"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Журнал"
+msgstr "Registro"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Перемещение"
+msgstr "Movimento"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Номер"
+msgstr "Numero"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Организации"
+msgstr "Controparte"
 
 #, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Registro"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Счет"
+msgstr "Conto"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Importo"
+
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Azienda"
+
+#, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Data"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Описание"
+msgstr "Descrizione"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Строки"
+msgstr "Righe"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Номер"
+msgstr "Numero"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Организации"
+msgstr "Controparte"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Situazione"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Statement"
+msgstr "Situazione"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Stato del documento"
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Situazione"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr ""
+msgstr "Estratto Conto"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Statement Journals"
+msgstr "Estratto Registro"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr ""
+msgstr "Riga estratto conto"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr ""
+msgstr "Raggruppamento righe estratto conto"
 
+#, fuzzy
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr ""
+msgstr "Riga estratto conto"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
 msgstr "Move Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Перемещения"
+msgstr "Movimenti"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
 msgstr "Reconcile Statements"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
 msgstr "Origins"
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "Все"
+msgstr "All"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Черновик"
+msgstr "Draft"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Проведен"
+msgstr "Posted"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Утвержденный"
+msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -438,14 +449,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -476,15 +503,15 @@
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Annulla"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
@@ -492,163 +519,149 @@
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
 msgstr "Reconcile"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Validate"
+msgstr "Verifica"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
 msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Registri documenti"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
 msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
 msgstr "Statement"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Importo"
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Отменено"
+msgstr "Annullato"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Data"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Дата:"
+msgstr "Data:"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Описание"
+msgstr "Descrizione"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Черновик"
+msgstr "Bozza"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Журнал"
+msgstr "Registro:"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Номер"
+msgstr "Numero"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Организации"
+msgstr "Controparte"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Situazione"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Итого"
+msgstr "Totale"
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Situazione"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Отменено"
+msgstr "Annullato"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Черновик"
+msgstr "Bozza"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Проведен"
+msgstr "Defnitivo"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Утвержденный"
+msgstr "Validato"
 
-#, fuzzy
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Сумма"
+msgstr "Importo"
 
-#, fuzzy
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Баланс"
+msgstr "Saldo"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr ""
+msgstr "Numero di righe"
 
-#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Другая информация"
+msgstr "Altre info"
 
-#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Righe situazione"
 
-#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Annulla"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_statement-7.0.2/locale/sl.po` & `trytond_account_statement-7.2.0/locale/sl.po`

 * *Files 4% similar despite different names*

```diff
@@ -123,20 +123,29 @@
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Znesek"
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Družba"
 
 #, fuzzy
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr "Partner družbe"
+
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr "Datum"
@@ -165,26 +174,35 @@
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Izpisek"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
 msgstr "Stanje izpiska"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Znesek"
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr "Datum"
@@ -201,34 +219,48 @@
 msgid "Number"
 msgstr "Številka"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Partner"
 
+#, fuzzy
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Izpisek"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr "Konto"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Znesek"
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Družba"
 
 #, fuzzy
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr "Partner družbe"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
@@ -259,14 +291,19 @@
 msgstr "Partner"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr "Valuta"
+
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Izpisek"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -387,23 +424,23 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validated"
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -416,14 +453,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
```

### Comparing `trytond_account_statement-7.0.2/locale/tr.po` & `trytond_account_statement-7.2.0/locale/es_419.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr ""
+msgstr "Saldo"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
@@ -16,20 +16,19 @@
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr ""
+msgstr "Saldo Final"
 
-#, fuzzy
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Yevmiye Defteri:"
+msgstr "Libro diario"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
@@ -43,31 +42,29 @@
 msgid "Origin File"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Origins"
+msgstr ""
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr ""
+msgstr "Saldo Inicial"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Reconcile"
+msgstr ""
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
 msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
@@ -101,18 +98,17 @@
 msgid "Company Party"
 msgstr ""
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Yevmiye Defteri:"
+msgstr "Libro diario"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
@@ -122,18 +118,26 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.line,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
 msgstr ""
@@ -142,95 +146,107 @@
 msgid "Description"
 msgstr ""
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Sayı"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origins"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Parti"
+msgstr ""
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:account.statement.line,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Estado del estado de cuenta"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.line.group,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Yevmiye Defteri:"
+msgstr "Libro diario"
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
 msgstr "Moves"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Sayı"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Parti"
+msgstr ""
+
+msgctxt "field:account.statement.line.group,second_currency:"
+msgid "Second Currency"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,amount_second_currency:"
+msgid "Amount Second Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.statement.origin,company_currency:"
+msgid "Company Currency"
+msgstr ""
+
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
 msgstr ""
@@ -243,156 +259,161 @@
 msgid "Information"
 msgstr ""
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Sayı"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Parti"
+msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
+msgctxt "field:account.statement.origin,second_currency:"
+msgid "Second Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Estado del estado de cuenta"
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr ""
+msgstr "Estado de cuenta"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Statement Journals"
+msgstr "Libro diario de estado de cuenta"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr ""
+msgstr "Línea de estado de cuenta"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr ""
+msgstr "Grupo de líneas de estado de cuenta"
 
+#, fuzzy
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr ""
+msgstr "Línea de estado de cuenta"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Move Lines"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
 msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Reconcile Statements"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Libro diario de estado de cuenta"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Líneas de estado de cuenta"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Líneas de estado de cuenta"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Origins"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Import Statement"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Posted"
+msgstr ""
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Validated"
+msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_no_journal"
+msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
-"To import statement, you must create a journal for account \"%(account)s\"."
+"The currency of bank account \"%(bank_account)s\" must be the same as "
+"\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_import_wrong_currency"
+msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
-"To import statement, the journal \"%(journal)s\" must have the currency "
-"\"%(currency)s\" instead of \"%(journal_currency)s\"."
+"To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
@@ -405,14 +426,30 @@
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
+msgid ""
+"To delete line \"%(line)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
+msgid "You must set the same sign for second currency than amount."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
+msgid ""
+"To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
+"\"%(statement)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
@@ -441,172 +478,169 @@
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anular"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Post"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Reconcile"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Validate"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Import Statement"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Libro diario de estado de cuenta"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "report:account.statement:"
 msgid "#"
-msgstr "#"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Amount"
 msgstr ""
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "Anulado"
 
 msgctxt "report:account.statement:"
 msgid "Date"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Date:"
 msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Description"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Yevmiye Defteri:"
+msgstr "Libro diario:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Sayı"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Parti"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Açıklama"
+msgstr "Estado de cuenta"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "Anulado"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Posted"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validate"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr ""
+msgstr "Saldo"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
 msgstr ""
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Líneas de estado de cuenta"
 
 #, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anular"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
 msgstr ""
```

### Comparing `trytond_account_statement-7.0.2/message.xml` & `trytond_account_statement-7.2.0/message.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_account_statement-7.0.2/message.xml` & `trytond_account_statement-7.2.0/message.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data grouped="1">
+    <record model="ir.message" id="msg_bank_account_currency">
+      <field name="text">The currency of bank account &quot;%(bank_account)s&quot; must be the same as &quot;%(currency)s&quot; of the journal &quot;%(journal)s&quot;.</field>
+    </record>
     <record model="ir.message" id="msg_journal_bank_account_unique">
       <field name="text">Only one journal is allowed per bank account.</field>
     </record>
     <record model="ir.message" id="msg_import_no_journal">
       <field name="text">To import statement, you must create a journal for account &quot;%(account)s&quot;.</field>
     </record>
-    <record model="ir.message" id="msg_import_wrong_currency">
-      <field name="text">To import statement, the journal &quot;%(journal)s&quot; must have the currency &quot;%(currency)s&quot; instead of &quot;%(journal_currency)s&quot;.</field>
-    </record>
     <record model="ir.message" id="msg_statement_wrong_end_balance">
       <field name="text">To validate statement &quot;%(statement)s&quot; you must change lines to have end balance of %(end_balance)s instead of %(amount)s.</field>
     </record>
     <record model="ir.message" id="msg_statement_wrong_total_amount">
       <field name="text">To validate statement &quot;%(statement)s&quot; you must change lines to have total amount of %(total_amount)s instead of %(amount)s.</field>
     </record>
     <record model="ir.message" id="msg_statement_wrong_number_of_lines_add">
@@ -32,12 +32,21 @@
     </record>
     <record model="ir.message" id="msg_statement_paid_invoice_draft">
       <field name="text">The validation of the statements will remove paid invoices from other statements.</field>
     </record>
     <record model="ir.message" id="msg_statement_post_pending_amount">
       <field name="text">To post statement &quot;%(statement)s&quot; you must create lines for pending %(amount)s of origin &quot;%(origin)s&quot;.</field>
     </record>
+    <record model="ir.message" id="msg_statement_line_second_currency_sign">
+      <field name="text">You must set the same sign for second currency than amount.</field>
+    </record>
+    <record model="ir.message" id="msg_statement_line_delete_cancel_draft">
+      <field name="text">To delete line &quot;%(line)s&quot; you must cancel or reset to draft statement &quot;%(statement)s&quot;.</field>
+    </record>
+    <record model="ir.message" id="msg_statement_origin_delete_cancel_draft">
+      <field name="text">To delete origin &quot;%(origin)s&quot; you must cancel or reset to draft statement &quot;%(statement)s&quot;.</field>
+    </record>
     <record model="ir.message" id="msg_post_statement_move">
       <field name="text">To post the move &quot;%(move)s&quot; you must post the statement &quot;%(statement)s&quot;.</field>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_statement-7.0.2/setup.py` & `trytond_account_statement-7.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
 def get_require_version(name):
     require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
@@ -55,15 +58,16 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": (
+            'https://docs.tryton.org/modules-account-statement'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement',
     package_dir={'trytond.modules.account_statement': '.'},
     packages=(
         ['trytond.modules.account_statement']
```

### Comparing `trytond_account_statement-7.0.2/statement.fodt` & `trytond_account_statement-7.2.0/statement.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_account_statement-7.0.2/statement.fodt` & `trytond_account_statement-7.2.0/statement.fodt`

```diff
@@ -448,15 +448,15 @@
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
@@ -468,15 +468,15 @@
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
```

### Comparing `trytond_account_statement-7.0.2/statement.py` & `trytond_account_statement-7.2.0/statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sql.conditionals import Coalesce
 from sql.functions import CharLength
 from sql.operators import Concat
 
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
-    DictSchemaMixin, Index, ModelSQL, ModelView, Workflow, fields,
+    Check, DictSchemaMixin, Index, ModelSQL, ModelView, Workflow, fields,
     sequence_ordered)
 from trytond.model.exceptions import AccessError
 from trytond.modules.company import CompanyReport
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
 from trytond.rpc import RPC
@@ -639,22 +639,44 @@
             required=True, ondelete='CASCADE', states=_states)
         statement_state = fields.Function(
             fields.Selection('get_statement_states', "Statement State"),
             'on_change_with_statement_state')
         company = fields.Function(
             fields.Many2One('company.company', "Company"),
             'on_change_with_company', searcher='search_company')
+        company_currency = fields.Function(
+            fields.Many2One('currency.currency', "Company Currency"),
+            'on_change_with_company_currency')
         number = fields.Char("Number")
         date = fields.Date(
             "Date", required=True, states=_states)
         amount = Monetary(
             "Amount", currency='currency', digits='currency', required=True,
             states=_states)
         currency = fields.Function(fields.Many2One(
                 'currency.currency', "Currency"), 'on_change_with_currency')
+        amount_second_currency = Monetary(
+            "Amount Second Currency",
+            currency='second_currency', digits='second_currency',
+            states={
+                'required': Bool(Eval('second_currency')),
+                'readonly': _states['readonly'],
+                })
+        second_currency = fields.Many2One(
+            'currency.currency', "Second Currency",
+            domain=[
+                ('id', '!=', Eval('currency', -1)),
+                If(Eval('currency', -1) != Eval('company_currency', -1),
+                    ('id', '=', Eval('company_currency', -1)),
+                    ()),
+                ],
+            states={
+                'required': Bool(Eval('amount_second_currency')),
+                'readonly': _states['readonly'],
+                })
         party = fields.Many2One(
             'party.party', "Party", states=_states,
             context={
                 'company': Eval('company', -1),
                 },
             depends={'company'})
         account = fields.Many2One(
@@ -696,14 +718,18 @@
         def on_change_with_company(self, name=None):
             return self.statement.company if self.statement else None
 
         @classmethod
         def search_company(cls, name, clause):
             return [('statement.' + clause[0],) + tuple(clause[1:])]
 
+        @fields.depends('statement', '_parent_statement.company')
+        def on_change_with_company_currency(self, name=None):
+            return self.statement.company.currency if self.statement else None
+
         @fields.depends('statement', '_parent_statement.journal')
         def on_change_with_currency(self, name=None):
             if self.statement and self.statement.journal:
                 return self.statement.journal.currency
 
     return Mixin
 
@@ -723,15 +749,18 @@
             ],
         depends=['company'])
     related_to = fields.Reference(
         "Related To", 'get_relations',
         domain={
             'account.invoice': [
                 ('company', '=', Eval('company', -1)),
-                ('currency', '=', Eval('currency', -1)),
+                If(Eval('second_currency'),
+                    ('currency', '=', Eval('second_currency', -1)),
+                    ('currency', '=', Eval('currency', -1))
+                    ),
                 If(Bool(Eval('party')),
                     ['OR',
                         ('party', '=', Eval('party', -1)),
                         ('alternative_payees', '=', Eval('party', -1)),
                         ],
                     []),
                 If(Bool(Eval('account')),
@@ -740,39 +769,49 @@
                 If(Eval('statement_state') == 'draft',
                     ('state', '=', 'posted'),
                     ('state', '!=', '')),
                 ],
             },
         states=_states,
         context={'with_payment': False})
-    origin = fields.Many2One('account.statement.origin', 'Origin',
-        readonly=True,
+    origin = fields.Many2One(
+        'account.statement.origin', 'Origin', readonly=True,
+        ondelete='RESTRICT',
         states={
             'invisible': ~Bool(Eval('origin')),
             },
         domain=[
             ('statement', '=', Eval('statement', -1)),
             ('date', '=', Eval('date', None)),
             ])
     party_required = fields.Function(
         fields.Boolean("Party Required"), 'on_change_with_party_required')
 
     @classmethod
     def __setup__(cls):
         super(Line, cls).__setup__()
+        table = cls.__table__()
         cls.date.states = {
             'readonly': (
                 (Eval('statement_state') != 'draft')
                 | Bool(Eval('origin', 0))),
             }
         cls.account.required = True
         cls.party.states = {
             'required': (Eval('party_required', False)
                 & (Eval('statement_state') == 'draft')),
             }
+        cls._sql_constraints += [
+            ('second_currency_sign',
+                Check(
+                    table,
+                    Coalesce(table.amount_second_currency, 0)
+                    * table.amount >= 0),
+                'account_statement.msg_statement_line_second_currency_sign'),
+            ]
 
     @classmethod
     def __register__(cls, module):
         table = cls.__table__()
 
         super().__register__(module)
 
@@ -927,14 +966,26 @@
         return self.statement.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('statement.rec_name',) + tuple(clause[1:])]
 
     @classmethod
+    def delete(cls, lines):
+        for line in lines:
+            if line.statement_state not in {'cancelled', 'draft'}:
+                raise AccessError(
+                    gettext(
+                        'account_statement.'
+                        'msg_statement_line_delete_cancel_draft',
+                        line=line.rec_name,
+                        sale=line.statement.rec_name))
+        super().delete(lines)
+
+    @classmethod
     def copy(cls, lines, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('move', None)
         default.setdefault('related_to', None)
@@ -1002,31 +1053,36 @@
     def get_move_line(self):
         '''
         Return the move line for the statement line
         '''
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         Currency = Pool().get('currency.currency')
-        zero = Decimal("0.0")
         if not self.amount:
             return
-        with Transaction().set_context(date=self.date):
-            amount = Currency.compute(self.statement.journal.currency,
-                self.amount, self.statement.company.currency)
-        if self.statement.journal.currency != self.statement.company.currency:
-            second_currency = self.statement.journal.currency.id
+        if self.second_currency == self.company_currency:
+            amount = self.amount_second_currency
+        else:
+            with Transaction().set_context(date=self.date):
+                amount = Currency.compute(
+                    self.currency, self.amount, self.company_currency)
+        if self.currency != self.company_currency:
+            second_currency = self.currency
             amount_second_currency = -self.amount
+        elif self.second_currency:
+            second_currency = self.second_currency
+            amount_second_currency = -self.amount_second_currency
         else:
-            amount_second_currency = None
             second_currency = None
+            amount_second_currency = None
 
         return MoveLine(
             origin=self,
-            debit=amount < zero and -amount or zero,
-            credit=amount >= zero and amount or zero,
+            debit=abs(amount) if amount < 0 else 0,
+            credit=abs(amount) if amount > 0 else 0,
             account=self.account,
             party=self.party if self.account.party_required else None,
             second_currency=second_currency,
             amount_second_currency=amount_second_currency,
             )
 
 
@@ -1042,14 +1098,18 @@
             'Journal'), 'get_journal', searcher='search_journal')
     number = fields.Char('Number')
     date = fields.Date('Date')
     amount = Monetary(
         "Amount", currency='currency', digits='currency')
     currency = fields.Function(fields.Many2One('currency.currency',
             'Currency'), 'get_currency')
+    amount_second_currency = Monetary(
+        "Amount Second Currency",
+        currency='second_currency', digits='second_currency')
+    second_currency = fields.Many2One('currency.currency', "Second Currency")
     party = fields.Many2One('party.party', 'Party')
     move = fields.Many2One('account.move', 'Move')
 
     @classmethod
     def __setup__(cls):
         cls.number.search_unaccented = False
         super(LineGroup, cls).__setup__()
@@ -1059,14 +1119,15 @@
     @classmethod
     def _grouped_columns(cls, line):
         return [
             Max(line.statement).as_('statement'),
             Max(line.number).as_('number'),
             Max(line.date).as_('date'),
             Sum(line.amount).as_('amount'),
+            Sum(line.amount_second_currency).as_('amount_second_currency'),
             Max(line.party).as_('party'),
             ]
 
     @classmethod
     def table_query(cls):
         pool = Pool()
         Move = pool.get('account.move')
@@ -1076,14 +1137,15 @@
 
         std_columns = [
             move.id,
             move.create_uid,
             move.create_date,
             move.write_uid,
             move.write_date,
+            line.second_currency,
             ]
 
         columns = (std_columns + [move.id.as_('move')]
             + cls._grouped_columns(line))
         return move.join(line,
             condition=move.id == line.move
             ).select(*columns,
@@ -1170,14 +1232,26 @@
             .select(table.id,
                 having=Operator(
                     table.amount - Coalesce(Sum(line.amount), 0), value),
                 group_by=table.id))
         return [('id', 'in', query)]
 
     @classmethod
+    def delete(cls, origins):
+        for origin in origins:
+            if origin.statement_state not in {'cancelled', 'draft'}:
+                raise AccessError(
+                    gettext(
+                        'account_statement.'
+                        'msg_statement_origin_delete_cancel_draft',
+                        origin=origin.rec_name,
+                        sale=origin.statement.rec_name))
+        super().delete(origins)
+
+    @classmethod
     def copy(cls, origins, default=None):
         default = default.copy() if default is not None else {}
         default.setdefault('lines')
         return super().copy(origins, default=default)
 
 
 del _states
```

### Comparing `trytond_account_statement-7.0.2/statement.xml` & `trytond_account_statement-7.2.0/statement.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_account_statement-7.0.2/statement.xml` & `trytond_account_statement-7.2.0/statement.xml`

```diff
@@ -61,15 +61,15 @@
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_statement_form"/>
     </record>
     <menuitem parent="menu_statements" action="act_statement_form" sequence="10" id="menu_statement_form"/>
     <record model="ir.rule.group" id="rule_group_statement_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
+      <field name="model">account.statement</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_statement_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_statement_companies"/>
     </record>
     <record model="ir.action.report" id="report_statement">
@@ -117,81 +117,81 @@
     </record>
     <record model="ir.action.keyword" id="act_statement_line_move_line_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">account.move.line,-1</field>
       <field name="action" ref="act_statement_line_move_line"/>
     </record>
     <record model="ir.model.access" id="access_statement">
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
+      <field name="model">account.statement</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_statement_account_admin">
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
+      <field name="model">account.statement</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_statement_account">
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
+      <field name="model">account.statement</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_statement_statement">
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
+      <field name="model">account.statement</field>
       <field name="group" ref="group_statement"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="statement_draft_button">
+      <field name="model">account.statement</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
     </record>
     <record model="ir.model.button-res.group" id="statement_draft_button_group_account">
       <field name="button" ref="statement_draft_button"/>
       <field name="group" ref="account.group_account"/>
     </record>
     <record model="ir.model.button" id="statement_validate_button">
+      <field name="model">account.statement</field>
       <field name="name">validate_statement</field>
       <field name="string">Validate</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
     </record>
     <record model="ir.model.button" id="statement_post_button">
+      <field name="model">account.statement</field>
       <field name="name">post</field>
       <field name="string">Post</field>
       <field name="confirm">Are you sure you want to post the statement?</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
     </record>
     <record model="ir.model.button-res.group" id="statement_post_button_group_account">
       <field name="button" ref="statement_post_button"/>
       <field name="group" ref="account.group_account"/>
     </record>
     <record model="ir.model.button" id="statement_cancel_button">
+      <field name="model">account.statement</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
     </record>
     <record model="ir.model.button-res.group" id="statement_cancel_button_group_account">
       <field name="button" ref="statement_cancel_button"/>
       <field name="group" ref="account.group_account_admin"/>
     </record>
     <record model="ir.model.button" id="statement_reconcile_button">
+      <field name="model">account.statement</field>
       <field name="name">reconcile</field>
       <field name="string">Reconcile</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
     </record>
     <record model="ir.model.button-res.group" id="statement_reconcile_button_group_account">
       <field name="button" ref="statement_reconcile_button"/>
       <field name="group" ref="account.group_account"/>
     </record>
     <record model="ir.ui.view" id="line_group_view_form">
       <field name="model">account.statement.line.group</field>
@@ -246,15 +246,15 @@
     </record>
     <record model="ir.action.keyword" id="act_statement_origin_form_statement_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">account.statement,-1</field>
       <field name="action" ref="act_statement_origin_form_statement"/>
     </record>
     <record model="ir.model.access" id="access_statement_origin_information">
-      <field name="model" search="[('model', '=', 'account.statement.origin.information')]"/>
+      <field name="model">account.statement.origin.information</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="statement_import_start_view_form">
       <field name="model">account.statement.import.start</field>
```

### Comparing `trytond_account_statement-7.0.2/tests/scenario_account_statement.rst` & `trytond_account_statement-7.2.0/tests/scenario_account_statement.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ==========================
 Account Statement Scenario
 ==========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+
+    >>> from proteus import Model, Report
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_statement', 'account_invoice'])
 
@@ -138,30 +137,27 @@
     >>> statement_line = StatementLine()
     >>> statement.lines.append(statement_line)
     >>> statement_line.number = '0001'
     >>> statement_line.description = 'description'
     >>> statement_line.date = today
     >>> statement_line.amount = Decimal('180')
     >>> statement_line.party = customer
-    >>> statement_line.account == receivable
-    True
+    >>> assertEqual(statement_line.account, receivable)
     >>> statement_line.related_to = customer_invoice1
     >>> statement_line.amount
     Decimal('100.00')
     >>> statement_line = statement.lines[-1]
     >>> statement_line.amount
     Decimal('80.00')
     >>> statement_line.number
     '0001'
     >>> statement_line.description
     'description'
-    >>> statement_line.party == customer
-    True
-    >>> statement_line.account == receivable
-    True
+    >>> assertEqual(statement_line.party, customer)
+    >>> assertEqual(statement_line.account, receivable)
     >>> statement_line.description = 'other description'
     >>> statement_line.related_to = customer_invoice2
     >>> statement_line.amount
     Decimal('80.00')
 
 Paid 50 to customer::
 
@@ -178,16 +174,15 @@
 Paid 50 to supplier::
 
     >>> statement_line = StatementLine()
     >>> statement.lines.append(statement_line)
     >>> statement_line.date = today
     >>> statement_line.amount = Decimal('-60')
     >>> statement_line.party = supplier
-    >>> statement_line.account == payable
-    True
+    >>> assertEqual(statement_line.account, payable)
     >>> statement_line.related_to = supplier_invoice
     >>> statement_line.amount
     Decimal('-50.00')
     >>> statement_line = statement.lines[-1]
     >>> statement_line.amount
     Decimal('-10.00')
 
@@ -207,15 +202,15 @@
     >>> statement.click('validate_statement')
     >>> statement.state
     'validated'
 
 Try posting a move::
 
     >>> statement_line = statement.lines[0]
-    >>> statement_line.move.click('post')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> statement_line.move.click('post')
     Traceback (most recent call last):
         ...
     trytond.modules.account.exceptions.PostError: ...
 
 Cancel statement::
 
     >>> statement.click('cancel')
@@ -305,16 +300,15 @@
     >>> statement_line = StatementLine()
     >>> statement.lines.append(statement_line)
     >>> statement_line.date = today
     >>> statement_line.party = customer
     >>> statement_line.account = receivable
     >>> statement_line.amount = Decimal(-120)
     >>> statement_line.related_to = customer_invoice3
-    >>> statement_line.related_to.id == customer_invoice3.id
-    True
+    >>> assertEqual(statement_line.related_to, customer_invoice3)
 
     >>> statement_line = StatementLine()
     >>> statement.lines.append(statement_line)
     >>> statement_line.date = today
     >>> statement_line.party = supplier
     >>> statement_line.account = payable
     >>> statement_line.amount = Decimal(50)
@@ -356,15 +350,15 @@
     >>> statement_line.date = today
     >>> statement_line.party = customer
     >>> statement_line.account = receivable
     >>> statement_line.amount = Decimal(300)
     >>> statement_line.related_to = customer_invoice4
     >>> statement2.save()
 
-    >>> statement1.click('validate_statement') # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> statement1.click('validate_statement')
     Traceback (most recent call last):
         ...
     StatementValidateWarning: ...
     >>> statement2.reload()
     >>> Model.get('res.user.warning')(user=config.user,
     ...     name=str(statement2.lines[0].id), always=True).save()
     >>> statement1.click('validate_statement')
@@ -392,15 +386,15 @@
     >>> statement.start_balance = Decimal('50.00')
     >>> statement.end_balance = Decimal('150.00')
     >>> line = statement.lines.new()
     >>> line.date = today
     >>> line.amount = Decimal('60.00')
     >>> line.account = receivable
     >>> line.party = customer
-    >>> statement.click('validate_statement')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> statement.click('validate_statement')
     Traceback (most recent call last):
         ...
     StatementValidateError: ...
 
     >>> second_line = statement.lines.new()
     >>> second_line.date = today
     >>> second_line.amount = Decimal('40.00')
@@ -421,15 +415,15 @@
     >>> statement.journal = journal_amount
     >>> statement.total_amount = Decimal('80.00')
     >>> line = statement.lines.new()
     >>> line.date = today
     >>> line.amount = Decimal('50.00')
     >>> line.account = receivable
     >>> line.party = customer
-    >>> statement.click('validate_statement')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> statement.click('validate_statement')
     Traceback (most recent call last):
         ...
     StatementValidateError: ...
 
     >>> second_line = statement.lines.new()
     >>> second_line.date = today
     >>> second_line.amount = Decimal('30.00')
@@ -450,15 +444,15 @@
     >>> statement.journal = journal_number
     >>> statement.number_of_lines = 2
     >>> line = statement.lines.new()
     >>> line.date = today
     >>> line.amount = Decimal('50.00')
     >>> line.account = receivable
     >>> line.party = customer
-    >>> statement.click('validate_statement')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> statement.click('validate_statement')
     Traceback (most recent call last):
         ...
     StatementValidateError: ...
 
     >>> second_line = statement.lines.new()
     >>> second_line.date = today
     >>> second_line.amount = Decimal('10.00')
```

### Comparing `trytond_account_statement-7.0.2/tests/scenario_statement_origin.rst` & `trytond_account_statement-7.2.0/tests/scenario_statement_origin.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Account Statement Origin Scenario
 =================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+
+    >>> from proteus import Model, Report
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement')
 
@@ -66,29 +66,26 @@
     >>> origin.date = today
     >>> origin.amount = Decimal('50.00')
     >>> origin.party = customer
     >>> statement.click('validate_statement')
 
 Statement can not be posted until all origins are finished::
 
-    >>> statement.click('post')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> statement.click('post')
     Traceback (most recent call last):
         ...
     StatementPostError: ...
     >>> statement.click('draft')
     >>> origin, = statement.origins
     >>> line = origin.lines.new()
-    >>> line.date == today
-    True
+    >>> assertEqual(line.date, today)
     >>> line.amount
     Decimal('50.00')
-    >>> line.party == customer
-    True
-    >>> line.account == receivable
-    True
+    >>> assertEqual(line.party, customer)
+    >>> assertEqual(line.account, receivable)
     >>> line.amount = Decimal('52.00')
     >>> line = origin.lines.new()
     >>> line.amount
     Decimal('-2.00')
     >>> line.account = expense
     >>> line.description = "Bank Fees"
     >>> statement.click('post')
```

### Comparing `trytond_account_statement-7.0.2/tests/scenario_statement_origin_invoices.rst` & `trytond_account_statement-7.2.0/tests/scenario_statement_origin_invoices.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Account Statement Origin Invoices Scenario
 ==========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement')
 
@@ -95,21 +95,17 @@
 Pending amount is used to fill all invoices::
 
     >>> origin, = statement.origins
     >>> line = origin.lines.new()
     >>> line.related_to = customer_invoice1
     >>> line.amount
     Decimal('100.00')
-    >>> line.party == customer
-    True
-    >>> line.account == receivable
-    True
+    >>> assertEqual(line.party, customer)
+    >>> assertEqual(line.account, receivable)
     >>> origin.pending_amount
     Decimal('80.00')
     >>> line = origin.lines.new()
     >>> line.related_to = customer_invoice2
     >>> line.amount
     Decimal('80.00')
-    >>> line.party == customer
-    True
-    >>> line.account == receivable
-    True
+    >>> assertEqual(line.party, customer)
+    >>> assertEqual(line.account, receivable)
```

### Comparing `trytond_account_statement-7.0.2/tox.ini` & `trytond_account_statement-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.0.2/trytond_account_statement.egg-info/SOURCES.txt` & `trytond_account_statement-7.2.0/trytond_account_statement.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 account.py
 account.xml
+bank.py
 exceptions.py
 journal.py
 journal.xml
 message.xml
 party.py
 setup.py
 statement.fodt
 statement.py
 statement.xml
 tox.ini
 tryton.cfg
 ./__init__.py
 ./account.py
 ./account.xml
+./bank.py
 ./exceptions.py
 ./journal.py
 ./journal.xml
 ./message.xml
 ./party.py
 ./statement.fodt
 ./statement.py
@@ -52,14 +53,16 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_account_statement.rst
+./tests/scenario_account_statement_bank_account.rst
+./tests/scenario_account_statement_second_currency_invoice.rst
 ./tests/scenario_statement_origin.rst
 ./tests/scenario_statement_origin_invoices.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/line_group_form.xml
 ./view/line_group_list.xml
 ./view/statement_form.xml
@@ -69,15 +72,18 @@
 ./view/statement_line_form.xml
 ./view/statement_line_tree.xml
 ./view/statement_line_tree_editable.xml
 ./view/statement_origin_form.xml
 ./view/statement_origin_tree.xml
 ./view/statement_tree.xml
 doc/conf.py
+doc/configuration.rst
+doc/design.rst
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -97,14 +103,16 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_account_statement.rst
+tests/scenario_account_statement_bank_account.rst
+tests/scenario_account_statement_second_currency_invoice.rst
 tests/scenario_statement_origin.rst
 tests/scenario_statement_origin_invoices.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_account_statement.egg-info/PKG-INFO
 trytond_account_statement.egg-info/SOURCES.txt
 trytond_account_statement.egg-info/dependency_links.txt
```

### Comparing `trytond_account_statement-7.0.2/view/line_group_form.xml` & `trytond_account_statement-7.2.0/view/line_group_form.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_account_statement-7.0.2/view/line_group_form.xml` & `trytond_account_statement-7.2.0/view/line_group_form.xml`

```diff
@@ -8,13 +8,14 @@
   <field name="journal" widget="selection"/>
   <label name="number"/>
   <field name="number"/>
   <label name="date"/>
   <field name="date"/>
   <label name="amount"/>
   <field name="amount"/>
-  <newline/>
+  <label name="amount_second_currency"/>
+  <field name="amount_second_currency"/>
   <label name="party"/>
   <field name="party"/>
   <label name="move"/>
   <field name="move"/>
 </form>
```

### Comparing `trytond_account_statement-7.0.2/view/statement_form.xml` & `trytond_account_statement-7.2.0/view/statement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.0.2/view/statement_journal_form.xml` & `trytond_account_statement-7.2.0/view/statement_journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.0.2/view/statement_origin_form.xml` & `trytond_account_statement-7.2.0/view/statement_line_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account_statement-7.0.2/view/statement_origin_form.xml` & `trytond_account_statement-7.2.0/view/statement_line_form.xml`

```diff
@@ -1,25 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
   <label name="statement"/>
-  <field name="statement"/>
-  <label name="company"/>
-  <field name="company"/>
+  <field name="statement" colspan="3"/>
   <label name="number"/>
   <field name="number"/>
+  <label name="sequence"/>
+  <field name="sequence"/>
   <label name="date"/>
   <field name="date"/>
   <label name="amount"/>
   <field name="amount"/>
-  <label name="pending_amount"/>
-  <field name="pending_amount"/>
+  <label name="amount_second_currency"/>
+  <field name="amount_second_currency"/>
+  <label name="second_currency"/>
+  <field name="second_currency"/>
   <label name="party"/>
   <field name="party"/>
   <label name="account"/>
   <field name="account"/>
+  <label name="related_to"/>
+  <field name="related_to"/>
+  <newline/>
   <label name="description"/>
   <field name="description" colspan="3"/>
-  <field name="information" colspan="4"/>
-  <field name="lines" colspan="4"/>
+  <label name="move"/>
+  <field name="move"/>
+  <label name="origin"/>
+  <field name="origin"/>
 </form>
```

