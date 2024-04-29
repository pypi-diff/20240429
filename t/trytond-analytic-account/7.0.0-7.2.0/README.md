# Comparing `tmp/trytond_analytic_account-7.0.0.tar.gz` & `tmp/trytond_analytic_account-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_account-7.0.0.tar", last modified: Mon Oct 30 17:26:25 2023, max compression
+gzip compressed data, was "trytond_analytic_account-7.2.0.tar", last modified: Mon Apr 29 15:37:38 2024, max compression
```

## Comparing `trytond_analytic_account-7.0.0.tar` & `trytond_analytic_account-7.2.0.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:25.894458 trytond_analytic_account-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:22:58.000000 trytond_analytic_account-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3495 2023-10-30 17:04:27.000000 trytond_analytic_account-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-10-30 17:04:26.000000 trytond_analytic_account-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_account-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-30 17:26:25.894458 trytond_analytic_account-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17400 2023-10-24 07:57:53.000000 trytond_analytic_account-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9177 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/analytic_account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:25.891125 trytond_analytic_account-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:22:58.000000 trytond_analytic_account-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:58.000000 trytond_analytic_account-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10602 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5544 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/line.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:25.887791 trytond_analytic_account-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8643 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8477 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7714 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8643 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8509 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7431 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8091 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8877 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7701 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8633 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8094 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7729 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8383 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8942 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7877 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8675 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7919 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8267 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7499 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8610 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8493 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7692 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7334 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7932 2023-10-30 16:47:45.000000 trytond_analytic_account-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-07 15:40:36.000000 trytond_analytic_account-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:26:25.894458 trytond_analytic_account-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2023-10-27 17:38:49.000000 trytond_analytic_account-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:25.887791 trytond_analytic_account-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7707 2023-10-24 07:57:53.000000 trytond_analytic_account-7.0.0/tests/scenario_analytic_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11115 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_analytic_account-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-10-30 17:04:22.000000 trytond_analytic_account-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:25.894458 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-30 17:26:25.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2501 2023-10-30 17:26:25.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:26:25.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:26:25.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:26:25.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:26:25.000000 trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:25.891125 trytond_analytic_account-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_analytic_account-7.0.0/view/account_distribution_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_distribution_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-01-16 14:00:20.000000 trytond_analytic_account-7.0.0/view/analytic_account_entry_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/analytic_account_entry_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_analytic_account-7.0.0/view/line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_analytic_account-7.0.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-24 08:23:41.000000 trytond_analytic_account-7.0.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-10-07 15:40:36.000000 trytond_analytic_account-7.0.0/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_analytic_account-7.0.0/view/rule_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.037161 trytond_analytic_account-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3596 2024-04-29 15:17:34.000000 trytond_analytic_account-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:17:34.000000 trytond_analytic_account-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17400 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8975 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/analytic_account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.030495 trytond_analytic_account-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:03.000000 trytond_analytic_account-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10602 2024-03-17 11:01:36.000000 trytond_analytic_account-7.2.0/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5436 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/line.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.030495 trytond_analytic_account-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8643 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8477 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7714 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8643 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8509 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7431 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8091 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8877 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7701 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8633 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8094 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7729 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8383 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8942 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7877 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8675 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7919 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8267 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8576 2024-04-29 13:17:17.000000 trytond_analytic_account-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8610 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8493 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7692 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7334 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7932 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:38.037161 trytond_analytic_account-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2024-03-17 11:01:36.000000 trytond_analytic_account-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7642 2024-04-22 12:14:36.000000 trytond_analytic_account-7.2.0/tests/scenario_analytic_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11115 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:03.000000 trytond_analytic_account-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-29 15:17:30.000000 trytond_analytic_account-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2483 2024-04-29 15:37:38.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/account_distribution_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_distribution_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/analytic_account_entry_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/analytic_account_entry_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/rule_list.xml
```

### Comparing `trytond_analytic_account-7.0.0/CHANGELOG` & `trytond_analytic_account-7.2.0/CHANGELOG`

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

### Comparing `trytond_analytic_account-7.0.0/COPYRIGHT` & `trytond_analytic_account-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 Copyright (C) 2004-2008 Tiny SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_analytic_account-7.0.0/LICENSE` & `trytond_analytic_account-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/PKG-INFO` & `trytond_analytic_account-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_account
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for analytic accounting
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
@@ -49,21 +49,21 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Analytic Account Module
 #######################
 
 The analytic account module adds the fundamentals required to analyse
 accounting using multiple different axes.
