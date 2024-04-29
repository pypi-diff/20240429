# Comparing `tmp/trytond_account_receivable_rule-7.0.0.tar.gz` & `tmp/trytond_account_receivable_rule-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_receivable_rule-7.0.0.tar", last modified: Mon Oct 30 17:23:58 2023, max compression
+gzip compressed data, was "trytond_account_receivable_rule-7.2.0.tar", last modified: Mon Apr 29 15:35:29 2024, max compression
```

## Comparing `trytond_account_receivable_rule-7.0.0.tar` & `trytond_account_receivable_rule-7.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:58.033753 trytond_account_receivable_rule-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:22:54.000000 trytond_account_receivable_rule-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:03:01.000000 trytond_account_receivable_rule-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:03:01.000000 trytond_account_receivable_rule-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2722 2023-10-30 17:23:58.033753 trytond_account_receivable_rule-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14188 2023-10-07 15:40:36.000000 trytond_account_receivable_rule-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4473 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:58.030419 trytond_account_receivable_rule-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:22:54.000000 trytond_account_receivable_rule-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:54.000000 trytond_account_receivable_rule-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:58.027086 trytond_account_receivable_rule-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3874 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3892 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3877 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3289 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4111 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-10-28 12:11:20.000000 trytond_account_receivable_rule-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:23:58.033753 trytond_account_receivable_rule-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4675 2023-10-27 17:38:49.000000 trytond_account_receivable_rule-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:58.030419 trytond_account_receivable_rule-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4519 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/tests/scenario_account_receivable_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3557 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/tests/scenario_account_receivable_rule_overflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_receivable_rule-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-10-30 17:02:57.000000 trytond_account_receivable_rule-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:58.030419 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2722 2023-10-30 17:23:57.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2080 2023-10-30 17:23:58.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:23:57.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:23:57.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-10-30 17:23:57.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:23:57.000000 trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:58.030419 trytond_account_receivable_rule-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/view/account_receivable_rule_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/view/account_receivable_rule_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-10-07 15:40:36.000000 trytond_account_receivable_rule-7.0.0/view/account_receivable_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.0.0/view/account_receivable_rule_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:15:39.000000 trytond_account_receivable_rule-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:39.000000 trytond_account_receivable_rule-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      893 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14181 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4381 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.790515 trytond_account_receivable_rule-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_receivable_rule-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.793848 trytond_account_receivable_rule-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3874 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3892 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3877 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3289 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4111 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3604 2024-04-29 13:17:17.000000 trytond_account_receivable_rule-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4731 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.793848 trytond_account_receivable_rule-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4496 2024-04-22 12:14:36.000000 trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3534 2024-04-22 12:14:36.000000 trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_overflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4028 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_receivable_rule-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-04-29 15:15:35.000000 trytond_account_receivable_rule-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2170 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-02-04 18:51:26.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_list.xml
```

### Comparing `trytond_account_receivable_rule-7.0.0/COPYRIGHT` & `trytond_account_receivable_rule-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
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

### Comparing `trytond_account_receivable_rule-7.0.0/LICENSE` & `trytond_account_receivable_rule-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/PKG-INFO` & `trytond_account_receivable_rule-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_receivable_rule
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to enforce receivable rules
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-receivable-rule
+Project-URL: Documentation, https://docs.tryton.org/modules-account-receivable-rule
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account receivable rules
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,21 @@
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
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement<7.3,>=7.2; extra == "test"
 
 ##############################
 Account Receivable Rule Module
 ##############################
 
 The *Account Receivable Rule Module* defines rules to reconcile receivable
 between accounts.
```

### Comparing `trytond_account_receivable_rule-7.0.0/__init__.py` & `trytond_account_receivable_rule-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/account.py` & `trytond_account_receivable_rule-7.2.0/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,14 @@
     __name__ = 'account.statement'
 
     @classmethod
     @ModelView.button
     @Workflow.transition('posted')
     def post(cls, statements):
         pool = Pool()
-        Rule = pool.get('account.account.receivable.rules')
+        Rule = pool.get('account.account.receivable.rule')
         super().post(statements)
         rules = set()
         for statement in statements:
             for line in statement.lines:
                 rules.update(line.account.receivable_rules)
-        Rule.apply(rules=Rule.browse(rules))
+        Rule.apply(Rule.browse(rules))
```

### Comparing `trytond_account_receivable_rule-7.0.0/account.xml` & `trytond_account_receivable_rule-7.2.0/account.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_account_receivable_rule-7.0.0/account.xml` & `trytond_account_receivable_rule-7.2.0/account.xml`

```diff
@@ -25,40 +25,40 @@
     <record model="ir.action.act_window.view" id="act_account_receivable_rule_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_receivable_rule_view_form"/>
       <field name="act_window" ref="act_account_receivable_rule_form"/>
     </record>
     <menuitem parent="account.menu_general_account_configuration" action="act_account_receivable_rule_form" sequence="20" id="menu_account_receivable_rule_form"/>
     <record model="ir.model.access" id="access_account_receivable_rule">
