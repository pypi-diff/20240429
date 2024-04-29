# Comparing `tmp/trytond_account_invoice_defer-7.0.0.tar.gz` & `tmp/trytond_account_invoice_defer-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_defer-7.0.0.tar", last modified: Mon Oct 30 17:20:59 2023, max compression
+gzip compressed data, was "trytond_account_invoice_defer-7.2.0.tar", last modified: Mon Apr 29 15:33:48 2024, max compression
```

## Comparing `trytond_account_invoice_defer-7.0.0.tar` & `trytond_account_invoice_defer-7.2.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:59.006232 trytond_account_invoice_defer-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:22:51.000000 trytond_account_invoice_defer-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-10-30 17:01:59.000000 trytond_account_invoice_defer-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:01:59.000000 trytond_account_invoice_defer-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2758 2023-10-30 17:20:59.006232 trytond_account_invoice_defer-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18660 2023-10-27 17:38:49.000000 trytond_account_invoice_defer-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8380 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:59.002899 trytond_account_invoice_defer-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:22:51.000000 trytond_account_invoice_defer-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1844 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:51.000000 trytond_account_invoice_defer-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:58.999565 trytond_account_invoice_defer-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5844 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5849 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5961 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4801 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5896 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-10-28 12:11:19.000000 trytond_account_invoice_defer-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:20:59.006232 trytond_account_invoice_defer-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4660 2023-10-27 17:38:49.000000 trytond_account_invoice_defer-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:59.002899 trytond_account_invoice_defer-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-10-07 15:40:36.000000 trytond_account_invoice_defer-7.0.0/tests/scenario_account_invoice_defer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-06-10 11:39:56.000000 trytond_account_invoice_defer-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_invoice_defer-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-10-30 17:01:56.000000 trytond_account_invoice_defer-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:59.002899 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2758 2023-10-30 17:20:58.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1854 2023-10-30 17:20:58.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:20:58.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:20:58.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-10-30 17:20:58.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:20:58.000000 trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:20:59.002899 trytond_account_invoice_defer-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-10-07 15:40:36.000000 trytond_account_invoice_defer-7.0.0/view/invoice_deferred_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/view/invoice_deferred_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.0.0/view/invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-29 15:14:26.000000 trytond_account_invoice_defer-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:14:25.000000 trytond_account_invoice_defer-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18660 2024-03-17 11:01:36.000000 trytond_account_invoice_defer-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-04-27 16:30:39.000000 trytond_account_invoice_defer-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.969819 trytond_account_invoice_defer-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_account_invoice_defer-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1844 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:55.000000 trytond_account_invoice_defer-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5844 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6073 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5849 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4801 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5896 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4856 2024-04-29 13:17:17.000000 trytond_account_invoice_defer-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4651 2024-04-27 16:30:39.000000 trytond_account_invoice_defer-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3862 2024-04-22 12:14:36.000000 trytond_account_invoice_defer-7.2.0/tests/scenario_account_invoice_defer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-01-27 09:58:52.000000 trytond_account_invoice_defer-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:55.000000 trytond_account_invoice_defer-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-29 15:14:20.000000 trytond_account_invoice_defer-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1836 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2024-02-04 18:51:26.000000 trytond_account_invoice_defer-7.2.0/view/invoice_deferred_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/view/invoice_deferred_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/view/invoice_line_form.xml
```

### Comparing `trytond_account_invoice_defer-7.0.0/CHANGELOG` & `trytond_account_invoice_defer-7.2.0/CHANGELOG`

 * *Files 25% similar despite different names*

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

### Comparing `trytond_account_invoice_defer-7.0.0/COPYRIGHT` & `trytond_account_invoice_defer-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_defer-7.0.0/LICENSE` & `trytond_account_invoice_defer-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/PKG-INFO` & `trytond_account_invoice_defer-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_defer
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-defer
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice-defer
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice defer expense revenue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ############################
 Account Invoice Defer Module
 ############################
 
 The *Account Invoice Defer Module* allow to defer the expense or the revenue of
 an invoice line over many periods.
