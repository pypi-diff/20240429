# Comparing `tmp/trytond_account_budget-7.0.0.tar.gz` & `tmp/trytond_account_budget-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_budget-7.0.0.tar", last modified: Mon Oct 30 17:18:29 2023, max compression
+gzip compressed data, was "trytond_account_budget-7.2.0.tar", last modified: Mon Apr 29 15:31:53 2024, max compression
```

## Comparing `trytond_account_budget-7.0.0.tar` & `trytond_account_budget-7.2.0.tar`

### file list

```diff
@@ -1,77 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:29.658853 trytond_account_budget-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:22:48.000000 trytond_account_budget-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      627 2023-10-30 17:00:54.000000 trytond_account_budget-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-10-30 17:00:54.000000 trytond_account_budget-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2879 2023-10-30 17:18:29.658853 trytond_account_budget-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30061 2023-10-24 07:56:52.000000 trytond_account_budget-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10646 2023-06-23 12:44:24.000000 trytond_account_budget-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:29.655520 trytond_account_budget-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:22:48.000000 trytond_account_budget-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1610 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:48.000000 trytond_account_budget-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:29.652186 trytond_account_budget-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10307 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10644 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10348 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10248 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8370 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8278 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10356 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9016 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2023-10-30 16:47:45.000000 trytond_account_budget-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1012 2023-10-24 07:56:52.000000 trytond_account_budget-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:18:29.658853 trytond_account_budget-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4653 2023-10-27 17:38:49.000000 trytond_account_budget-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:29.652186 trytond_account_budget-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6047 2023-08-13 15:26:13.000000 trytond_account_budget-7.0.0/tests/scenario_account_budget.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_budget-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-10-30 17:00:51.000000 trytond_account_budget-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:29.658853 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2879 2023-10-30 17:18:29.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2391 2023-10-30 17:18:29.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:18:29.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:18:29.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-10-30 17:18:29.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:18:29.000000 trytond_account_budget-7.0.0/trytond_account_budget.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:29.655520 trytond_account_budget-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_copy_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_form_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      563 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-08-21 07:34:17.000000 trytond_account_budget-7.0.0/view/budget_line_period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-08-21 07:34:17.000000 trytond_account_budget-7.0.0/view/budget_line_period_list_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_line_tree_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:14.000000 trytond_account_budget-7.0.0/view/budget_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:12:52.000000 trytond_account_budget-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-29 15:12:52.000000 trytond_account_budget-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2870 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30061 2024-02-04 18:51:26.000000 trytond_account_budget-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10485 2024-04-27 16:30:39.000000 trytond_account_budget-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.459506 trytond_account_budget-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_account_budget-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account_budget-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10307 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10644 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10348 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10248 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8370 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8278 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10356 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9670 2024-04-29 13:17:17.000000 trytond_account_budget-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9016 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1012 2024-02-04 18:51:26.000000 trytond_account_budget-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4644 2024-04-27 16:30:39.000000 trytond_account_budget-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5938 2024-04-22 12:14:36.000000 trytond_account_budget-7.2.0/tests/scenario_account_budget.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account_budget-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-04-29 15:12:48.000000 trytond_account_budget-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2870 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2373 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_copy_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_form_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      563 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-01-27 09:58:52.000000 trytond_account_budget-7.2.0/view/budget_line_period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-01-27 09:58:52.000000 trytond_account_budget-7.2.0/view/budget_line_period_list_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_tree_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_list.xml
```

### Comparing `trytond_account_budget-7.0.0/COPYRIGHT` & `trytond_account_budget-7.2.0/COPYRIGHT`

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

### Comparing `trytond_account_budget-7.0.0/LICENSE` & `trytond_account_budget-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/PKG-INFO` & `trytond_account_budget-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_budget
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that allows budgets to be setup for accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-budget
+Project-URL: Documentation, https://docs.tryton.org/modules-account-budget
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account budget
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
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #####################
 Account Budget Module
 #####################
 
 The *Account Budget Module* provides the ability to set budgets for accounts
 over a defined period of time.