-      <field name="model" search="[('model', '=', 'account.account.receivable.rule')]"/>
+      <field name="model">account.account.receivable.rule</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_receivable_rule_account_admin">
-      <field name="model" search="[('model', '=', 'account.account.receivable.rule')]"/>
+      <field name="model">account.account.receivable.rule</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="account_receivable_rule_apply_button">
+      <field name="model">account.account.receivable.rule</field>
       <field name="name">apply</field>
       <field name="string">Apply</field>
-      <field name="model" search="[('model', '=', 'account.account.receivable.rule')]"/>
     </record>
     <record model="ir.model.button-res.group" id="account_receivable_rule_apply_button_group_account">
       <field name="button" ref="account_receivable_rule_apply_button"/>
       <field name="group" ref="account.group_account"/>
     </record>
     <record model="ir.rule.group" id="rule_group_account_receivable_rule_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.account.receivable.rule')]"/>
+      <field name="model">account.account.receivable.rule</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_account_receivable_rule_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_account_receivable_rule_companies"/>
     </record>
     <record model="ir.ui.view" id="account_receivable_rule_account_view_form">
```

### Comparing `trytond_account_receivable_rule-7.0.0/doc/conf.py` & `trytond_account_receivable_rule-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_receivable_rule-7.0.0/doc/design.rst` & `trytond_account_receivable_rule-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/bg.po` & `trytond_account_receivable_rule-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/ca.po` & `trytond_account_receivable_rule-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/cs.po` & `trytond_account_receivable_rule-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/de.po` & `trytond_account_receivable_rule-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/es.po` & `trytond_account_receivable_rule-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/es_419.po` & `trytond_account_receivable_rule-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/et.po` & `trytond_account_receivable_rule-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/fa.po` & `trytond_account_receivable_rule-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/fi.po` & `trytond_account_receivable_rule-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/fr.po` & `trytond_account_receivable_rule-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/hu.po` & `trytond_account_receivable_rule-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/id.po` & `trytond_account_receivable_rule-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/it.po` & `trytond_account_receivable_rule-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/lo.po` & `trytond_account_receivable_rule-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/lt.po` & `trytond_account_receivable_rule-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/nl.po` & `trytond_account_receivable_rule-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/pl.po` & `trytond_account_receivable_rule-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/pt.po` & `trytond_account_receivable_rule-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/ro.po` & `trytond_account_receivable_rule-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/ru.po` & `trytond_account_receivable_rule-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/sl.po` & `trytond_account_receivable_rule-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/tr.po` & `trytond_account_receivable_rule-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/uk.po` & `trytond_account_receivable_rule-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/locale/zh_CN.po` & `trytond_account_receivable_rule-7.2.0/locale/ro.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account,receivable_rules:"
 msgid "Receivable Rules"
-msgstr ""
+msgstr "Reguli Client"
 
 msgctxt "field:account.account.receivable.rule,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt "field:account.account.receivable.rule,account_party_required:"
 msgid "Account Party Required"
 msgstr ""
 
 msgctxt "field:account.account.receivable.rule,account_payable:"
 msgid "Account Payable"
-msgstr ""
+msgstr "Cont Furnizor"
 
 msgctxt "field:account.account.receivable.rule,account_receivable:"
 msgid "Account Receivable"
-msgstr ""
+msgstr "Cont Client"
 
 msgctxt "field:account.account.receivable.rule,accounts:"
 msgid "Accounts"
-msgstr ""
+msgstr "Conturi"
 
 msgctxt "field:account.account.receivable.rule,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.account.receivable.rule,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.account.receivable.rule,overflow_account:"
 msgid "Overflow Account"
 msgstr ""
 
 msgctxt "field:account.account.receivable.rule,priorities:"
 msgid "Priorities"
-msgstr ""
+msgstr "Priorități"
 
 msgctxt "field:account.account.receivable.rule.account,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt ""
 "field:account.account.receivable.rule.account,account_party_required:"
 msgid "Account Party Required"
-msgstr ""
+msgstr "Parte este Necesară pentru Cont"
 
 msgctxt "field:account.account.receivable.rule.account,account_payable:"
 msgid "Account Payable"
-msgstr ""
+msgstr "Cont Furnizor"
 
 msgctxt "field:account.account.receivable.rule.account,account_receivable:"
 msgid "Account Receivable"
 msgstr ""
 
 msgctxt "field:account.account.receivable.rule.account,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.account.receivable.rule.account,only_reconcile:"
 msgid "Only Reconcile"
-msgstr ""
+msgstr "Doar Reconciliere"
 
 msgctxt "field:account.account.receivable.rule.account,rule:"
 msgid "Rule"
