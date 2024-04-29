# Comparing `tmp/trytond_sale_extra-7.0.1.tar.gz` & `tmp/trytond_sale_extra-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_extra-7.0.1.tar", last modified: Wed Apr 17 10:36:47 2024, max compression
+gzip compressed data, was "trytond_sale_extra-7.2.0.tar", last modified: Mon Apr 29 15:47:49 2024, max compression
```

## Comparing `trytond_sale_extra-7.0.1.tar` & `trytond_sale_extra-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1827 2024-04-17 10:36:44.000000 trytond_sale_extra-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-17 10:36:44.000000 trytond_sale_extra-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3757 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.251603 trytond_sale_extra-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2789 2024-03-03 16:24:20.000000 trytond_sale_extra-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.251603 trytond_sale_extra-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2189 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1976 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1765 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2008 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2151 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1840 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1921 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1979 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2028 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1972 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7969 2024-04-12 22:42:09.000000 trytond_sale_extra-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4683 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4397 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.251603 trytond_sale_extra-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4733 2024-02-05 16:24:27.000000 trytond_sale_extra-7.0.1/tests/scenario_sale_extra.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-02-05 16:24:27.000000 trytond_sale_extra-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3757 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-17 10:36:47.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:06.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:36:46.000000 trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:36:47.254936 trytond_sale_extra-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-10-30 17:06:38.000000 trytond_sale_extra-7.0.1/view/extra_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:49.994489 trytond_sale_extra-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1827 2024-04-29 15:25:07.000000 trytond_sale_extra-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:25:07.000000 trytond_sale_extra-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_extra-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3757 2024-04-29 15:47:49.994489 trytond_sale_extra-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-01-16 14:00:21.000000 trytond_sale_extra-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:49.991156 trytond_sale_extra-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_sale_extra-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-01-16 14:00:21.000000 trytond_sale_extra-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:25.000000 trytond_sale_extra-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:49.991156 trytond_sale_extra-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2189 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1976 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1970 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1765 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2008 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2151 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1840 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1921 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1970 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1979 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2028 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1987 2024-04-29 13:17:17.000000 trytond_sale_extra-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2199 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1972 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1808 2024-04-27 16:43:26.000000 trytond_sale_extra-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7969 2024-04-27 16:30:39.000000 trytond_sale_extra-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4614 2024-04-27 16:30:39.000000 trytond_sale_extra-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:49.994489 trytond_sale_extra-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4397 2024-03-17 11:01:36.000000 trytond_sale_extra-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:49.991156 trytond_sale_extra-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4684 2024-04-22 12:14:36.000000 trytond_sale_extra-7.2.0/tests/scenario_sale_extra.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:25.000000 trytond_sale_extra-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-04-29 15:25:02.000000 trytond_sale_extra-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:49.994489 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3757 2024-04-29 15:47:49.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-29 15:47:49.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:49.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:47:49.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-29 15:47:49.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:49.000000 trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:49.994489 trytond_sale_extra-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:21.000000 trytond_sale_extra-7.2.0/view/extra_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-01-16 14:00:21.000000 trytond_sale_extra-7.2.0/view/extra_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/view/extra_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/view/extra_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_sale_extra-7.2.0/view/extra_list.xml
```

### Comparing `trytond_sale_extra-7.0.1/CHANGELOG` & `trytond_sale_extra-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-04-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_extra-7.0.1/COPYRIGHT` & `trytond_sale_extra-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/LICENSE` & `trytond_sale_extra-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/PKG-INFO` & `trytond_sale_extra-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_extra
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for sale extra
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
@@ -49,22 +49,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Extra
 ##########
 
 The sale_extra module allows to add extra line on sale based on criteria.
 
 The extra products are added when the sale goes into quotation but the added
```

### Comparing `trytond_sale_extra-7.0.1/README.rst` & `trytond_sale_extra-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/doc/conf.py` & `trytond_sale_extra-7.2.0/doc/conf.py`

 * *Files 6% similar despite different names*

```diff
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