```

### Comparing `trytond_account_budget-7.0.0/__init__.py` & `trytond_account_budget-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/account.py` & `trytond_account_budget-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/account.xml` & `trytond_account_budget-7.2.0/account.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account_budget-7.0.0/account.xml` & `trytond_account_budget-7.2.0/account.xml`

```diff
@@ -42,49 +42,49 @@
     <record model="ir.action.act_window.view" id="act_budget_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="budget_view_form"/>
       <field name="act_window" ref="act_budget_form"/>
     </record>
     <menuitem parent="menu_budget" action="act_budget_form" sequence="10" id="menu_budget_form"/>
     <record model="ir.model.button" id="budget_update_lines_button">
+      <field name="model">account.budget</field>
       <field name="name">update_lines</field>
       <field name="string">Update Lines</field>
-      <field name="model" search="[('model', '=', 'account.budget')]"/>
     </record>
     <record model="ir.model.button" id="budget_copy_button">
+      <field name="model">account.budget</field>
       <field name="name">copy_button</field>
       <field name="string">Copy</field>
-      <field name="model" search="[('model', '=', 'account.budget')]"/>
     </record>
     <record model="ir.model.access" id="access_budget">
-      <field name="model" search="[('model', '=', 'account.budget')]"/>
+      <field name="model">account.budget</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_budget_account">
-      <field name="model" search="[('model', '=', 'account.budget')]"/>
+      <field name="model">account.budget</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_budget_budget">
-      <field name="model" search="[('model', '=', 'account.budget')]"/>
+      <field name="model">account.budget</field>
       <field name="group" ref="group_budget"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_budget_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.budget')]"/>
+      <field name="model">account.budget</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_budget_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_budget_companies"/>
     </record>
     <record model="ir.ui.view" id="budget_line_view_form">
@@ -152,17 +152,17 @@
     <record model="ir.action.act_window.view" id="act_budget_report_view2">
       <field name="view" ref="budget_line_view_form_amount"/>
       <field name="sequence" eval="20"/>
       <field name="act_window" ref="act_budget_report"/>
     </record>
     <menuitem parent="account.menu_reporting" action="act_budget_report" sequence="30" id="menu_budget_report"/>
     <record model="ir.model.button" id="budget_line_create_periods_button">
+      <field name="model">account.budget.line</field>
       <field name="name">create_periods</field>
       <field name="string">Create Periods</field>
-      <field name="model" search="[('model', '=', 'account.budget.line')]"/>
     </record>
     <record model="ir.ui.view" id="budget_line_period_view_form">
       <field name="model">account.budget.line.period</field>
       <field name="type">form</field>
       <field name="name">budget_line_period_form</field>
     </record>
     <record model="ir.ui.view" id="budget_line_period_view_list">