```

### Comparing `trytond_analytic_account-7.0.0/README.rst` & `trytond_analytic_account-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/__init__.py` & `trytond_analytic_account-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/account.py` & `trytond_analytic_account-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/account.xml` & `trytond_analytic_account-7.2.0/account.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_analytic_account-7.0.0/account.xml` & `trytond_analytic_account-7.2.0/account.xml`

```diff
@@ -81,30 +81,30 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_view_form"/>
       <field name="act_window" ref="act_account_tree_chart"/>
     </record>
     <menuitem parent="account.menu_reporting" action="act_account_tree_chart" sequence="30" id="menu_account_tree_chart"/>
     <record model="ir.rule.group" id="rule_group_account_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'analytic_account.account')]"/>
+      <field name="model">analytic_account.account</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_account_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_account_companies"/>
     </record>
     <record model="ir.model.access" id="access_account">
-      <field name="model" search="[('model', '=', 'analytic_account.account')]"/>
+      <field name="model">analytic_account.account</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_account_admin">
-      <field name="model" search="[('model', '=', 'analytic_account.account')]"/>
+      <field name="model">analytic_account.account</field>
       <field name="group" ref="group_analytic_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="account_distribution_view_form">
@@ -114,22 +114,22 @@
     </record>
     <record model="ir.ui.view" id="account_distribution_view_list">
       <field name="model">analytic_account.account.distribution</field>
       <field name="type">tree</field>
       <field name="name">account_distribution_list</field>
     </record>
     <record model="ir.model.access" id="access_account_distribution">
-      <field name="model" search="[('model', '=', 'analytic_account.account.distribution')]"/>
+      <field name="model">analytic_account.account.distribution</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_distribution_account_admin">
-      <field name="model" search="[('model', '=', 'analytic_account.account.distribution')]"/>
+      <field name="model">analytic_account.account.distribution</field>
       <field name="group" ref="group_analytic_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="account_context_view_form">
@@ -145,15 +145,15 @@
     <record model="ir.ui.view" id="analytic_account_entry_view_list">
       <field name="model">analytic.account.entry</field>
       <field name="type">tree</field>
       <field name="name">analytic_account_entry_tree</field>
     </record>
     <record model="ir.rule.group" id="rule_group_entry_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'analytic.account.entry')]"/>
+      <field name="model">analytic.account.entry</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_entry_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_entry_companies"/>
     </record>
   </data>
```

### Comparing `trytond_analytic_account-7.0.0/analytic_account.xml` & `trytond_analytic_account-7.2.0/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/doc/conf.py` & `trytond_analytic_account-7.2.0/doc/conf.py`

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

### Comparing `trytond_analytic_account-7.0.0/doc/index.rst` & `trytond_analytic_account-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/line.py` & `trytond_analytic_account-7.2.0/line.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/line.xml` & `trytond_analytic_account-7.2.0/line.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_analytic_account-7.0.0/line.xml` & `trytond_analytic_account-7.2.0/line.xml`

```diff
@@ -25,30 +25,30 @@
     <record model="ir.action.act_window.view" id="act_line_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="line_view_form"/>
       <field name="act_window" ref="act_line_form"/>
     </record>
     <record model="ir.rule.group" id="rule_group_line_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'analytic_account.line')]"/>
+      <field name="model">analytic_account.line</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_line_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_line_companies"/>
     </record>
     <record model="ir.model.access" id="access_line">