### Comparing `trytond_sale_extra-7.0.1/doc/index.rst` & `trytond_sale_extra-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/bg.po` & `trytond_sale_extra-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/ca.po` & `trytond_sale_extra-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/cs.po` & `trytond_sale_extra-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/de.po` & `trytond_sale_extra-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/es.po` & `trytond_sale_extra-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/es_419.po` & `trytond_sale_extra-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/et.po` & `trytond_sale_extra-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/fa.po` & `trytond_sale_extra-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/fi.po` & `trytond_sale_extra-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/fr.po` & `trytond_sale_extra-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/hu.po` & `trytond_sale_extra-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/id.po` & `trytond_sale_extra-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/it.po` & `trytond_sale_extra-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/lo.po` & `trytond_sale_extra-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/lt.po` & `trytond_sale_extra-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/nl.po` & `trytond_sale_extra-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/pl.po` & `trytond_sale_extra-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/pt.po` & `trytond_sale_extra-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/ro.po` & `trytond_sale_extra-7.2.0/locale/tr.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.extra,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.extra,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
 msgctxt "field:sale.extra,end_date:"
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:sale.extra,lines:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "field:sale.extra,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:sale.extra,price_list:"
 msgid "Price List"
-msgstr "Listă de prețuri"
+msgstr ""
 
 msgctxt "field:sale.extra,sale_amount:"
 msgid "Sale Amount"
 msgstr ""
 
 msgctxt "field:sale.extra,start_date:"
 msgid "Start Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.extra.line,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.extra.line,extra:"
 msgid "Extra"
-msgstr ""
+msgstr "Extras"
 
 msgctxt "field:sale.extra.line,free:"
 msgid "Free"
 msgstr ""
 
 msgctxt "field:sale.extra.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:sale.extra.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
 msgctxt "field:sale.extra.line,quantity:"
 msgid "Quantity"
@@ -64,37 +63,39 @@
 msgid "Sale Amount"
 msgstr ""
 
 msgctxt "field:sale.extra.line,unit:"
 msgid "Unit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.line,extra:"
 msgid "Extra"
-msgstr ""
+msgstr "Extras"
 
 msgctxt "model:ir.action,name:act_extra_form"
 msgid "Extras"
-msgstr ""
+msgstr "Extras"
 
 msgctxt "model:ir.action,name:act_extra_relate"
 msgid "Sale Extras"
-msgstr ""
+msgstr "Sale Extras"
 
 msgctxt "model:ir.rule.group,name:rule_group_extra_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_extra"
 msgid "Extras"
-msgstr ""
+msgstr "Extras"
 
+#, fuzzy
 msgctxt "model:sale.extra,name:"
 msgid "Sale Extra"
-msgstr ""
+msgstr "Sale Extras"
 
 msgctxt "model:sale.extra.line,name:"
 msgid "Sale Extra Line"
 msgstr ""
 
 msgctxt "view:sale.extra.line:"
 msgid "Sale Line"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_extra-7.0.1/locale/ru.po` & `trytond_sale_extra-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/sl.po` & `trytond_sale_extra-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/tr.po` & `trytond_sale_extra-7.2.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:sale.extra,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.extra,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
 msgctxt "field:sale.extra,price_list:"
 msgid "Price List"
 msgstr ""
 
 msgctxt "field:sale.extra,sale_amount:"
 msgid "Sale Amount"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_extra-7.0.1/locale/uk.po` & `trytond_sale_extra-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/locale/zh_CN.po` & `trytond_sale_extra-7.2.0/locale/ro.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,102 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.extra,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:sale.extra,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:sale.extra,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data de sfârşit"
 
 msgctxt "field:sale.extra,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
-#, fuzzy
 msgctxt "field:sale.extra,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nume"
 
 msgctxt "field:sale.extra,price_list:"
 msgid "Price List"
