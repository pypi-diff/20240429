# Comparing `tmp/trytond_account_statement_rule-7.0.0.tar.gz` & `tmp/trytond_account_statement_rule-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_rule-7.0.0.tar", last modified: Mon Oct 30 17:24:46 2023, max compression
+gzip compressed data, was "trytond_account_statement_rule-7.2.0.tar", last modified: Mon Apr 29 15:36:13 2024, max compression
```

## Comparing `trytond_account_statement_rule-7.0.0.tar` & `trytond_account_statement_rule-7.2.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:46.680651 trytond_account_statement_rule-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:22:56.000000 trytond_account_statement_rule-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1024 2023-10-30 17:03:32.000000 trytond_account_statement_rule-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:03:31.000000 trytond_account_statement_rule-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4478 2023-10-30 17:24:46.680651 trytond_account_statement_rule-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15926 2023-08-13 15:26:13.000000 trytond_account_statement_rule-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5496 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:46.677318 trytond_account_statement_rule-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:22:56.000000 trytond_account_statement_rule-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:56.000000 trytond_account_statement_rule-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:46.673985 trytond_account_statement_rule-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5079 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2023-10-30 16:47:45.000000 trytond_account_statement_rule-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4268 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5253 2023-10-30 16:47:45.000000 trytond_account_statement_rule-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4157 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2023-10-30 16:47:45.000000 trytond_account_statement_rule-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4088 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-10-28 12:11:20.000000 trytond_account_statement_rule-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:24:46.680651 trytond_account_statement_rule-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2023-10-27 17:38:49.000000 trytond_account_statement_rule-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:46.677318 trytond_account_statement_rule-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2660 2023-06-10 11:39:56.000000 trytond_account_statement_rule-7.0.0/tests/scenario_account_statement_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3944 2023-06-10 11:39:56.000000 trytond_account_statement_rule-7.0.0/tests/scenario_account_statement_rule_keyword_bank_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3489 2023-06-10 11:39:56.000000 trytond_account_statement_rule-7.0.0/tests/scenario_account_statement_rule_keywords.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_statement_rule-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-10-30 17:03:28.000000 trytond_account_statement_rule-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:46.680651 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4478 2023-10-30 17:24:46.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2157 2023-10-30 17:24:46.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:24:46.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:24:46.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:24:46.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:24:46.000000 trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:24:46.677318 trytond_account_statement_rule-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-10-07 15:40:36.000000 trytond_account_statement_rule-7.0.0/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1031 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/rule_information_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/rule_information_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/rule_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.0.0/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1125 2024-04-29 15:16:15.000000 trytond_account_statement_rule-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:16:14.000000 trytond_account_statement_rule-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15926 2024-01-27 09:58:52.000000 trytond_account_statement_rule-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5381 2024-04-27 16:30:39.000000 trytond_account_statement_rule-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.072717 trytond_account_statement_rule-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_statement_rule-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:00.000000 trytond_account_statement_rule-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.072717 trytond_account_statement_rule-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5079 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5253 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4673 2024-04-29 13:17:17.000000 trytond_account_statement_rule-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4088 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2024-03-17 11:01:36.000000 trytond_account_statement_rule-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.072717 trytond_account_statement_rule-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2641 2024-04-22 12:14:36.000000 trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3950 2024-04-22 12:14:36.000000 trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keyword_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3484 2024-04-22 12:14:36.000000 trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keywords.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:00.000000 trytond_account_statement_rule-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-29 15:16:10.000000 trytond_account_statement_rule-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2139 2024-04-29 15:36:13.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-02-04 18:51:26.000000 trytond_account_statement_rule-7.2.0/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1031 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_information_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_information_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/statement_tree.xml
```

### Comparing `trytond_account_statement_rule-7.0.0/CHANGELOG` & `trytond_account_statement_rule-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_account_statement_rule-7.0.0/COPYRIGHT` & `trytond_account_statement_rule-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_statement_rule-7.0.0/LICENSE` & `trytond_account_statement_rule-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/PKG-INFO` & `trytond_account_statement_rule-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_rule
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to automate statement import with rules
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
@@ -47,23 +47,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_bank<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_bank<7.3,>=7.2; extra == "test"
 
 Account Statement Rule Module
 #############################
 
 The account_statement_rule module allows rules to be defined to complete
 statement lines from imported files.
 When the "Apply Rule" button is clicked on a statement, each rule is tested in