-      <field name="model" search="[('model', '=', 'analytic_account.line')]"/>
+      <field name="model">analytic_account.line</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_line_account">
-      <field name="model" search="[('model', '=', 'analytic_account.line')]"/>
+      <field name="model">analytic_account.line</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.wizard" id="act_open_account">
@@ -89,13 +89,13 @@
     <record model="ir.action.act_window.view" id="act_move_line_form_completion_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account.move_line_view_form"/>
       <field name="act_window" ref="act_move_line_form_completion"/>
     </record>
     <menuitem parent="account.menu_processing" action="act_move_line_form_completion" sequence="10" id="menu_completion"/>
     <record model="ir.model.button" id="line_apply_analytic_rules_button">
+      <field name="model">account.move.line</field>
       <field name="name">apply_analytic_rules</field>
       <field name="string">Apply Analytic Rules</field>
-      <field name="model" search="[('model', '=', 'account.move.line')]"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_analytic_account-7.0.0/locale/bg.po` & `trytond_analytic_account-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/ca.po` & `trytond_analytic_account-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/cs.po` & `trytond_analytic_account-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/de.po` & `trytond_analytic_account-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/es.po` & `trytond_analytic_account-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/es_419.po` & `trytond_analytic_account-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/et.po` & `trytond_analytic_account-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/fa.po` & `trytond_analytic_account-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/fi.po` & `trytond_analytic_account-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/fr.po` & `trytond_analytic_account-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/hu.po` & `trytond_analytic_account-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/id.po` & `trytond_analytic_account-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/it.po` & `trytond_analytic_account-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/lo.po` & `trytond_analytic_account-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/lt.po` & `trytond_analytic_account-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/nl.po` & `trytond_analytic_account-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/pl.po` & `trytond_analytic_account-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/pt.po` & `trytond_analytic_account-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/ro.po` & `trytond_analytic_account-7.2.0/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -8,55 +8,55 @@
 
 msgctxt "field:account.move.line,analytic_state:"
 msgid "Analytic State"
 msgstr ""
 
 msgctxt "field:analytic.account.entry,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,root:"
 msgid "Root Analytic"
 msgstr ""
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
-msgstr "Sold"
+msgstr ""
 
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr "Copii"
+msgstr ""
 
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "field:analytic_account.account,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:analytic_account.account,debit:"
 msgid "Debit"
-msgstr "Debit"
+msgstr ""
 
 msgctxt "field:analytic_account.account,distribution_parents:"
 msgid "Distribution Parents"
 msgstr ""
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
@@ -82,26 +82,25 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
@@ -109,81 +108,79 @@
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
 msgstr ""
 
 msgctxt "field:analytic_account.line,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:analytic_account.line,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:analytic_account.line,credit:"
 msgid "Credit"
-msgstr "Credit"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
-msgstr "Debit"
+msgstr ""
 
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
 msgstr ""
 
 msgctxt "field:analytic_account.rule,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,analytic_accounts:"
 msgid "Analytic Accounts"
 msgstr ""
 
 msgctxt "field:analytic_account.rule,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
 msgstr ""
 
 msgctxt "field:analytic_account.rule,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,party_visible:"
 msgid "Party Visible"
 msgstr ""
 
 msgctxt "model:analytic.account.entry,name:"
 msgid "Analytic Account Entry"
 msgstr ""
 
 msgctxt "model:analytic_account.account,name:"
 msgid "Analytic Account"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:analytic_account.account.context,name:"
 msgid "Open Chart of Accounts"
-msgstr "Deschidere Plan de Conturi"
+msgstr ""
 
 msgctxt "model:analytic_account.account.distribution,name:"
 msgid "Analytic Account Distribution"
 msgstr ""
 
 msgctxt "model:analytic_account.line,name:"
 msgid "Analytic Line"
@@ -191,24 +188,23 @@
 
 msgctxt "model:analytic_account.rule,name:"
 msgid "Analytic Rule"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_account_list"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr "Рахунки"
 
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr "Рахунки"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Deschidere Plan de Conturi"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Analytic Lines"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_form_completion"
 msgid "Analytic Lines to Complete"
