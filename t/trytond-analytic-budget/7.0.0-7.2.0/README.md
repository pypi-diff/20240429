# Comparing `tmp/trytond_analytic_budget-7.0.0.tar.gz` & `tmp/trytond_analytic_budget-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_budget-7.0.0.tar", last modified: Mon Oct 30 17:26:35 2023, max compression
+gzip compressed data, was "trytond_analytic_budget-7.2.0.tar", last modified: Mon Apr 29 15:37:45 2024, max compression
```

## Comparing `trytond_analytic_budget-7.0.0.tar` & `trytond_analytic_budget-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:35.104502 trytond_analytic_budget-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:22:58.000000 trytond_analytic_budget-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      627 2023-10-30 17:04:32.000000 trytond_analytic_budget-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-10-30 17:04:31.000000 trytond_analytic_budget-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2924 2023-10-30 17:26:35.104502 trytond_analytic_budget-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7903 2023-08-13 15:26:13.000000 trytond_analytic_budget-7.0.0/analytic_account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8543 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/analytic_account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:35.101168 trytond_analytic_budget-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:22:58.000000 trytond_analytic_budget-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1336 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:58.000000 trytond_analytic_budget-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      948 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:35.097835 trytond_analytic_budget-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6125 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5869 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4916 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5876 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4975 2023-10-30 16:47:45.000000 trytond_analytic_budget-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-10-28 12:11:21.000000 trytond_analytic_budget-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:26:35.104502 trytond_analytic_budget-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4687 2023-10-27 17:38:49.000000 trytond_analytic_budget-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:35.097835 trytond_analytic_budget-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4424 2023-08-13 15:26:13.000000 trytond_analytic_budget-7.0.0/tests/scenario_analytic_budget.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_analytic_budget-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2023-10-30 17:04:27.000000 trytond_analytic_budget-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:35.104502 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2924 2023-10-30 17:26:34.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2060 2023-10-30 17:26:35.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:26:34.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:26:34.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      138 2023-10-30 17:26:34.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:26:34.000000 trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:35.101168 trytond_analytic_budget-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_copy_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      639 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_line_form_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_line_tree_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.0.0/view/budget_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.416968 trytond_analytic_budget-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:17:39.000000 trytond_analytic_budget-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-29 15:17:39.000000 trytond_analytic_budget-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2915 2024-04-29 15:37:45.416968 trytond_analytic_budget-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7903 2024-01-27 09:58:52.000000 trytond_analytic_budget-7.2.0/analytic_account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8405 2024-04-27 16:30:39.000000 trytond_analytic_budget-7.2.0/analytic_account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.410302 trytond_analytic_budget-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_analytic_budget-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1336 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:03.000000 trytond_analytic_budget-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      948 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5895 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6125 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5869 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4916 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5876 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5023 2024-04-29 13:17:17.000000 trytond_analytic_budget-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4975 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:45.416968 trytond_analytic_budget-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4678 2024-04-27 16:30:39.000000 trytond_analytic_budget-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4419 2024-04-22 12:14:36.000000 trytond_analytic_budget-7.2.0/tests/scenario_analytic_budget.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:03.000000 trytond_analytic_budget-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2024-04-29 15:17:35.000000 trytond_analytic_budget-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2915 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2042 2024-04-29 15:37:45.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      138 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_copy_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      639 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_form_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_tree_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_list.xml
```

### Comparing `trytond_analytic_budget-7.0.0/COPYRIGHT` & `trytond_analytic_budget-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2023 B2CK
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 B2CK
+Copyright (C) 2021-2024 Cédric Krier
 Copyright (C) 2020-2021 David Harper
 Copyright (C) 2019 Adrián Bernardi
 Copyright (C) 2016 Sergi Almacellas Abellana
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `trytond_analytic_budget-7.0.0/LICENSE` & `trytond_analytic_budget-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/PKG-INFO` & `trytond_analytic_budget-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_budget
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that allows creating budgets for analytic accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-analytic-budget
+Project-URL: Documentation, https://docs.tryton.org/modules-analytic-budget
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account budget
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_budget<7.1,>=7.0
-Requires-Dist: trytond_analytic_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_budget<7.3,>=7.2
+Requires-Dist: trytond_analytic_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ######################
 Analytic Budget Module
 ######################
 
 The *Analytic Budget Module* provides the ability to set budgets for analytic
 accounts over a defined period of time.
```

