# Comparing `tmp/trytond_account_rule-7.0.0.tar.gz` & `tmp/trytond_account_rule-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_rule-7.0.0.tar", last modified: Mon Oct 30 17:24:04 2023, max compression
+gzip compressed data, was "trytond_account_rule-7.2.0.tar", last modified: Mon Apr 29 15:35:35 2024, max compression
```

## Comparing `trytond_account_rule-7.0.0.tar` & `trytond_account_rule-7.2.0.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:04.907119 trytond_account_rule-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-10-22 17:22:54.000000 trytond_account_rule-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      627 2023-10-30 17:03:05.000000 trytond_account_rule-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:03:05.000000 trytond_account_rule-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3414 2023-10-30 17:24:04.907119 trytond_account_rule-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5523 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3756 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:04.903785 trytond_account_rule-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2813 2023-10-22 17:22:54.000000 trytond_account_rule-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:54.000000 trytond_account_rule-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:04.900452 trytond_account_rule-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1864 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1855 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1836 2023-10-30 16:47:45.000000 trytond_account_rule-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1635 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1648 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1851 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1827 2023-10-30 16:47:45.000000 trytond_account_rule-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2023-10-28 12:11:20.000000 trytond_account_rule-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1755 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-07 15:40:36.000000 trytond_account_rule-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-10-07 15:40:36.000000 trytond_account_rule-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:24:04.907119 trytond_account_rule-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5177 2023-10-27 17:38:49.000000 trytond_account_rule-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:04.900452 trytond_account_rule-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3186 2023-10-07 15:40:36.000000 trytond_account_rule-7.0.0/tests/scenario_account_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_rule-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-10-30 17:03:02.000000 trytond_account_rule-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:04.903785 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3414 2023-10-30 17:24:04.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1815 2023-10-30 17:24:04.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:24:04.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-30 17:24:04.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-10-30 17:24:04.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:24:04.000000 trytond_account_rule-7.0.0/trytond_account_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:04.903785 trytond_account_rule-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      719 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/view/account_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/view/account_rule_form_stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/view/account_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_account_rule-7.0.0/view/account_rule_list_stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:35.493699 trytond_account_rule-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:15:44.000000 trytond_account_rule-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:44.000000 trytond_account_rule-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-04-29 15:35:35.493699 trytond_account_rule-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5523 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3687 2024-04-27 16:30:39.000000 trytond_account_rule-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:35.490366 trytond_account_rule-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-27 16:30:39.000000 trytond_account_rule-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_rule-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:35.490366 trytond_account_rule-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1864 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1855 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1836 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1635 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1648 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1851 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1594 2024-04-29 13:17:17.000000 trytond_account_rule-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1827 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-27 16:43:21.000000 trytond_account_rule-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1755 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-01-27 09:58:52.000000 trytond_account_rule-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-01-27 09:58:52.000000 trytond_account_rule-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:35.493699 trytond_account_rule-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5168 2024-04-27 16:30:39.000000 trytond_account_rule-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:35.493699 trytond_account_rule-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3163 2024-04-22 12:14:36.000000 trytond_account_rule-7.2.0/tests/scenario_account_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_rule-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-04-29 15:15:40.000000 trytond_account_rule-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:35.493699 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-04-29 15:35:35.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2024-04-29 15:35:35.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:35.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:35:35.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2024-04-29 15:35:35.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:35.000000 trytond_account_rule-7.2.0/trytond_account_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:35.493699 trytond_account_rule-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      719 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/view/account_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/view/account_rule_form_stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/view/account_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_account_rule-7.2.0/view/account_rule_list_stock.xml
```

### Comparing `trytond_account_rule-7.0.0/LICENSE` & `trytond_account_rule-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/PKG-INFO` & `trytond_account_rule-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_rule
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to change account used with rules
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-rule
+Project-URL: Documentation, https://docs.tryton.org/modules-account-rule
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account rule determination tax warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,31 +47,31 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
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
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_anglo_saxon<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_gift_card<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_consignment<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_anglo_saxon<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_gift_card<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_consignment<7.3,>=7.2; extra == "test"
 
 ###################
 Account Rule Module
 ###################
 
 The *Account Rule Module* allows rules which substitute default accounts with
 other accounts.
```

### Comparing `trytond_account_rule-7.0.0/__init__.py` & `trytond_account_rule-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/account.py` & `trytond_account_rule-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/account.xml` & `trytond_account_rule-7.2.0/account.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_account_rule-7.0.0/account.xml` & `trytond_account_rule-7.2.0/account.xml`

```diff
@@ -26,31 +26,31 @@
     <record model="ir.action.act_window.view" id="act_account_rule_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_rule_view_form"/>
       <field name="act_window" ref="act_account_rule_form"/>
     </record>
     <menuitem parent="account.menu_general_account_configuration" action="act_account_rule_form" sequence="50" id="menu_account_rule_form"/>
     <record model="ir.model.access" id="access_account_rule">