@@ -246,44 +242,43 @@
 
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr "Utilizator în companii"
+msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.rule.group,name:rule_group_entry_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr "Рахунки"
 
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr "Рахунки"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Deschidere Plan de Conturi"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr "Analitic"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
@@ -299,15 +294,15 @@
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Valid"
 msgstr ""
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Closed"
-msgstr "Închis"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Opened"
@@ -331,15 +326,15 @@
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
 msgstr ""
 
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
-msgstr "%"
+msgstr ""
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
 msgstr ""
 
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
```

### Comparing `trytond_analytic_account-7.0.0/locale/ru.po` & `trytond_analytic_account-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/sl.po` & `trytond_analytic_account-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/tr.po` & `trytond_analytic_account-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/locale/uk.po` & `trytond_analytic_account-7.2.0/locale/zh_CN.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.move.line,analytic_lines:"
 msgid "Analytic Lines"
-msgstr ""
+msgstr "Analytic Lines"
 
 msgctxt "field:account.move.line,analytic_state:"
 msgid "Analytic State"
 msgstr ""
 
 msgctxt "field:analytic.account.entry,account:"
 msgid "Account"
@@ -26,21 +27,23 @@
 msgid "Root Analytic"
 msgstr ""
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr ""
+msgstr "子项"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr ""
+msgstr "语言编码"
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
@@ -58,53 +61,61 @@
 msgid "Distribution Parents"
 msgstr ""
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,note:"
 msgid "Note"
-msgstr ""
+msgstr "注释"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "上级"
 
 msgctxt "field:analytic_account.account,root:"
 msgid "Root"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "写入日期"
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "上级"
 
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
 msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
@@ -122,37 +133,40 @@
 msgid "Credit"
 msgstr ""
 
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
 msgstr ""
 
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
 msgstr ""
 
 msgctxt "field:analytic_account.rule,account:"
 msgid "Account"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts:"
 msgid "Analytic Accounts"
-msgstr ""
+msgstr "Analytic Accounts"
 
+#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr ""
+msgstr "Analytic Accounts"
 
 msgctxt "field:analytic_account.rule,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:analytic_account.rule,journal:"
 msgid "Journal"
@@ -166,57 +180,64 @@
 msgid "Party Visible"
 msgstr ""
 
 msgctxt "model:analytic.account.entry,name:"
 msgid "Analytic Account Entry"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:analytic_account.account,name:"
 msgid "Analytic Account"
-msgstr ""
+msgstr "Analytic Account"
 
+#, fuzzy
 msgctxt "model:analytic_account.account.context,name:"
 msgid "Open Chart of Accounts"
-msgstr ""
+msgstr "Open Chart of Analytic Accounts"
 
 msgctxt "model:analytic_account.account.distribution,name:"
 msgid "Analytic Account Distribution"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:analytic_account.line,name:"
 msgid "Analytic Line"
-msgstr ""
+msgstr "Analytic Lines"
 
+#, fuzzy
 msgctxt "model:analytic_account.rule,name:"
 msgid "Analytic Rule"
-msgstr ""
+msgstr "Analytic Rules"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_account_list"
 msgid "Accounts"
-msgstr "Рахунки"
+msgstr "Open Account"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
-msgstr "Рахунки"
+msgstr "Open Account"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr ""
+msgstr "Open Chart of Analytic Accounts"
 
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Analytic Lines"
-msgstr ""
+msgstr "Analytic Lines"
 
 msgctxt "model:ir.action,name:act_move_line_form_completion"
 msgid "Analytic Lines to Complete"
-msgstr ""
+msgstr "Analytic Lines to Complete"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Account"
-msgstr ""
+msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_account_wrong_type_line"
 msgid ""
@@ -236,61 +257,66 @@
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
 msgid "Only one account is allowed by analytic root and origin."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
-msgstr ""
+msgstr "Analytic Rules"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr "Користувач у компаніях"
+msgstr "公司用户"
 
 msgctxt "model:ir.rule.group,name:rule_group_entry_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr "Користувач у компаніях"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
-msgstr "Рахунки"
+msgstr "Open Account"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
-msgstr "Рахунки"
+msgstr "Open Account"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr ""
+msgstr "Open Chart of Analytic Accounts"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr ""
+msgstr "Analytic Lines"
 
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
-msgstr ""
+msgstr "Analytic Lines to Complete"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
 msgstr ""
 
 msgctxt "model:res.group,name:group_analytic_admin"
 msgid "Analytic Administration"