```

### Comparing `trytond_account_budget-7.0.0/doc/conf.py` & `trytond_account_budget-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_budget-7.0.0/doc/design.rst` & `trytond_account_budget-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/doc/reference.rst` & `trytond_account_budget-7.2.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/doc/usage.rst` & `trytond_account_budget-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/bg.po` & `trytond_account_budget-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/ca.po` & `trytond_account_budget-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/cs.po` & `trytond_account_budget-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/de.po` & `trytond_account_budget-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/es.po` & `trytond_account_budget-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/es_419.po` & `trytond_account_budget-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/et.po` & `trytond_account_budget-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/fa.po` & `trytond_account_budget-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/fi.po` & `trytond_account_budget-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/fr.po` & `trytond_account_budget-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/hu.po` & `trytond_account_budget-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/id.po` & `trytond_account_budget-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/it.po` & `trytond_account_budget-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/lo.po` & `trytond_account_budget-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/lt.po` & `trytond_account_budget-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/nl.po` & `trytond_account_budget-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/pl.po` & `trytond_account_budget-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/pt.po` & `trytond_account_budget-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/ro.po` & `trytond_account_budget-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/ru.po` & `trytond_account_budget-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/sl.po` & `trytond_account_budget-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/tr.po` & `trytond_account_budget-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/locale/uk.po` & `trytond_account_budget-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/message.xml` & `trytond_account_budget-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/setup.py` & `trytond_account_budget-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
-        'https://docs.tryton.org/projects/modules-account-budget',
+        'https://docs.tryton.org/modules-account-budget',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account budget',
     package_dir={'trytond.modules.account_budget': '.'},
     packages=(
         ['trytond.modules.account_budget']
```

### Comparing `trytond_account_budget-7.0.0/tests/scenario_account_budget.rst` & `trytond_account_budget-7.2.0/tests/scenario_account_budget.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 =======================
 Account Budget Scenario
 =======================
 
 Imports::
 
-    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_budget')
 
     >>> Account = Model.get('account.account')
     >>> Budget = Model.get('account.budget')
@@ -132,24 +130,24 @@
 Create periods::
 
     >>> create_periods = pl_budget.click('create_periods')
     >>> create_periods.execute('create_periods')
     >>> revenue_budget, expense_budget = pl_budget.children
     >>> len(pl_budget.periods)
     12
-    >>> all(p.total_amount == Decimal('-8.33') for p in pl_budget.periods)
-    True
+    >>> {p.total_amount for p in pl_budget.periods}
+    {Decimal('-8.33')}
     >>> len(revenue_budget.periods)
     12
-    >>> all(p.total_amount == Decimal('-12.50') for p in revenue_budget.periods)
-    True
+    >>> {p.total_amount for p in revenue_budget.periods}
+    {Decimal('-12.50')}
     >>> len(expense_budget.periods)
     12
-    >>> all(p.total_amount == Decimal('4.16') for p in expense_budget.periods)
-    True
+    >>> {p.total_amount for p in expense_budget.periods}
+    {Decimal('4.16')}
 
 Check the budget's periods::
 
     >>> pl_budget.periods[0].actual_amount
     Decimal('-70.00')
     >>> pl_budget.periods[0].percentage
     Decimal('8.4034')
@@ -174,15 +172,15 @@
     >>> expense_budget.periods[1].percentage
     Decimal('0.0000')
 
 Try to set invalid ratio::
 
     >>> period = pl_budget.periods[0]
     >>> period.ratio = Decimal('0.1')
-    >>> budget.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> budget.save()
     Traceback (most recent call last):
         ...
     BudgetValidationError: ...
     >>> budget.reload()
 
 Copy the budget without amounts::
```

### Comparing `trytond_account_budget-7.0.0/tox.ini` & `trytond_account_budget-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/trytond_account_budget.egg-info/PKG-INFO` & `trytond_account_budget-7.2.0/trytond_account_budget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-budget
-Version: 7.0.0
+Name: trytond_account_budget
+Version: 7.2.0
 Summary: Tryton module that allows budgets to be setup for accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-budget
+Project-URL: Documentation, https://docs.tryton.org/modules-account-budget
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account budget
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
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #####################
 Account Budget Module
 #####################
 
 The *Account Budget Module* provides the ability to set budgets for accounts
 over a defined period of time.
```

### Comparing `trytond_account_budget-7.0.0/trytond_account_budget.egg-info/SOURCES.txt` & `trytond_account_budget-7.2.0/trytond_account_budget.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_budget-7.0.0/view/budget_form.xml` & `trytond_account_budget-7.2.0/view/budget_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/view/budget_line_form.xml` & `trytond_account_budget-7.2.0/view/budget_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/view/budget_line_form_amount.xml` & `trytond_account_budget-7.2.0/view/budget_line_form_amount.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.0.0/view/budget_line_period_form.xml` & `trytond_account_budget-7.2.0/view/budget_line_period_form.xml`

 * *Files identical despite different names*