```

### Comparing `trytond_account_statement_rule-7.0.0/README.rst` & `trytond_account_statement_rule-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/__init__.py` & `trytond_account_statement_rule-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/account.py` & `trytond_account_statement_rule-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/account.xml` & `trytond_account_statement_rule-7.2.0/account.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account_statement_rule-7.0.0/account.xml` & `trytond_account_statement_rule-7.2.0/account.xml`

```diff
@@ -10,17 +10,17 @@
     </record>
     <record model="ir.ui.view" id="statement_view_tree">
       <field name="model">account.statement</field>
       <field name="inherit" ref="account_statement.statement_view_tree"/>
       <field name="name">statement_tree</field>
     </record>
     <record model="ir.model.button" id="statement_apply_rules_button">
+      <field name="model">account.statement</field>
       <field name="name">apply_rules</field>
       <field name="string">Apply Rules</field>
-      <field name="model" search="[('model', '=', 'account.statement')]"/>
     </record>
     <record model="ir.ui.view" id="rule_view_form">
       <field name="model">account.statement.rule</field>
       <field name="type">form</field>
       <field name="name">rule_form</field>
     </record>
     <record model="ir.ui.view" id="rule_view_list">
@@ -41,42 +41,42 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="rule_view_form"/>
       <field name="act_window" ref="act_rule_form"/>
     </record>
     <menuitem parent="account_statement.menu_statement_configuration" sequence="20" action="act_rule_form" id="menu_rule_form"/>
     <record model="ir.rule.group" id="rule_group_rule_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.statement.rule')]"/>
+      <field name="model">account.statement.rule</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_rule_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_rule_companies"/>
     </record>
     <record model="ir.rule" id="rule_rule_no_company">
       <field name="domain" eval="[('company', '=', None)]" pyson="1"/>
       <field name="rule_group" ref="rule_group_rule_companies"/>
     </record>
     <record model="ir.model.access" id="access_rule">
-      <field name="model" search="[('model', '=', 'account.statement.rule')]"/>
+      <field name="model">account.statement.rule</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_rule_account_admin">
-      <field name="model" search="[('model', '=', 'account.statement.rule')]"/>
+      <field name="model">account.statement.rule</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_rule_statement">
-      <field name="model" search="[('model', '=', 'account.statement.rule')]"/>
+      <field name="model">account.statement.rule</field>
       <field name="group" ref="account_statement.group_statement"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="rule_information_view_form">
```

### Comparing `trytond_account_statement_rule-7.0.0/doc/conf.py` & `trytond_account_statement_rule-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_statement_rule-7.0.0/doc/index.rst` & `trytond_account_statement_rule-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/bg.po` & `trytond_account_statement_rule-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/ca.po` & `trytond_account_statement_rule-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/cs.po` & `trytond_account_statement_rule-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/de.po` & `trytond_account_statement_rule-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/es.po` & `trytond_account_statement_rule-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/es_419.po` & `trytond_account_statement_rule-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/et.po` & `trytond_account_statement_rule-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/fa.po` & `trytond_account_statement_rule-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/fi.po` & `trytond_account_statement_rule-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/fr.po` & `trytond_account_statement_rule-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/hu.po` & `trytond_account_statement_rule-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/id.po` & `trytond_account_statement_rule-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/it.po` & `trytond_account_statement_rule-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/lo.po` & `trytond_account_statement_rule-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/lt.po` & `trytond_account_statement_rule-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/nl.po` & `trytond_account_statement_rule-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/pl.po` & `trytond_account_statement_rule-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/pt.po` & `trytond_account_statement_rule-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/ro.po` & `trytond_account_statement_rule-7.2.0/locale/uk.po`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,31 @@
 
 msgctxt "field:account.statement.rule,amount_low:"
 msgid "Amount Low"
 msgstr ""
 
 msgctxt "field:account.statement.rule,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.rule,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
 msgctxt "field:account.statement.rule,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:account.statement.rule,information_rules:"
 msgid "Information Rules"
 msgstr ""
 
 msgctxt "field:account.statement.rule,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr ""
 
 msgctxt "field:account.statement.rule,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:account.statement.rule,name:"
 msgid "Name"
@@ -89,27 +88,27 @@
 
 msgctxt "field:account.statement.rule.information,selection:"
 msgid "Selection"
 msgstr ""
 
 msgctxt "field:account.statement.rule.line,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:account.statement.rule.line,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.statement.rule.line,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.statement.rule.line,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.statement.rule.line,rule:"
 msgid "Rule"
 msgstr ""
 
 msgctxt "help:account.statement.rule,description:"
 msgid ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_statement_rule-7.0.0/locale/ru.po` & `trytond_account_statement_rule-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/sl.po` & `trytond_account_statement_rule-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/tr.po` & `trytond_account_statement_rule-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/locale/uk.po` & `trytond_account_statement_rule-7.2.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -163,21 +163,23 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.statement.rule.information:"
 msgid "-"
-msgstr ""
+msgstr "-"
 
+#, fuzzy
 msgctxt "view:account.statement.rule:"
 msgid "-"
-msgstr ""
+msgstr "-"
 
 msgctxt "view:account.statement.rule:"
 msgid "Between"
 msgstr ""
 
 msgctxt "view:account.statement.rule:"
 msgid "Criteria"
```