-msgstr ""
+msgstr "Analytic Administration"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Valid"
@@ -316,26 +342,29 @@
 msgid "Normal"
 msgstr ""
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Root"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:analytic_account.account,type:"
 msgid "View"
-msgstr ""
+msgstr "视图"
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
-msgstr ""
+msgstr "注释"
```

### Comparing `trytond_analytic_account-7.0.0/locale/zh_CN.po` & `trytond_analytic_account-7.2.0/locale/ro.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,370 +1,367 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:account.move.line,analytic_lines:"
 msgid "Analytic Lines"
-msgstr "Analytic Lines"
+msgstr "Rânduri Analitice"
 
 msgctxt "field:account.move.line,analytic_state:"
 msgid "Analytic State"
-msgstr ""
+msgstr "Stare Analitică"
 
 msgctxt "field:analytic.account.entry,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt "field:analytic.account.entry,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:analytic.account.entry,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:analytic.account.entry,root:"
 msgid "Root Analytic"
 msgstr ""
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
-msgstr ""
+msgstr "Sold"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr "子项"
+msgstr "Copii"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr "语言编码"
+msgstr "Cod"
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Credit"
 
 msgctxt "field:analytic_account.account,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valută"
 
 msgctxt "field:analytic_account.account,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Debit"
 
 msgctxt "field:analytic_account.account,distribution_parents:"
 msgid "Distribution Parents"
 msgstr ""
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
-msgstr ""
+msgstr "Distribuții"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nume"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,note:"
 msgid "Note"
-msgstr "注释"
+msgstr "Notă"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,parent:"
 msgid "Parent"
-msgstr "上级"
+msgstr ""
 
 msgctxt "field:analytic_account.account,root:"
 msgid "Root"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:analytic_account.account,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
 #, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr "日期格式"
+msgstr "Data de sfârșit"
 
 #, fuzzy
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
-msgstr "写入日期"
+msgstr "Data de Început"
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
-#, fuzzy
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
-msgstr "上级"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
-msgstr ""
+msgstr "Rație"
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
 msgstr ""
 
 msgctxt "field:analytic_account.line,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt "field:analytic_account.line,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:analytic_account.line,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Credit"
 
+#, fuzzy
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Debit"
 
+#, fuzzy
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
-msgstr ""
+msgstr "Rând Mişcare Cont"
 
 msgctxt "field:analytic_account.rule,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
-#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts:"
 msgid "Analytic Accounts"
-msgstr "Analytic Accounts"
+msgstr "Conturi Analitice"
 
-#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr "Analytic Accounts"
+msgstr "Mărimea Conturilor Analitice"
 
 msgctxt "field:analytic_account.rule,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:analytic_account.rule,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:analytic_account.rule,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:analytic_account.rule,party_visible:"
 msgid "Party Visible"
 msgstr ""
 
 msgctxt "model:analytic.account.entry,name:"
 msgid "Analytic Account Entry"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:analytic_account.account,name:"
 msgid "Analytic Account"
-msgstr "Analytic Account"
+msgstr "Cont Analitic"
 
 #, fuzzy
 msgctxt "model:analytic_account.account.context,name:"
 msgid "Open Chart of Accounts"
-msgstr "Open Chart of Analytic Accounts"
+msgstr "Deschidere Plan de Conturi"
 
+#, fuzzy
 msgctxt "model:analytic_account.account.distribution,name:"
 msgid "Analytic Account Distribution"
-msgstr ""
+msgstr "Distribuția analitică a conturilor"
 
 #, fuzzy
 msgctxt "model:analytic_account.line,name:"
 msgid "Analytic Line"
-msgstr "Analytic Lines"
+msgstr "Rând Analitic"
 
 #, fuzzy
 msgctxt "model:analytic_account.rule,name:"
 msgid "Analytic Rule"
