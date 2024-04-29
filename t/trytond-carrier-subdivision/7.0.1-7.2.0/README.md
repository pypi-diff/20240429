# Comparing `tmp/trytond_carrier_subdivision-7.0.1.tar.gz` & `tmp/trytond_carrier_subdivision-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_subdivision-7.0.1.tar", last modified: Mon Jan  1 12:10:17 2024, max compression
+gzip compressed data, was "trytond_carrier_subdivision-7.2.0.tar", last modified: Mon Apr 29 15:38:54 2024, max compression
```

## Comparing `trytond_carrier_subdivision-7.0.1.tar` & `trytond_carrier_subdivision-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:10:17.982564 trytond_carrier_subdivision-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-01-01 12:10:15.000000 trytond_carrier_subdivision-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-01-01 12:10:15.000000 trytond_carrier_subdivision-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2552 2024-01-01 12:10:17.982564 trytond_carrier_subdivision-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3259 2023-12-27 10:43:58.000000 trytond_carrier_subdivision-7.0.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1086 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:10:17.979231 trytond_carrier_subdivision-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:10:17.979231 trytond_carrier_subdivision-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1795 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1816 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1790 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1860 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1795 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1908 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-01 12:10:17.982564 trytond_carrier_subdivision-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4700 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:10:17.979231 trytond_carrier_subdivision-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/tests/scenario_carrier_subdivision.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2840 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/tests/scenario_carrier_subdivision_postal_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2023-10-30 17:55:12.000000 trytond_carrier_subdivision-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:10:17.982564 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2552 2024-01-01 12:10:17.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1744 2024-01-01 12:10:17.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-01 12:10:17.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-01-01 12:10:17.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:45.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      142 2024-01-01 12:10:17.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-01 12:10:17.000000 trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:10:17.982564 trytond_carrier_subdivision-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/view/carrier_selection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-10-30 17:06:38.000000 trytond_carrier_subdivision-7.0.1/view/carrier_selection_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:54.731822 trytond_carrier_subdivision-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-29 15:18:35.000000 trytond_carrier_subdivision-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-04-29 15:18:35.000000 trytond_carrier_subdivision-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2552 2024-04-29 15:38:54.728489 trytond_carrier_subdivision-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3259 2024-04-22 12:14:36.000000 trytond_carrier_subdivision-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1086 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:54.725155 trytond_carrier_subdivision-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_carrier_subdivision-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:06.000000 trytond_carrier_subdivision-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:54.728489 trytond_carrier_subdivision-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1795 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1816 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1790 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1860 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1795 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:22.000000 trytond_carrier_subdivision-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1908 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:54.731822 trytond_carrier_subdivision-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4700 2024-03-17 11:01:36.000000 trytond_carrier_subdivision-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:54.728489 trytond_carrier_subdivision-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3764 2024-04-22 12:14:36.000000 trytond_carrier_subdivision-7.2.0/tests/scenario_carrier_subdivision.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2843 2024-04-22 12:14:36.000000 trytond_carrier_subdivision-7.2.0/tests/scenario_carrier_subdivision_postal_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:06.000000 trytond_carrier_subdivision-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-04-29 15:18:30.000000 trytond_carrier_subdivision-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:54.728489 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2552 2024-04-29 15:38:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-04-29 15:38:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:38:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      142 2024-04-29 15:38:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:54.000000 trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:54.728489 trytond_carrier_subdivision-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/view/carrier_selection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_carrier_subdivision-7.2.0/view/carrier_selection_list.xml
```

### Comparing `trytond_carrier_subdivision-7.0.1/CHANGELOG` & `trytond_carrier_subdivision-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-01-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_carrier_subdivision-7.0.1/COPYRIGHT` & `trytond_carrier_subdivision-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/LICENSE` & `trytond_carrier_subdivision-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/PKG-INFO` & `trytond_carrier_subdivision-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_subdivision
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module that allows carriers selection to be restrictedby subdivision
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
@@ -46,15 +46,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier_carriage<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier_carriage<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_carrier_subdivision-7.0.1/__init__.py` & `trytond_carrier_subdivision-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/carrier.py` & `trytond_carrier_subdivision-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/carrier.xml` & `trytond_carrier_subdivision-7.2.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/doc/conf.py` & `trytond_carrier_subdivision-7.2.0/doc/conf.py`

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

### Comparing `trytond_carrier_subdivision-7.0.1/locale/bg.po` & `trytond_carrier_subdivision-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/ca.po` & `trytond_carrier_subdivision-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/cs.po` & `trytond_carrier_subdivision-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/de.po` & `trytond_carrier_subdivision-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/es.po` & `trytond_carrier_subdivision-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/es_419.po` & `trytond_carrier_subdivision-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/et.po` & `trytond_carrier_subdivision-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/fa.po` & `trytond_carrier_subdivision-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/fi.po` & `trytond_carrier_subdivision-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/fr.po` & `trytond_carrier_subdivision-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/hu.po` & `trytond_carrier_subdivision-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/id.po` & `trytond_carrier_subdivision-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/it.po` & `trytond_carrier_subdivision-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/lo.po` & `trytond_carrier_subdivision-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/lt.po` & `trytond_carrier_subdivision-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/nl.po` & `trytond_carrier_subdivision-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/pl.po` & `trytond_carrier_subdivision-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/pt.po` & `trytond_carrier_subdivision-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/ro.po` & `trytond_carrier_subdivision-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/ru.po` & `trytond_carrier_subdivision-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/sl.po` & `trytond_carrier_subdivision-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/tr.po` & `trytond_carrier_subdivision-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/uk.po` & `trytond_carrier_subdivision-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/locale/zh_CN.po` & `trytond_carrier_subdivision-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/sale.py` & `trytond_carrier_subdivision-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/setup.py` & `trytond_carrier_subdivision-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/tests/scenario_carrier_subdivision.rst` & `trytond_carrier_subdivision-7.2.0/tests/scenario_carrier_subdivision.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ============================
 Carrier Subdivision Scenario
 ============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['carrier_subdivision', 'sale_shipment_cost'])
 
 Create company::
 