### Comparing `trytond_account_statement_rule-7.0.0/setup.py` & `trytond_account_statement_rule-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/tests/scenario_account_statement_rule.rst` & `trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Account Statement Rule Scenario
 ===============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_rule')
 
 Create company::
@@ -80,11 +80,9 @@
 Apply rules on statement::
 
     >>> statement.click('apply_rules')
     >>> len(statement.lines)
     2
     >>> sorted([l.amount for l in statement.lines])
     [Decimal('5.00'), Decimal('45.00')]
-    >>> {l.account for l in statement.lines} == {tax, receivable}
-    True
-    >>> {l.party for l in statement.lines}  == {None, customer}
-    True
+    >>> assertEqual({l.account for l in statement.lines}, {tax, receivable})
+    >>> assertEqual({l.party for l in statement.lines}, {None, customer})
```

### Comparing `trytond_account_statement_rule-7.0.0/tests/scenario_account_statement_rule_keyword_bank_account.rst` & `trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keyword_bank_account.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Account Statement Rule Keyword Bank Account Scenario
 ====================================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_statement_rule', 'bank'])
 
     >>> AccountJournal = Model.get('account.journal')
@@ -102,16 +103,15 @@
     >>> number.number = "123456"
     >>> bank_account.save()
 
 Apply rules on statement match::
 
     >>> statement.click('apply_rules')
     >>> line, = statement.lines
-    >>> line.party == customer
-    True
+    >>> assertEqual(line.party, customer)
 
     >>> statement.click('validate_statement')
     >>> statement.click('post')
 
 Remove the bank account::
 
     >>> bank_account.delete()
@@ -131,11 +131,9 @@
 
 Now a party is found::
 
     >>> statement.click('apply_rules')
     >>> line, = statement.lines
     >>> line.amount
     Decimal('50.00')
-    >>> line.party == customer
-    True
-    >>> line.account == accounts['receivable']
-    True
+    >>> assertEqual(line.party, customer)
+    >>> assertEqual(line.account, accounts['receivable'])
```

### Comparing `trytond_account_statement_rule-7.0.0/tests/scenario_account_statement_rule_keywords.rst` & `trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keywords.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Account Statement Rule Keyword Scenario
 =======================================
 
 Imports::
 
     >>> import datetime as dt
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
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_rule')
 
@@ -112,11 +112,9 @@
 
 Now a party is found::
 
     >>> statement.click('apply_rules')
     >>> line, = statement.lines
     >>> line.amount
     Decimal('50.00')
-    >>> line.party == customer
-    True
-    >>> line.account == receivable
-    True
+    >>> assertEqual(line.party, customer)
+    >>> assertEqual(line.account, receivable)
```

### Comparing `trytond_account_statement_rule-7.0.0/tox.ini` & `trytond_account_statement_rule-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/PKG-INFO` & `trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-statement-rule
-Version: 7.0.0
+Name: trytond_account_statement_rule
+Version: 7.2.0
 Summary: Tryton module to automate statement import with rules
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
@@ -47,23 +47,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_statement<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_statement<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_bank<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_bank<7.3,>=7.2; extra == "test"
 
 Account Statement Rule Module
 #############################
 
 The account_statement_rule module allows rules to be defined to complete
 statement lines from imported files.
 When the "Apply Rule" button is clicked on a statement, each rule is tested in
```

### Comparing `trytond_account_statement_rule-7.0.0/trytond_account_statement_rule.egg-info/SOURCES.txt` & `trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_statement_rule-7.0.0/view/rule_form.xml` & `trytond_account_statement_rule-7.2.0/view/rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.0.0/view/rule_information_form.xml` & `trytond_account_statement_rule-7.2.0/view/rule_information_form.xml`

 * *Files identical despite different names*