-      <field name="model" search="[('model', '=', 'account.account.rule')]"/>
+      <field name="model">account.account.rule</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_rule_account_admin">
-      <field name="model" search="[('model', '=', 'account.account.rule')]"/>
+      <field name="model">account.account.rule</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_account_rule_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.account.rule')]"/>
+      <field name="model">account.account.rule</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_account_rule_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_account_rule_companies"/>
     </record>
   </data>
```

### Comparing `trytond_account_rule-7.0.0/doc/conf.py` & `trytond_account_rule-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_rule-7.0.0/doc/design.rst` & `trytond_account_rule-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/bg.po` & `trytond_account_rule-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/ca.po` & `trytond_account_rule-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/cs.po` & `trytond_account_rule-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/de.po` & `trytond_account_rule-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/es.po` & `trytond_account_rule-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/es_419.po` & `trytond_account_rule-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/et.po` & `trytond_account_rule-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/fa.po` & `trytond_account_rule-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/fi.po` & `trytond_account_rule-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/fr.po` & `trytond_account_rule-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/hu.po` & `trytond_account_rule-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/id.po` & `trytond_account_rule-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/it.po` & `trytond_account_rule-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/lo.po` & `trytond_account_rule-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/lt.po` & `trytond_account_rule-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/nl.po` & `trytond_account_rule-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/pl.po` & `trytond_account_rule-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/pt.po` & `trytond_account_rule-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/ro.po` & `trytond_account_rule-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/ru.po` & `trytond_account_rule-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/sl.po` & `trytond_account_rule-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/tr.po` & `trytond_account_rule-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/uk.po` & `trytond_account_rule-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/locale/zh_CN.po` & `trytond_account_rule-7.2.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #
+#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.rule,account:"
 msgid "Substitution Account"
 msgstr ""
 
@@ -60,15 +61,15 @@
 
 msgctxt "selection:account.account.rule,type:"
 msgid "Expense"
 msgstr ""
 
 msgctxt "selection:account.account.rule,type:"
 msgid "Payable"
-msgstr ""
+msgstr "Furnizor"
 
 msgctxt "selection:account.account.rule,type:"
 msgid "Receivable"
 msgstr ""
 
 msgctxt "selection:account.account.rule,type:"
 msgid "Revenue"
```

### Comparing `trytond_account_rule-7.0.0/party.py` & `trytond_account_rule-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/product.py` & `trytond_account_rule-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/purchase.py` & `trytond_account_rule-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/sale.py` & `trytond_account_rule-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/setup.py` & `trytond_account_rule-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-rule'),
+            'https://docs.tryton.org/modules-account-rule'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account rule determination tax warehouse',
     package_dir={'trytond.modules.account_rule': '.'},
     packages=(
         ['trytond.modules.account_rule']
```

### Comparing `trytond_account_rule-7.0.0/stock.py` & `trytond_account_rule-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/tests/scenario_account_rule.rst` & `trytond_account_rule-7.2.0/tests/scenario_account_rule.rst`

 * *Files 25% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Account Rule Scenario
 =====================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax)
+    ...     create_chart, create_tax, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['account_rule', 'product', 'sale'])
 
     >>> AccountRule = Model.get('account.account.rule')
     >>> Party = Model.get('party.party')
@@ -100,13 +99,10 @@
     >>> line.description = 'Sample'
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> sale.state
     'processing'
 
     >>> invoice, = sale.invoices
-    >>> invoice.lines[0].account == account_revenue1
-    True
-    >>> invoice.lines[1].account == account_revenue2
-    True
-    >>> invoice.lines[2].account == account_revenue3
-    True
+    >>> assertEqual(invoice.lines[0].account, account_revenue1)
+    >>> assertEqual(invoice.lines[1].account, account_revenue2)
+    >>> assertEqual(invoice.lines[2].account, account_revenue3)
```

### Comparing `trytond_account_rule-7.0.0/tests/test_module.py` & `trytond_account_rule-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/tox.ini` & `trytond_account_rule-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/trytond_account_rule.egg-info/PKG-INFO` & `trytond_account_rule-7.2.0/trytond_account_rule.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-rule
-Version: 7.0.0
+Name: trytond_account_rule
+Version: 7.2.0
 Summary: Tryton module to change account used with rules
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-rule
+Project-URL: Documentation, https://docs.tryton.org/modules-account-rule
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account rule determination tax warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,31 +47,31 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
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
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_anglo_saxon<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_gift_card<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_consignment<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_anglo_saxon<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_gift_card<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_consignment<7.3,>=7.2; extra == "test"
 
 ###################
 Account Rule Module
 ###################
 
 The *Account Rule Module* allows rules which substitute default accounts with
 other accounts.
```

### Comparing `trytond_account_rule-7.0.0/trytond_account_rule.egg-info/SOURCES.txt` & `trytond_account_rule-7.2.0/trytond_account_rule.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_rule-7.0.0/view/account_rule_form.xml` & `trytond_account_rule-7.2.0/view/account_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_rule-7.0.0/view/account_rule_list.xml` & `trytond_account_rule-7.2.0/view/account_rule_list.xml`

 * *Files identical despite different names*