-msgstr "Analytic Rules"
+msgstr "Regulă analitică"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_list"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Conturi"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Conturi"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Open Chart of Analytic Accounts"
+msgstr "Planu de Conturi Analitice"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Analytic Lines"
-msgstr "Analytic Lines"
+msgstr "Rânduri Analitice"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_move_line_form_completion"
 msgid "Analytic Lines to Complete"
-msgstr "Analytic Lines to Complete"
+msgstr "Rânduri analitice de completat"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Account"
-msgstr "Open Account"
+msgstr "Cont deschis"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
-msgstr ""
+msgstr "Reguli"
 
 msgctxt "model:ir.message,text:msg_account_wrong_type_line"
 msgid ""
 "You cannot change the type of account \"%(account)s\" because it has move "
 "lines."
 msgstr ""
+"Nu puteți schimba tipul de cont \"%(account)s\" deoarece are rânduri de "
+"mişcare."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_analytic_account_root_change"
 msgid ""
 "You cannot change the root of the analytic account \"%(account)s\" which is "
 "associated with analytic account entry."
 msgstr ""
+"Nu puteți modifica rădăcina contului analitic „%(account)s”, care este "
+"asociată cu introducerea contului analitic."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
+"Pentru a salva contul „%(account)s”, suma distribuțiilor acestora trebuie să"
+" fie de 100%."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_root_origin_unique"
 msgid "Only one account is allowed by analytic root and origin."
-msgstr ""
+msgstr "Un singur cont este permis după rădăcina analitică și origine."
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
-msgstr "Analytic Rules"
+msgstr "Aplicare reguli analitice"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr "公司用户"
+msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_entry_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în companii"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Conturi"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Conturi"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Open Chart of Analytic Accounts"
+msgstr "Plan de Conturi Analitice"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr "Analytic Lines"
+msgstr "Analitic"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
-msgstr "Analytic Lines to Complete"
+msgstr "Rânduri analitice de completat"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
-msgstr ""
+msgstr "Reguli"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_analytic_admin"
 msgid "Analytic Administration"
-msgstr "Analytic Administration"
+msgstr "Administrare analitică"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Draft"
-msgstr ""
+msgstr "Ciornă"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Valid"
-msgstr ""
+msgstr "Valabil"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Closed"
-msgstr ""
+msgstr "Închis"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Ciornă"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Opened"
-msgstr ""
+msgstr "Deschis"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Distribution"
-msgstr ""
+msgstr "Distribuție"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Normal"
-msgstr ""
+msgstr "Normal"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Root"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:analytic_account.account,type:"
 msgid "View"
-msgstr "视图"
+msgstr "Vedere"
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
-msgstr ""
+msgstr "Analitic"
 
-#, fuzzy
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
-msgstr ""
+msgstr "Informații Generale"
 
-#, fuzzy
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
-msgstr "注释"
+msgstr "Notiţe"
```

### Comparing `trytond_analytic_account-7.0.0/message.xml` & `trytond_analytic_account-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/rule.py` & `trytond_analytic_account-7.2.0/rule.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/rule.xml` & `trytond_analytic_account-7.2.0/rule.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_analytic_account-7.0.0/rule.xml` & `trytond_analytic_account-7.2.0/rule.xml`

```diff
@@ -26,30 +26,30 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="rule_view_form"/>
       <field name="act_window" ref="act_rule_form"/>
     </record>
     <menuitem parent="menu_analytic_account_configuration" action="act_rule_form" sequence="50" id="menu_rule_form"/>
     <record model="ir.rule.group" id="rule_group_rule_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'analytic_account.rule')]"/>
+      <field name="model">analytic_account.rule</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_rule_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_rule_companies"/>
     </record>
     <record model="ir.model.access" id="access_rule">
-      <field name="model" search="[('model', '=', 'analytic_account.rule')]"/>
+      <field name="model">analytic_account.rule</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_rule_account_admin">
-      <field name="model" search="[('model', '=', 'analytic_account.rule')]"/>
+      <field name="model">analytic_account.rule</field>
       <field name="group" ref="group_analytic_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_analytic_account-7.0.0/setup.py` & `trytond_analytic_account-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/tests/scenario_analytic_account.rst` & `trytond_analytic_account-7.2.0/tests/scenario_analytic_account.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 =========================
 Analytic Account Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('analytic_account')
 
     >>> Reconciliation = Model.get('account.move.reconciliation')
 