-msgstr ""
+msgstr "Listă de prețuri"
 
 msgctxt "field:sale.extra,sale_amount:"
 msgid "Sale Amount"
-msgstr ""
+msgstr "Valoarea vânzării"
 
 msgctxt "field:sale.extra,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data de Început"
 
 msgctxt "field:sale.extra.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 #, fuzzy
 msgctxt "field:sale.extra.line,extra:"
 msgid "Extra"
-msgstr "Extras"
+msgstr "Suplimentar"
 
 msgctxt "field:sale.extra.line,free:"
 msgid "Free"
-msgstr ""
+msgstr "Gratuit"
 
 msgctxt "field:sale.extra.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:sale.extra.line,product_uom_category:"
 msgid "Product UoM Category"
-msgstr ""
+msgstr "Categorie UM Produs"
 
 msgctxt "field:sale.extra.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:sale.extra.line,sale_amount:"
 msgid "Sale Amount"
-msgstr ""
+msgstr "Valoarea vânzării"
 
 msgctxt "field:sale.extra.line,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 #, fuzzy
 msgctxt "field:sale.line,extra:"
 msgid "Extra"
-msgstr "Extras"
+msgstr "Suplimentar"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_extra_form"
 msgid "Extras"
-msgstr "Extras"
+msgstr "In plus"
 
 msgctxt "model:ir.action,name:act_extra_relate"
 msgid "Sale Extras"
-msgstr "Sale Extras"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_extra_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.ui.menu,name:menu_extra"
 msgid "Extras"
-msgstr "Extras"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:sale.extra,name:"
 msgid "Sale Extra"
-msgstr "Sale Extras"
+msgstr ""
 
 msgctxt "model:sale.extra.line,name:"
 msgid "Sale Extra Line"
 msgstr ""
 
 msgctxt "view:sale.extra.line:"
 msgid "Sale Line"
-msgstr ""
+msgstr "Rând de vânzare"
```

### Comparing `trytond_sale_extra-7.0.1/sale.py` & `trytond_sale_extra-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/sale.xml` & `trytond_sale_extra-7.2.0/sale.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_sale_extra-7.0.1/sale.xml` & `trytond_sale_extra-7.2.0/sale.xml`

```diff
@@ -39,30 +39,30 @@
     <record model="ir.action.keyword" id="act_extra_relate_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">product.price_list,-1</field>
       <field name="action" ref="act_extra_relate"/>
     </record>
     <record model="ir.rule.group" id="rule_group_extra_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.extra')]"/>
+      <field name="model">sale.extra</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_extra_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_extra_companies"/>
     </record>
     <record model="ir.model.access" id="access_extra">
-      <field name="model" search="[('model', '=', 'sale.extra')]"/>
+      <field name="model">sale.extra</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_extra_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.extra')]"/>
+      <field name="model">sale.extra</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="extra_line_view_form">
```

### Comparing `trytond_sale_extra-7.0.1/setup.py` & `trytond_sale_extra-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/tests/scenario_sale_extra.rst` & `trytond_sale_extra-7.2.0/tests/scenario_sale_extra.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 Sale Extra Scenario
 ===================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_extra')
 
 Create company::
```

### Comparing `trytond_sale_extra-7.0.1/tox.ini` & `trytond_sale_extra-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/PKG-INFO` & `trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_extra
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for sale extra
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
@@ -49,22 +49,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Extra
 ##########
 
 The sale_extra module allows to add extra line on sale based on criteria.
 
 The extra products are added when the sale goes into quotation but the added
```

### Comparing `trytond_sale_extra-7.0.1/trytond_sale_extra.egg-info/SOURCES.txt` & `trytond_sale_extra-7.2.0/trytond_sale_extra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/view/extra_form.xml` & `trytond_sale_extra-7.2.0/view/extra_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-7.0.1/view/extra_line_form.xml` & `trytond_sale_extra-7.2.0/view/extra_line_form.xml`

 * *Files identical despite different names*