```

### Comparing `trytond_account_invoice_defer-7.0.0/__init__.py` & `trytond_account_invoice_defer-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/account.py` & `trytond_account_invoice_defer-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/account.xml` & `trytond_account_invoice_defer-7.2.0/account.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_invoice_defer-7.0.0/account.xml` & `trytond_account_invoice_defer-7.2.0/account.xml`

```diff
@@ -87,43 +87,43 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain" eval="[]" pyson="1"/>
       <field name="act_window" ref="act_invoice_deferred_in_form"/>
     </record>
     <menuitem parent="account_invoice.menu_invoices" action="act_invoice_deferred_in_form" sequence="50" id="menu_invoice_deferred_in_form"/>
     <record model="ir.model.access" id="access_invoice_deferred">
-      <field name="model" search="[('model', '=', 'account.invoice.deferred')]"/>
+      <field name="model">account.invoice.deferred</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_deferred_account">
-      <field name="model" search="[('model', '=', 'account.invoice.deferred')]"/>
+      <field name="model">account.invoice.deferred</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_invoice_deferred_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.invoice.deferred')]"/>
+      <field name="model">account.invoice.deferred</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_invoice_deferred_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_invoice_deferred_companies"/>
     </record>
     <record model="ir.model.button" id="invoice_deferred_run_button">
+      <field name="model">account.invoice.deferred</field>
       <field name="name">run</field>
       <field name="string">Run</field>
       <field name="confirm">Are you sure you want to defer the invoices?</field>
       <field name="help">Start deferring the invoice</field>
-      <field name="model" search="[('model', '=', 'account.invoice.deferred')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_invoice_deferred_create_moves">
       <field name="name">Create Invoices Deferred Moves</field>
       <field name="wiz_name">account.invoice.deferred.create_moves</field>
     </record>
     <menuitem parent="account_invoice.menu_invoices" sequence="90" action="wizard_invoice_deferred_create_moves" id="menu_invoice_deferred_create_moves"/>
     <record model="ir.action-res.group" id="wizard_invoice_deferred_create_moves-group_account">
```

### Comparing `trytond_account_invoice_defer-7.0.0/doc/conf.py` & `trytond_account_invoice_defer-7.2.0/doc/conf.py`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_invoice_defer-7.0.0/doc/design.rst` & `trytond_account_invoice_defer-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/bg.po` & `trytond_account_invoice_defer-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/ca.po` & `trytond_account_invoice_defer-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/cs.po` & `trytond_account_invoice_defer-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/de.po` & `trytond_account_invoice_defer-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/es.po` & `trytond_account_invoice_defer-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/es_419.po` & `trytond_account_invoice_defer-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/et.po` & `trytond_account_invoice_defer-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/fa.po` & `trytond_account_invoice_defer-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/fi.po` & `trytond_account_invoice_defer-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/fr.po` & `trytond_account_invoice_defer-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/hu.po` & `trytond_account_invoice_defer-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/id.po` & `trytond_account_invoice_defer-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/it.po` & `trytond_account_invoice_defer-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/lo.po` & `trytond_account_invoice_defer-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/lt.po` & `trytond_account_invoice_defer-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/nl.po` & `trytond_account_invoice_defer-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/pl.po` & `trytond_account_invoice_defer-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/pt.po` & `trytond_account_invoice_defer-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/ro.po` & `trytond_account_invoice_defer-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/ru.po` & `trytond_account_invoice_defer-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/sl.po` & `trytond_account_invoice_defer-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/tr.po` & `trytond_account_invoice_defer-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/uk.po` & `trytond_account_invoice_defer-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/locale/zh_CN.po` & `trytond_account_invoice_defer-7.2.0/locale/ro.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #
+#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,deferred_account_expense:"
 msgid "Deferred Account Expense"
 msgstr ""
 
@@ -18,51 +19,51 @@
 msgctxt ""
 "field:account.configuration.default_account,deferred_account_revenue:"
 msgid "Deferred Account Revenue"
 msgstr ""
 
 msgctxt "field:account.invoice.deferred,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:account.invoice.deferred,company:"
 msgid "Company"
-msgstr ""
+msgstr "Compania"
 
 msgctxt "field:account.invoice.deferred,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:account.invoice.deferred,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data Sfarsit"
 
 msgctxt "field:account.invoice.deferred,invoice_line:"
 msgid "Invoice Line"
 msgstr ""
 
 msgctxt "field:account.invoice.deferred,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.invoice.deferred,moves:"
 msgid "Moves"
-msgstr ""
+msgstr "Miscari"
 
 msgctxt "field:account.invoice.deferred,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data Inceput"
 
 msgctxt "field:account.invoice.deferred,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.invoice.deferred,type:"
 msgid "Type"
-msgstr ""
+msgstr "Tip"
 
 msgctxt "field:account.invoice.line,defer_from:"
 msgid "Defer From"
 msgstr ""
 
 msgctxt "field:account.invoice.line,defer_to:"
 msgid "Defer To"
@@ -92,30 +93,30 @@
 "model:ir.action.act_window.domain,name:act_invoice_deferred_in_form_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_deferred_in_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Ciorna"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_deferred_in_form_domain_running"
 msgid "Running"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_deferred_out_form_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_deferred_out_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Ciorna"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_deferred_out_form_domain_running"
 msgid "Running"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_defer_invoice_line_unique"
```