### Comparing `trytond_analytic_budget-7.0.0/__init__.py` & `trytond_analytic_budget-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/analytic_account.py` & `trytond_analytic_budget-7.2.0/analytic_account.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/analytic_account.xml` & `trytond_analytic_budget-7.2.0/analytic_account.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_analytic_budget-7.0.0/analytic_account.xml` & `trytond_analytic_budget-7.2.0/analytic_account.xml`

```diff
@@ -30,49 +30,49 @@
     <record model="ir.action.act_window.view" id="act_budget_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="budget_view_form"/>
       <field name="act_window" ref="act_budget_form"/>
     </record>
     <menuitem parent="account_budget.menu_budget" action="act_budget_form" sequence="10" id="menu_budget_form"/>
     <record model="ir.model.button" id="budget_update_lines_button">
+      <field name="model">analytic_account.budget</field>
       <field name="name">update_lines</field>
       <field name="string">Update Lines</field>
-      <field name="model" search="[('model', '=', 'analytic_account.budget')]"/>
     </record>
     <record model="ir.model.button" id="budget_copy_button">
+      <field name="model">analytic_account.budget</field>
       <field name="name">copy_button</field>
       <field name="string">Copy</field>
-      <field name="model" search="[('model', '=', 'analytic_account.budget')]"/>
     </record>
     <record model="ir.model.access" id="access_budget">
-      <field name="model" search="[('model', '=', 'analytic_account.budget')]"/>
+      <field name="model">analytic_account.budget</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_budget_account">
-      <field name="model" search="[('model', '=', 'analytic_account.budget')]"/>
+      <field name="model">analytic_account.budget</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_budget_budget">
-      <field name="model" search="[('model', '=', 'analytic_account.budget')]"/>
+      <field name="model">analytic_account.budget</field>
       <field name="group" ref="account_budget.group_budget"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_budget_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'analytic_account.budget')]"/>
+      <field name="model">analytic_account.budget</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_budget_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_budget_companies"/>
     </record>
     <record model="ir.ui.view" id="budget_line_view_form">
```

### Comparing `trytond_analytic_budget-7.0.0/doc/conf.py` & `trytond_analytic_budget-7.2.0/doc/conf.py`

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

### Comparing `trytond_analytic_budget-7.0.0/doc/design.rst` & `trytond_analytic_budget-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/doc/usage.rst` & `trytond_analytic_budget-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/bg.po` & `trytond_analytic_budget-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/ca.po` & `trytond_analytic_budget-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/cs.po` & `trytond_analytic_budget-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/de.po` & `trytond_analytic_budget-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/es.po` & `trytond_analytic_budget-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/es_419.po` & `trytond_analytic_budget-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/et.po` & `trytond_analytic_budget-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/fa.po` & `trytond_analytic_budget-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/fi.po` & `trytond_analytic_budget-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/fr.po` & `trytond_analytic_budget-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/hu.po` & `trytond_analytic_budget-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/id.po` & `trytond_analytic_budget-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/it.po` & `trytond_analytic_budget-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/lo.po` & `trytond_analytic_budget-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/lt.po` & `trytond_analytic_budget-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/nl.po` & `trytond_analytic_budget-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/pl.po` & `trytond_analytic_budget-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/pt.po` & `trytond_analytic_budget-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/ro.po` & `trytond_analytic_budget-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/ru.po` & `trytond_analytic_budget-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/sl.po` & `trytond_analytic_budget-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/tr.po` & `trytond_analytic_budget-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/uk.po` & `trytond_analytic_budget-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/locale/zh_CN.po` & `trytond_analytic_budget-7.2.0/locale/ro.po`

 * *Files 13% similar despite different names*

