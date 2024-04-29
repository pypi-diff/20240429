# Comparing `tmp/trytond_sale_amendment-7.0.1.tar.gz` & `tmp/trytond_sale_amendment-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_amendment-7.0.1.tar", last modified: Sun Mar  3 12:20:10 2024, max compression
+gzip compressed data, was "trytond_sale_amendment-7.2.0.tar", last modified: Mon Apr 29 15:47:18 2024, max compression
```

## Comparing `trytond_sale_amendment-7.0.1.tar` & `trytond_sale_amendment-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1068 2024-03-03 12:20:07.000000 trytond_sale_amendment-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-03-03 12:20:07.000000 trytond_sale_amendment-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:20:10.288116 trytond_sale_amendment-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2024-02-05 16:24:27.000000 trytond_sale_amendment-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4347 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4360 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4382 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4398 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3870 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4378 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4358 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3753 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16693 2024-02-29 11:47:34.000000 trytond_sale_amendment-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5880 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4510 2024-02-05 16:24:27.000000 trytond_sale_amendment-7.0.1/tests/scenario_sale_amendment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      129 2024-02-05 16:24:27.000000 trytond_sale_amendment-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-03-03 12:20:09.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1789 2024-03-03 12:20:10.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:20:09.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-03-03 12:20:09.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-03-03 12:20:09.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:20:09.000000 trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:20:10.291450 trytond_sale_amendment-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      621 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/view/sale_amendment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1305 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/view/sale_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/view/sale_amendment_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/view/sale_amendment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:38.000000 trytond_sale_amendment-7.0.1/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1068 2024-04-29 15:24:42.000000 trytond_sale_amendment-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:24:41.000000 trytond_sale_amendment-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.401982 trytond_sale_amendment-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_amendment-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_sale_amendment-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4347 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4360 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4382 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4398 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3870 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4395 2024-04-29 13:17:17.000000 trytond_sale_amendment-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4358 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4334 2024-04-29 13:17:17.000000 trytond_sale_amendment-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16693 2024-04-27 16:30:39.000000 trytond_sale_amendment-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5788 2024-04-27 16:30:39.000000 trytond_sale_amendment-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2024-03-17 11:01:36.000000 trytond_sale_amendment-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4516 2024-04-22 12:14:36.000000 trytond_sale_amendment-7.2.0/tests/scenario_sale_amendment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_sale_amendment-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      129 2024-04-29 15:24:37.000000 trytond_sale_amendment-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1771 2024-04-29 15:47:18.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      621 2024-01-27 09:58:52.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1305 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_form.xml
```

### Comparing `trytond_sale_amendment-7.0.1/CHANGELOG` & `trytond_sale_amendment-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-03-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_amendment-7.0.1/COPYRIGHT` & `trytond_sale_amendment-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/LICENSE` & `trytond_sale_amendment-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/PKG-INFO` & `trytond_sale_amendment-7.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_amendment
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to amend sales
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
@@ -47,21 +47,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_history<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_history<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Amendment Module
 #####################
 
 The sale amendment module allows you to change sales that are being processed
 and keep track of the changes.
 An amendment is composed of action lines which can:
```

### Comparing `trytond_sale_amendment-7.0.1/README.rst` & `trytond_sale_amendment-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/doc/conf.py` & `trytond_sale_amendment-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_sale_amendment-7.0.1/doc/index.rst` & `trytond_sale_amendment-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/bg.po` & `trytond_sale_amendment-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/ca.po` & `trytond_sale_amendment-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/cs.po` & `trytond_sale_amendment-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/de.po` & `trytond_sale_amendment-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/es.po` & `trytond_sale_amendment-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/es_419.po` & `trytond_sale_amendment-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/et.po` & `trytond_sale_amendment-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/fa.po` & `trytond_sale_amendment-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/fi.po` & `trytond_sale_amendment-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/fr.po` & `trytond_sale_amendment-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/hu.po` & `trytond_sale_amendment-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/id.po` & `trytond_sale_amendment-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/it.po` & `trytond_sale_amendment-7.2.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Verifica"
 
 msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utente in aziende"
 
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Correzioni"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
```

### Comparing `trytond_sale_amendment-7.0.1/locale/lo.po` & `trytond_sale_amendment-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/lt.po` & `trytond_sale_amendment-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/nl.po` & `trytond_sale_amendment-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/pl.po` & `trytond_sale_amendment-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/pt.po` & `trytond_sale_amendment-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/ro.po` & `trytond_sale_amendment-7.2.0/locale/ru.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.amendment,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:sale.amendment,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.amendment,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:sale.amendment,sale:"
 msgid "Sale"
@@ -20,23 +20,23 @@
 
 msgctxt "field:sale.amendment,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,action:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,amendment:"
 msgid "Amendment"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,invoice_party:"
 msgid "Invoice Party"
@@ -44,23 +44,23 @@
 
 msgctxt "field:sale.amendment.line,line:"
 msgid "Line"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,payment_term:"
 msgid "Payment Term"