@@ -102,16 +102,15 @@
     >>> cancel_move.execute('cancel')
     >>> move.reload()
     >>> line, = [l for l in move.lines if l.account == receivable]
     >>> bool(line.reconciliation)
     True
     >>> cancel_move, = [l.move for l in line.reconciliation.lines
     ...     if l.move != move]
-    >>> cancel_move.origin == move
-    True
+    >>> assertEqual(cancel_move.origin, move)
     >>> analytic_account.reload()
     >>> analytic_account.credit
     Decimal('42.00')
     >>> analytic_account.debit
     Decimal('42.00')
 
     >>> reconciliations = {
@@ -134,16 +133,15 @@
     >>> cancel_move.execute('cancel')
     >>> move.reload()
     >>> line, = [l for l in move.lines if l.account == receivable]
     >>> bool(line.reconciliation)
     True
     >>> cancel_move, = [l.move for l in line.reconciliation.lines
     ...     if l.move != move]
-    >>> cancel_move.origin == move
-    True
+    >>> assertEqual(cancel_move.origin, move)
     >>> analytic_account.reload()
     >>> analytic_account.credit
     Decimal('0.00')
     >>> analytic_account.debit
     Decimal('0.00')
 
 Create Move without analytic accounts::
@@ -161,20 +159,18 @@
     >>> line.party = customer
 
 Check analytic lines are created on posting::
 
     >>> move.click('post')
     >>> line, = [l for l in move.lines if l.analytic_lines]
     >>> analytic_line, = line.analytic_lines
-    >>> analytic_line.account == analytic_account2
-    True
+    >>> assertEqual(analytic_line.account, analytic_account2)
     >>> analytic_line.credit
     Decimal('73')
-    >>> analytic_line.date == analytic_line.move_line.date
-    True
+    >>> assertEqual(analytic_line.date, analytic_line.move_line.date)
 
 Prepare to balance non-deferral accounts::
 
     >>> Sequence = Model.get('ir.sequence')
     >>> Period = Model.get('account.period')
     >>> AccountType = Model.get('account.account.type')
     >>> Account = Model.get('account.account')
@@ -216,25 +212,25 @@
     []
 
 Prevent changing root of account with entries::
 
     >>> root2 = AnalyticAccount(type='root', name="Root2")
     >>> root2.save()
     >>> analytic_account.root = root2
-    >>> analytic_account.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> analytic_account.save()
     Traceback (most recent call last):
         ...
     AccessError: ...
 
     >>> analytic_account.reload()
     >>> analytic_account.code = "1"
     >>> analytic_account.save()
     >>> analytic_account.code
     '1'
 
 Prevent changing type of analytic account with lines::
 
     >>> analytic_account.type = 'view'
-    >>> analytic_account.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> analytic_account.save()
     Traceback (most recent call last):
         ...
     AccountValidationError: ...
```

### Comparing `trytond_analytic_account-7.0.0/tests/test_module.py` & `trytond_analytic_account-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/tox.ini` & `trytond_analytic_account-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/PKG-INFO` & `trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-analytic-account
-Version: 7.0.0
+Name: trytond_analytic_account
+Version: 7.2.0
 Summary: Tryton module for analytic accounting
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
@@ -49,21 +49,21 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Analytic Account Module
 #######################
 
 The analytic account module adds the fundamentals required to analyse
 accounting using multiple different axes.
```

### Comparing `trytond_analytic_account-7.0.0/trytond_analytic_account.egg-info/SOURCES.txt` & `trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/SOURCES.txt`

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

### Comparing `trytond_analytic_account-7.0.0/view/account_form.xml` & `trytond_analytic_account-7.2.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/view/move_line_list.xml` & `trytond_analytic_account-7.2.0/view/move_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.0.0/view/rule_form.xml` & `trytond_analytic_account-7.2.0/view/rule_form.xml`

 * *Files identical despite different names*