```diff
@@ -162,37 +162,41 @@
 msgid "Analytic Budget"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_budget_form"
 msgid "Analytic Budgets"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_budget_line_form"
 msgid "Budget Lines"
-msgstr ""
+msgstr "Randuri de Buget"
 
 msgctxt "model:ir.action,name:act_budget_report"
 msgid "Analytic Budgets"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_budget_copy"
 msgid "Copy Budget"
-msgstr ""
+msgstr "Copiere Buget"
 
 msgctxt "model:ir.model.button,string:budget_copy_button"
 msgid "Copy"
-msgstr ""
+msgstr "Copiere"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:budget_update_lines_button"
 msgid "Update Lines"
-msgstr ""
+msgstr "Actualizare Randuri"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_budget_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator in companii"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_form"
 msgid "Analytic Budgets"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_budget_report"
 msgid "Analytic Budgets"
```

### Comparing `trytond_analytic_budget-7.0.0/setup.py` & `trytond_analytic_budget-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
-        'https://docs.tryton.org/projects/modules-analytic-budget',
+        'https://docs.tryton.org/modules-analytic-budget',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton analytic account budget',
     package_dir={'trytond.modules.analytic_budget': '.'},
     packages=(
         ['trytond.modules.analytic_budget']
```

### Comparing `trytond_analytic_budget-7.0.0/tests/scenario_analytic_budget.rst` & `trytond_analytic_budget-7.2.0/tests/scenario_analytic_budget.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ========================
 Analytic Budget Scenario
 ========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate the analytic_budget module::
 
     >>> config = activate_modules('analytic_budget')
 
     >>> AnalyticAccount = Model.get('analytic_account.account')
     >>> Budget = Model.get('analytic_account.budget')
@@ -125,18 +125,16 @@
 
     >>> copy_budget = budget.click('copy_button')
     >>> copy_budget.form.start_date = next_period.start_date
     >>> copy_budget.form.end_date = next_period.end_date
     >>> copy_budget.form.factor = Decimal('1.2')
     >>> copy_budget.execute('copy')
     >>> new_budget, = copy_budget.actions[0]
-    >>> new_budget.start_date == next_period.start_date
-    True
-    >>> new_budget.end_date == next_period.end_date
-    True
+    >>> assertEqual(new_budget.start_date, next_period.start_date)
+    >>> assertEqual(new_budget.end_date, next_period.end_date)
     >>> analytic_budget, other_analytic_budget = new_budget.lines
     >>> analytic_budget.total_amount
     Decimal('-84.00')
     >>> analytic_budget.actual_amount
     Decimal('0.00')
     >>> analytic_budget.percentage
     Decimal('0.0000')
```

### Comparing `trytond_analytic_budget-7.0.0/tox.ini` & `trytond_analytic_budget-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/PKG-INFO` & `trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-analytic-budget
-Version: 7.0.0
+Name: trytond_analytic_budget
+Version: 7.2.0
 Summary: Tryton module that allows creating budgets for analytic accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-analytic-budget
+Project-URL: Documentation, https://docs.tryton.org/modules-analytic-budget
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account budget
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_budget<7.1,>=7.0
-Requires-Dist: trytond_analytic_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_budget<7.3,>=7.2
+Requires-Dist: trytond_analytic_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ######################
 Analytic Budget Module
 ######################
 
 The *Analytic Budget Module* provides the ability to set budgets for analytic
 accounts over a defined period of time.
```

### Comparing `trytond_analytic_budget-7.0.0/trytond_analytic_budget.egg-info/SOURCES.txt` & `trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/SOURCES.txt`

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
 analytic_account.py
```

### Comparing `trytond_analytic_budget-7.0.0/view/budget_copy_start_form.xml` & `trytond_analytic_budget-7.2.0/view/budget_copy_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/view/budget_form.xml` & `trytond_analytic_budget-7.2.0/view/budget_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/view/budget_line_form.xml` & `trytond_analytic_budget-7.2.0/view/budget_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.0.0/view/budget_line_form_amount.xml` & `trytond_analytic_budget-7.2.0/view/budget_line_form_amount.xml`

 * *Files identical despite different names*