-msgstr ""
+msgstr "Regulă"
 
 msgctxt "help:account.account.receivable.rule,overflow_account:"
 msgid ""
 "The account to move exceeded amount.\n"
 "Leave empty to keep it in the current account."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:account.account.receivable.rule.account,only_reconcile:"
 msgid "Distribute only to fully reconcile."
-msgstr ""
+msgstr "Distribuiți numai pentru a reconcilia pe deplin."
 
 msgctxt "model:account.account.receivable.rule,name:"
 msgid "Account Receivable Rule"
 msgstr ""
 
 msgctxt "model:account.account.receivable.rule.account,name:"
 msgid "Account Receivable Rule Account"
@@ -91,37 +92,39 @@
 
 msgctxt "model:ir.action,name:act_account_receivable_rule_form"
 msgid "Account Receivable Rules"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_account_unique"
 msgid "Only one active rule is allowed by account."
-msgstr ""
+msgstr "Este permisă o singură regulă activă pe cont."
 
 msgctxt "model:ir.message,text:msg_rule_account_unique"
 msgid "Only one account is allowed by rule."
-msgstr ""
+msgstr "Un singur cont este permis de regulă."
 
 msgctxt "model:ir.model.button,string:account_receivable_rule_apply_button"
 msgid "Apply"
-msgstr ""
+msgstr "Aplicare"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_account_receivable_rule_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în companii"
 
 msgctxt "model:ir.ui.menu,name:menu_account_receivable_rule_form"
 msgid "Account Receivable Rules"
-msgstr ""
+msgstr "Reguli Cont Client"
 
+#, fuzzy
 msgctxt "selection:account.account.receivable.rule,priorities:"
 msgid "Account, Maturity Date"
-msgstr ""
+msgstr "Cont, Data scadenței"
 
+#, fuzzy
 msgctxt "selection:account.account.receivable.rule,priorities:"
 msgid "Maturity Date, Account"
-msgstr ""
+msgstr "Data scadenței, cont"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Apply Account Receivable Rules"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_receivable_rule-7.0.0/message.xml` & `trytond_account_receivable_rule-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/setup.py` & `trytond_account_receivable_rule-7.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,28 +46,31 @@
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond_account_statement'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module to enforce receivable rules',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-receivable-rule'
+            'https://docs.tryton.org/modules-account-receivable-rule'
             ),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account receivable rules',
     package_dir={'trytond.modules.account_receivable_rule': '.'},
     packages=(
```

### Comparing `trytond_account_receivable_rule-7.0.0/tests/scenario_account_receivable_rule.rst` & `trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Account Receivable Rule Scenario
 ================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_receivable_rule')
 
     >>> Journal = Model.get('account.journal')
     >>> Party = Model.get('party.party')
```

### Comparing `trytond_account_receivable_rule-7.0.0/tests/scenario_account_receivable_rule_overflow.rst` & `trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_overflow.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Account Receivable Rule Overflow Scenario
 =========================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_receivable_rule')
 
     >>> Journal = Model.get('account.journal')
     >>> Party = Model.get('party.party')
```

### Comparing `trytond_account_receivable_rule-7.0.0/tox.ini` & `trytond_account_receivable_rule-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/PKG-INFO` & `trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-receivable-rule
-Version: 7.0.0
+Name: trytond_account_receivable_rule
+Version: 7.2.0
 Summary: Tryton module to enforce receivable rules
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-receivable-rule
+Project-URL: Documentation, https://docs.tryton.org/modules-account-receivable-rule
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account receivable rules
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,21 @@
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
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement<7.3,>=7.2; extra == "test"
 
 ##############################
 Account Receivable Rule Module
 ##############################
 
 The *Account Receivable Rule Module* defines rules to reconcile receivable
 between accounts.
```

### Comparing `trytond_account_receivable_rule-7.0.0/trytond_account_receivable_rule.egg-info/SOURCES.txt` & `trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/SOURCES.txt`

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
 account.py
@@ -41,14 +40,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_account_receivable_rule.rst
 ./tests/scenario_account_receivable_rule_overflow.rst
+./tests/scenario_account_receivable_rule_statement.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/account_receivable_rule_account_form.xml
 ./view/account_receivable_rule_account_list.xml
 ./view/account_receivable_rule_form.xml
 ./view/account_receivable_rule_list.xml
 doc/conf.py
@@ -81,14 +81,15 @@
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_account_receivable_rule.rst
 tests/scenario_account_receivable_rule_overflow.rst
+tests/scenario_account_receivable_rule_statement.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_account_receivable_rule.egg-info/PKG-INFO
 trytond_account_receivable_rule.egg-info/SOURCES.txt
 trytond_account_receivable_rule.egg-info/dependency_links.txt
 trytond_account_receivable_rule.egg-info/entry_points.txt
 trytond_account_receivable_rule.egg-info/not-zip-safe
```

### Comparing `trytond_account_receivable_rule-7.0.0/view/account_receivable_rule_form.xml` & `trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_form.xml`

 * *Files identical despite different names*