### Comparing `trytond_account_invoice_defer-7.0.0/message.xml` & `trytond_account_invoice_defer-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/setup.py` & `trytond_account_invoice_defer-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-invoice-defer'),
+            'https://docs.tryton.org/modules-account-invoice-defer'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice defer expense revenue',
     package_dir={'trytond.modules.account_invoice_defer': '.'},
     packages=(
         ['trytond.modules.account_invoice_defer']
```

### Comparing `trytond_account_invoice_defer-7.0.0/tests/scenario_account_invoice_defer.rst` & `trytond_account_invoice_defer-7.2.0/tests/scenario_account_invoice_defer.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
     >>> from trytond.modules.account_invoice_defer.tests.tools import (
     ...     add_deferred_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice_defer')
 
@@ -86,22 +85,19 @@
     >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> invoice_line, = invoice.lines
 
 Check invoice deferred and run it::
 
     >>> deferral, = InvoiceDeferred.find([])
-    >>> deferral.invoice_line == invoice_line
-    True
+    >>> assertEqual(deferral.invoice_line, invoice_line)
     >>> deferral.amount
     Decimal('1000.00')
-    >>> deferral.start_date == invoice_line.defer_from
-    True
-    >>> deferral.end_date == invoice_line.defer_to
-    True
+    >>> assertEqual(deferral.start_date, invoice_line.defer_from)
+    >>> assertEqual(deferral.end_date, invoice_line.defer_to)
     >>> deferral.click('run')
 
 Check moves on invoice deferred::
 
     >>> deferral.reload()
     >>> deferral.state
     'running'
```

### Comparing `trytond_account_invoice_defer-7.0.0/tests/tools.py` & `trytond_account_invoice_defer-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/tox.ini` & `trytond_account_invoice_defer-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/PKG-INFO` & `trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice-defer
-Version: 7.0.0
+Name: trytond_account_invoice_defer
+Version: 7.2.0
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-defer
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice-defer
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice defer expense revenue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ############################
 Account Invoice Defer Module
 ############################
 
 The *Account Invoice Defer Module* allow to defer the expense or the revenue of
 an invoice line over many periods.
```

### Comparing `trytond_account_invoice_defer-7.0.0/trytond_account_invoice_defer.egg-info/SOURCES.txt` & `trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_account_invoice_defer-7.0.0/view/invoice_deferred_form.xml` & `trytond_account_invoice_defer-7.2.0/view/invoice_deferred_form.xml`

 * *Files identical despite different names*