-msgstr "Termen de plata"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,quantity:"
 msgid "Quantity"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_amendment-7.0.1/locale/ru.po` & `trytond_sale_amendment-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/sl.po` & `trytond_sale_amendment-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/tr.po` & `trytond_sale_amendment-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/locale/uk.po` & `trytond_sale_amendment-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/sale.py` & `trytond_sale_amendment-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/sale.xml` & `trytond_sale_amendment-7.2.0/sale.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_sale_amendment-7.0.1/sale.xml` & `trytond_sale_amendment-7.2.0/sale.xml`

```diff
@@ -56,42 +56,42 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_sale_amendment_form"/>
     </record>
     <menuitem parent="sale.menu_sale" action="act_sale_amendment_form" sequence="40" id="menu_sale_amendment"/>
     <record model="ir.model.access" id="access_sale_amendment">
-      <field name="model" search="[('model', '=', 'sale.amendment')]"/>
+      <field name="model">sale.amendment</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_sale_amendment_sale">
-      <field name="model" search="[('model', '=', 'sale.amendment')]"/>
+      <field name="model">sale.amendment</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sale_amendment_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.amendment')]"/>
+      <field name="model">sale.amendment</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sale_amendment_companies">
       <field name="domain" eval="[('sale.company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sale_amendment_companies"/>
     </record>
     <record model="ir.model.button" id="sale_amendment_validation_amendment_button">
+      <field name="model">sale.amendment</field>
       <field name="name">validate_amendment</field>
       <field name="string">Validate</field>
       <field name="confirm">Are you sure you want to validate the amendments?</field>
-      <field name="model" search="[('model', '=', 'sale.amendment')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_amendment_validation_amendment_button_group_sale_amendment">
       <field name="button" ref="sale_amendment_validation_amendment_button"/>
       <field name="group" ref="group_sale_amendment"/>
     </record>
     <record model="ir.ui.view" id="sale_amendment_line_view_list">
       <field name="model">sale.amendment.line</field>
```

### Comparing `trytond_sale_amendment-7.0.1/setup.py` & `trytond_sale_amendment-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/tests/scenario_sale_amendment.rst` & `trytond_sale_amendment-7.2.0/tests/scenario_sale_amendment.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =======================
 Sale Amendment Scenario
 =======================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
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
 
 Activate modules::
 
     >>> config = activate_modules('sale_amendment')
 
 Create company::
 
@@ -97,26 +97,24 @@
     >>> amendment = sale.amendments.new()
     >>> line = amendment.lines.new()
     >>> line.action = 'taxes'
     >>> line = amendment.lines.new()
     >>> line.action = 'payment_term'
     >>> line = amendment.lines.new()
     >>> line.action = 'party'
-    >>> line.party == customer1
-    True
+    >>> assertEqual(line.party, customer1)
     >>> line.party = customer2
     >>> line = amendment.lines.new()
     >>> line.action = 'warehouse'
     >>> bool(line.warehouse)
     True
     >>> line = amendment.lines.new()
     >>> line.action = 'line'
     >>> line.line = sale.lines[0]
-    >>> line.product == product1
-    True
+    >>> assertEqual(line.product, product1)
     >>> line.product = product2
     >>> line.quantity
     5.0
     >>> line.quantity = 4.0
     >>> line.unit_price
     Decimal('10.0000')
     >>> line.unit_price = Decimal('9.0000')
@@ -129,40 +127,36 @@
 
 Validate amendment::
 
     >>> amendment.click('validate_amendment')
     >>> sale.reload()
     >>> sale.revision
     1
-    >>> sale.party == customer2
-    True
+    >>> assertEqual(sale.party, customer2)
     >>> line = sale.lines[0]
-    >>> line.product == product2
-    True
+    >>> assertEqual(line.product, product2)
     >>> line.quantity
     4.0
     >>> line.unit_price
     Decimal('9.0000')
     >>> line = sale.lines[1]
     >>> line.quantity
     2.0
     >>> sale.total_amount
     Decimal('46.00')
 
     >>> shipment, = sale.shipments
     >>> move, = shipment.outgoing_moves
-    >>> move.product == product2
-    True
+    >>> assertEqual(move.product, product2)
     >>> move.quantity
     4.0
 
     >>> invoice, = sale.invoices
     >>> line = invoice.lines[0]
-    >>> line.product == product2
-    True
+    >>> assertEqual(line.product, product2)
     >>> line.quantity
     4.0
     >>> line.unit_price
     Decimal('9.0000')
     >>> line = invoice.lines[1]
     >>> line.product
     >>> line.quantity
```

### Comparing `trytond_sale_amendment-7.0.1/tox.ini` & `trytond_sale_amendment-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/PKG-INFO` & `trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_amendment
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to amend sales
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
@@ -47,21 +47,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_history<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_history<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Amendment Module
 #####################
 
 The sale amendment module allows you to change sales that are being processed
 and keep track of the changes.
 An amendment is composed of action lines which can:
```

### Comparing `trytond_sale_amendment-7.0.1/trytond_sale_amendment.egg-info/SOURCES.txt` & `trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_sale_amendment-7.0.1/view/sale_amendment_form.xml` & `trytond_sale_amendment-7.2.0/view/sale_amendment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.0.1/view/sale_amendment_line_form.xml` & `trytond_sale_amendment-7.2.0/view/sale_amendment_line_form.xml`

 * *Files identical despite different names*