@@ -115,13 +115,11 @@
     >>> csc.save()
 
 Test right carrier is used on sale::
 
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
     >>> sale.party = customer
-    >>> sale.carrier == carrier
-    True
+    >>> assertEqual(sale.carrier, carrier)
     >>> sale.carrier = None
     >>> sale.party = other_customer
-    >>> sale.carrier == catalan_carrier
-    True
+    >>> assertEqual(sale.carrier, catalan_carrier)
```

### Comparing `trytond_carrier_subdivision-7.0.1/tests/scenario_carrier_subdivision_postal_code.rst` & `trytond_carrier_subdivision-7.2.0/tests/scenario_carrier_subdivision_postal_code.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ========================================
 Carrier Subdivision Postal Code Scenario
 ========================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['carrier_subdivision', 'sale_shipment_cost'])
 
 Create company::
 
@@ -85,13 +85,11 @@
     >>> csc.save()
 
 Test right carrier is used on sale::
 
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
     >>> sale.party = customer
-    >>> sale.carrier == carrier
-    True
+    >>> assertEqual(sale.carrier, carrier)
     >>> sale.carrier = None
     >>> sale.party = other_customer
-    >>> sale.carrier == local_carrier
-    True
+    >>> assertEqual(sale.carrier, local_carrier)
```

### Comparing `trytond_carrier_subdivision-7.0.1/tox.ini` & `trytond_carrier_subdivision-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/PKG-INFO` & `trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-carrier-subdivision
-Version: 7.0.1
+Name: trytond_carrier_subdivision
+Version: 7.2.0
 Summary: Tryton module that allows carriers selection to be restrictedby subdivision
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
@@ -46,15 +46,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier_carriage<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier_carriage<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_carrier_subdivision-7.0.1/trytond_carrier_subdivision.egg-info/SOURCES.txt` & `trytond_carrier_subdivision-7.2.0/trytond_carrier_subdivision.egg-info/SOURCES.txt`

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
 carrier.py
```

### Comparing `trytond_carrier_subdivision-7.0.1/view/carrier_selection_form.xml` & `trytond_carrier_subdivision-7.2.0/view/carrier_selection_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_subdivision-7.0.1/view/carrier_selection_list.xml` & `trytond_carrier_subdivision-7.2.0/view/carrier_selection_list.xml`

 * *Files identical despite different names*

