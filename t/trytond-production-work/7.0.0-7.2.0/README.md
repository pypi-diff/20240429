# Comparing `tmp/trytond_production_work-7.0.0.tar.gz` & `tmp/trytond_production_work-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_work-7.0.0.tar", last modified: Mon Oct 30 17:34:09 2023, max compression
+gzip compressed data, was "trytond_production_work-7.2.0.tar", last modified: Mon Apr 29 15:44:27 2024, max compression
```

## Comparing `trytond_production_work-7.0.0.tar` & `trytond_production_work-7.2.0.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:09.560003 trytond_production_work-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:23:12.000000 trytond_production_work-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1615 2023-10-30 17:09:51.000000 trytond_production_work-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-10-30 17:09:51.000000 trytond_production_work-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2023-10-30 17:34:09.560003 trytond_production_work-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:09.560003 trytond_production_work-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:23:12.000000 trytond_production_work-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:12.000000 trytond_production_work-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:09.556669 trytond_production_work-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7172 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6990 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7093 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7025 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6136 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6549 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6854 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6329 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7025 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6784 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6138 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6621 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7227 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6400 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6891 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6624 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6691 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6019 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7250 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6878 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6650 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5968 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6574 2023-10-30 16:47:45.000000 trytond_production_work-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4001 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)      734 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1139 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/routing.py
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/routing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:34:09.560003 trytond_production_work-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2023-10-27 17:38:49.000000 trytond_production_work-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:09.556669 trytond_production_work-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7983 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/tests/scenario_production_work.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_production_work-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-10-30 17:09:47.000000 trytond_production_work-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:09.560003 trytond_production_work-7.0.0/trytond_production_work.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2023-10-30 17:34:09.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2362 2023-10-30 17:34:09.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:34:09.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:34:09.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-10-30 17:34:09.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:34:09.000000 trytond_production_work-7.0.0/trytond_production_work.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:09.556669 trytond_production_work-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/view/operation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/view/operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/view/work_center_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/view/work_center_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/view/work_center_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/view/work_center_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/view/work_center_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      690 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/view/work_cycle_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-01-16 14:00:21.000000 trytond_production_work-7.0.0/view/work_cycle_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_production_work-7.0.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/view/work_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14680 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15346 2023-10-07 15:40:36.000000 trytond_production_work-7.0.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1716 2024-04-29 15:22:51.000000 trytond_production_work-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2024-04-29 15:22:50.000000 trytond_production_work-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.813110 trytond_production_work-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:18.000000 trytond_production_work-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.816444 trytond_production_work-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7172 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6990 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6355 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7093 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7025 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6136 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6549 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6854 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6329 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7025 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6784 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6138 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6621 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7227 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6400 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6891 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6624 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6691 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7032 2024-04-29 13:17:17.000000 trytond_production_work-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6878 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6650 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5968 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6574 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      734 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1139 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/routing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/routing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2024-03-17 11:01:36.000000 trytond_production_work-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.816444 trytond_production_work-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7987 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/tests/scenario_production_work.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:18.000000 trytond_production_work-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-29 15:22:46.000000 trytond_production_work-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/trytond_production_work.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/operation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/work_center_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_center_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/work_center_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_center_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_center_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      690 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/view/work_cycle_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/work_cycle_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/view/work_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14680 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14850 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/work.xml
```

### Comparing `trytond_production_work-7.0.0/CHANGELOG` & `trytond_production_work-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

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
 * Add employee on cycles for running and done states
 * Display cost of works
```

### Comparing `trytond_production_work-7.0.0/COPYRIGHT` & `trytond_production_work-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2023 Cédric Krier.
-Copyright (C) 2015-2023 B2CK SPRL.
+Copyright (C) 2015-2024 Cédric Krier.
+Copyright (C) 2015-2024 B2CK SPRL.
 Copyright (C) 2013-2015 NaN·tic.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_production_work-7.0.0/LICENSE` & `trytond_production_work-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/PKG-INFO` & `trytond_production_work-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_production_work
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for production work
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_production_routing<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_production_routing<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Production Work Module
 ######################
 
 The production work module allows to manage work order for each production.
 It also adds in the production cost for the work cost.
```

### Comparing `trytond_production_work-7.0.0/README.rst` & `trytond_production_work-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/doc/conf.py` & `trytond_production_work-7.2.0/doc/conf.py`

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

### Comparing `trytond_production_work-7.0.0/doc/index.rst` & `trytond_production_work-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/bg.po` & `trytond_production_work-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/ca.po` & `trytond_production_work-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/cs.po` & `trytond_production_work-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/de.po` & `trytond_production_work-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/es.po` & `trytond_production_work-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/es_419.po` & `trytond_production_work-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/et.po` & `trytond_production_work-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/fa.po` & `trytond_production_work-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/fi.po` & `trytond_production_work-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/fr.po` & `trytond_production_work-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/hu.po` & `trytond_production_work-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/id.po` & `trytond_production_work-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/it.po` & `trytond_production_work-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/lo.po` & `trytond_production_work-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/lt.po` & `trytond_production_work-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/nl.po` & `trytond_production_work-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/pl.po` & `trytond_production_work-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/pt.po` & `trytond_production_work-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/ro.po` & `trytond_production_work-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 
 msgctxt "field:production.work,active_cycles:"
 msgid "Active Cycles"
 msgstr ""
 
 msgctxt "field:production.work,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:production.work,cost:"
 msgid "Cost"
-msgstr "Cost"
+msgstr ""
 
 msgctxt "field:production.work,cycles:"
 msgid "Cycles"
 msgstr ""
 
 msgctxt "field:production.work,operation:"
 msgid "Operation"
@@ -53,76 +52,75 @@
 
 msgctxt "field:production.work,work_center_category:"
 msgid "Work Center Category"
 msgstr ""
 
 msgctxt "field:production.work.center,category:"
 msgid "Category"
-msgstr "Categorie"
+msgstr ""
 
 msgctxt "field:production.work.center,children:"
 msgid "Children"
-msgstr "Copii"
+msgstr ""
 
 msgctxt "field:production.work.center,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:production.work.center,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
 msgctxt "field:production.work.center,cost_price:"
 msgid "Cost Price"
-msgstr "Cost"
+msgstr ""
 
 msgctxt "field:production.work.center,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr ""
 
 msgctxt "field:production.work.center,parent:"
 msgid "Parent"
-msgstr "Părinte"
+msgstr ""
 
 msgctxt "field:production.work.center,warehouse:"
 msgid "Warehouse"
-msgstr "Depozit"
+msgstr ""
 
 msgctxt "field:production.work.center.category,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr ""
 
 msgctxt "field:production.work.cycle,cancelled_by:"
 msgid "Cancelled By"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:production.work.cycle,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:production.work.cycle,cost:"
 msgid "Cost"
-msgstr "Cost"
+msgstr ""
 
 msgctxt "field:production.work.cycle,done_by:"
 msgid "Done By"
 msgstr ""
 
 msgctxt "field:production.work.cycle,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr ""
 
 msgctxt "field:production.work.cycle,run_by:"
 msgid "Run By"
 msgstr ""
 
 msgctxt "field:production.work.cycle,state:"
 msgid "State"
-msgstr "Stare"
+msgstr ""
 
 msgctxt "field:production.work.cycle,work:"
 msgid "Work"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_work_center_category_list"
 msgid "Work Center Categories"
@@ -134,19 +132,19 @@
 
 msgctxt "model:ir.action,name:act_work_center_tree"
 msgid "Work Centers"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "Manopera"
+msgstr "Роботи"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
-msgstr "Toate"
+msgstr "Усі"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_draft"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_request"
 msgid "Request"
@@ -196,15 +194,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_center_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.rule.group,name:rule_group_work_cycle_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_category_list"
 msgid "Work Center Categories"
@@ -216,15 +214,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_tree"
 msgid "Work Centers"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr ""
+msgstr "Роботи"
 
 msgctxt "model:production.work,name:"
 msgid "Production Work"
 msgstr ""
 
 msgctxt "model:production.work.center,name:"
 msgid "Work Center"
```

### Comparing `trytond_production_work-7.0.0/locale/ru.po` & `trytond_production_work-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/sl.po` & `trytond_production_work-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/tr.po` & `trytond_production_work-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/locale/uk.po` & `trytond_production_work-7.2.0/locale/zh_CN.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:production,work_center:"
 msgid "Work Center"
-msgstr ""
+msgstr "Work Centers"
 
+#, fuzzy
 msgctxt "field:production,works:"
 msgid "Works"
-msgstr ""
+msgstr "Works"
 
+#, fuzzy
 msgctxt "field:production.routing.operation,work_center_category:"
 msgid "Work Center Category"
-msgstr ""
+msgstr "Work Center Categories"
 
+#, fuzzy
 msgctxt "field:production.work,active_cycles:"
 msgid "Active Cycles"
-msgstr ""
+msgstr "启用"
 
 msgctxt "field:production.work,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:production.work,cost:"
 msgid "Cost"
@@ -34,133 +38,145 @@
 msgid "Operation"
 msgstr ""
 
 msgctxt "field:production.work,production:"
 msgid "Production"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
 msgctxt "field:production.work,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work,work_center:"
 msgid "Work Center"
-msgstr ""
+msgstr "Work Centers"
 
+#, fuzzy
 msgctxt "field:production.work,work_center_category:"
 msgid "Work Center Category"
-msgstr ""
+msgstr "Work Center Categories"
 
 msgctxt "field:production.work.center,category:"
 msgid "Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work.center,children:"
 msgid "Children"
-msgstr ""
+msgstr "子项"
 
 msgctxt "field:production.work.center,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:production.work.center,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
 msgctxt "field:production.work.center,cost_price:"
 msgid "Cost Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work.center,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
+#, fuzzy
 msgctxt "field:production.work.center,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "上级"
 
 msgctxt "field:production.work.center,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work.center.category,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
+#, fuzzy
 msgctxt "field:production.work.cycle,cancelled_by:"
 msgid "Cancelled By"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "field:production.work.cycle,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:production.work.cycle,cost:"
 msgid "Cost"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work.cycle,done_by:"
 msgid "Done By"
-msgstr ""
+msgstr "完成"
 
 msgctxt "field:production.work.cycle,duration:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "field:production.work.cycle,run_by:"
 msgid "Run By"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.work.cycle,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
+#, fuzzy
 msgctxt "field:production.work.cycle,work:"
 msgid "Work"
-msgstr ""
+msgstr "Works"
 
 msgctxt "model:ir.action,name:act_work_center_category_list"
 msgid "Work Center Categories"
-msgstr ""
+msgstr "Work Center Categories"
 
 msgctxt "model:ir.action,name:act_work_center_list"
 msgid "Work Centers"
-msgstr ""
+msgstr "Work Centers"
 
 msgctxt "model:ir.action,name:act_work_center_tree"
 msgid "Work Centers"
-msgstr ""
+msgstr "Work Centers"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "Роботи"
+msgstr "工作"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
-msgstr "Усі"
+msgstr "全部"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_request"
 msgid "Request"
-msgstr ""
+msgstr "Request"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_running"
 msgid "Running"
-msgstr ""
+msgstr "Running"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_waiting"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
 msgctxt "model:ir.message,text:msg_delete_request"
 msgid "To delete work \"%(work)s\" it must be in the \"request\" or \"draft\" state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_do_finished_work"
 msgid "To complete production \"%(production)s\", work \"%(work)s\" must be finished."
@@ -170,116 +186,129 @@
 msgid ""
 "Could not find a work center of category \"%(category)s\" under "
 "\"%(parent)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:work_cycle_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:work_cycle_do_button"
 msgid "Do"
-msgstr ""
+msgstr "Do"
 
 msgctxt "model:ir.model.button,string:work_cycle_run_button"
 msgid "Run"
-msgstr ""
+msgstr "Run"
 
 msgctxt "model:ir.model.button,string:work_start_button"
 msgid "Start"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:work_stop_button"
 msgid "Stop"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_center_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr "Користувач у компаніях"
+msgstr "公司中的用户"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_cycle_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_category_list"
 msgid "Work Center Categories"
-msgstr ""
+msgstr "Work Center Categories"
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_list"
 msgid "Work Centers"
-msgstr ""
+msgstr "Work Centers"
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_tree"
 msgid "Work Centers"
-msgstr ""
+msgstr "Work Centers"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr "Роботи"
+msgstr "工作"
 
 msgctxt "model:production.work,name:"
 msgid "Production Work"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:production.work.center,name:"
 msgid "Work Center"
-msgstr ""
+msgstr "Work Centers"
 
+#, fuzzy
 msgctxt "model:production.work.center.category,name:"
 msgid "Work Center Category"
-msgstr ""
+msgstr "Work Center Categories"
 
 msgctxt "model:production.work.cycle,name:"
 msgid "Work Cycle"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Done"
-msgstr ""
+msgstr "完成"
 
+#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "selection:production.work,state:"
 msgid "Finished"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Request"
-msgstr ""
+msgstr "Request"
 
+#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Running"
-msgstr ""
+msgstr "Running"
 
+#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
 msgctxt "selection:production.work.center,cost_method:"
 msgid "Per Cycle"
 msgstr ""
 
 msgctxt "selection:production.work.center,cost_method:"
 msgid "Per Hour"
 msgstr ""
 
 msgctxt "selection:production.work.cycle,state:"
 msgid "Cancelled"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:production.work.cycle,state:"
 msgid "Done"
-msgstr ""
+msgstr "完成"
 
+#, fuzzy
 msgctxt "selection:production.work.cycle,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:production.work.cycle,state:"
 msgid "Running"
-msgstr ""
+msgstr "Running"
```

### Comparing `trytond_production_work-7.0.0/locale/zh_CN.po` & `trytond_production_work-7.2.0/locale/ro.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,314 +1,309 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:production,work_center:"
 msgid "Work Center"
-msgstr "Work Centers"
+msgstr "Centru de lucru"
 
-#, fuzzy
 msgctxt "field:production,works:"
 msgid "Works"
-msgstr "Works"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:production.routing.operation,work_center_category:"
 msgid "Work Center Category"
-msgstr "Work Center Categories"
+msgstr "Categorie Centru de lucru"
 
 #, fuzzy
 msgctxt "field:production.work,active_cycles:"
 msgid "Active Cycles"
-msgstr "启用"
+msgstr "Cicluri active"
 
 msgctxt "field:production.work,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:production.work,cost:"
 msgid "Cost"
-msgstr ""
+msgstr "Cost"
 
 msgctxt "field:production.work,cycles:"
 msgid "Cycles"
-msgstr ""
+msgstr "Cicluri"
 
 msgctxt "field:production.work,operation:"
 msgid "Operation"
-msgstr ""
+msgstr "Operațiune"
 
 msgctxt "field:production.work,production:"
 msgid "Production"
-msgstr ""
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "field:production.work,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
 msgctxt "field:production.work,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Depozit"
 
 #, fuzzy
 msgctxt "field:production.work,work_center:"
 msgid "Work Center"
-msgstr "Work Centers"
+msgstr "Centru de lucru"
 
 #, fuzzy
 msgctxt "field:production.work,work_center_category:"
 msgid "Work Center Category"
-msgstr "Work Center Categories"
+msgstr "Categorie Centru de lucru"
 
 msgctxt "field:production.work.center,category:"
 msgid "Category"
-msgstr ""
+msgstr "Categorie"
 
-#, fuzzy
 msgctxt "field:production.work.center,children:"
 msgid "Children"
-msgstr "子项"
+msgstr "Copii"
 
 msgctxt "field:production.work.center,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:production.work.center,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
 msgctxt "field:production.work.center,cost_price:"
 msgid "Cost Price"
-msgstr ""
+msgstr "Cost"
 
-#, fuzzy
 msgctxt "field:production.work.center,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Denumire"
 
-#, fuzzy
 msgctxt "field:production.work.center,parent:"
 msgid "Parent"
-msgstr "上级"
+msgstr "Părinte"
 
 msgctxt "field:production.work.center,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Depozit"
 
-#, fuzzy
 msgctxt "field:production.work.center.category,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Denumire"
 
-#, fuzzy
 msgctxt "field:production.work.cycle,cancelled_by:"
 msgid "Cancelled By"
-msgstr "Cancel"
+msgstr "Anulat de"
 
 msgctxt "field:production.work.cycle,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:production.work.cycle,cost:"
 msgid "Cost"
-msgstr ""
+msgstr "Cost"
 
-#, fuzzy
 msgctxt "field:production.work.cycle,done_by:"
 msgid "Done By"
-msgstr "完成"
+msgstr ""
 
 msgctxt "field:production.work.cycle,duration:"
 msgid "Duration"
-msgstr ""
+msgstr "Durata"
 
+#, fuzzy
 msgctxt "field:production.work.cycle,run_by:"
 msgid "Run By"
-msgstr ""
+msgstr "Condus de"
 
-#, fuzzy
 msgctxt "field:production.work.cycle,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
 #, fuzzy
 msgctxt "field:production.work.cycle,work:"
 msgid "Work"
-msgstr "Works"
+msgstr "Muncă"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_work_center_category_list"
 msgid "Work Center Categories"
-msgstr "Work Center Categories"
+msgstr "Categorii de centre de lucru"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_work_center_list"
 msgid "Work Centers"
-msgstr "Work Centers"
+msgstr "Centre de lucru"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_work_center_tree"
 msgid "Work Centers"
-msgstr "Work Centers"
+msgstr "Centre de lucru"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "工作"
+msgstr "Manopera"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Toate"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_request"
 msgid "Request"
-msgstr "Request"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_running"
 msgid "Running"
-msgstr "Running"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_waiting"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
 msgctxt "model:ir.message,text:msg_delete_request"
 msgid "To delete work \"%(work)s\" it must be in the \"request\" or \"draft\" state."
 msgstr ""
+"Pentru a șterge lucrarea \"%(work)s\" trebuie să fie în starea „cerere” sau "
+"„ciornă”."
 
 msgctxt "model:ir.message,text:msg_do_finished_work"
 msgid "To complete production \"%(production)s\", work \"%(work)s\" must be finished."
 msgstr ""
+"Pentru a finaliza producția \"%(production)s\", lucrarea \"%(work)s\" "
+"trebuie să fie terminată."
 
 msgctxt "model:ir.message,text:msg_missing_work_center"
 msgid ""
 "Could not find a work center of category \"%(category)s\" under "
 "\"%(parent)s\"."
 msgstr ""
+"Nu s-a putut găsi un centru de lucru din categoria \"%(category)s\" sub "
+"\"%(parent)s\"."
 
 msgctxt "model:ir.model.button,string:work_cycle_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:work_cycle_do_button"
 msgid "Do"
-msgstr "Do"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:work_cycle_run_button"
 msgid "Run"
-msgstr "Run"
+msgstr "Rulează"
 
 msgctxt "model:ir.model.button,string:work_start_button"
 msgid "Start"
-msgstr ""
+msgstr "Start"
 
 msgctxt "model:ir.model.button,string:work_stop_button"
 msgid "Stop"
-msgstr ""
+msgstr "Stop"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_center_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în Companii"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în companii"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_cycle_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în Companii"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_center_category_list"
 msgid "Work Center Categories"
-msgstr "Work Center Categories"
+msgstr "Categorii de centre de lucru"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_center_list"
 msgid "Work Centers"
-msgstr "Work Centers"
+msgstr "Centre de lucru"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_center_tree"
 msgid "Work Centers"
-msgstr "Work Centers"
+msgstr "Centre de lucru"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr "工作"
+msgstr "Lucrări"
 
+#, fuzzy
 msgctxt "model:production.work,name:"
 msgid "Production Work"
-msgstr ""
+msgstr "Muncă de producție"
 
 #, fuzzy
 msgctxt "model:production.work.center,name:"
 msgid "Work Center"
-msgstr "Work Centers"
+msgstr "Centru de lucru"
 
 #, fuzzy
 msgctxt "model:production.work.center.category,name:"
 msgid "Work Center Category"
-msgstr "Work Center Categories"
+msgstr "Categorie Centru de lucru"
 
+#, fuzzy
 msgctxt "model:production.work.cycle,name:"
 msgid "Work Cycle"
-msgstr ""
+msgstr "Ciclul de lucru"
 
-#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Done"
-msgstr "完成"
+msgstr "Terminat"
 
-#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 msgctxt "selection:production.work,state:"
 msgid "Finished"
-msgstr ""
+msgstr "Terminat"
 
-#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Request"
-msgstr "Request"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Running"
-msgstr "Running"
+msgstr "În derulare"
 
-#, fuzzy
 msgctxt "selection:production.work,state:"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
 msgctxt "selection:production.work.center,cost_method:"
 msgid "Per Cycle"
-msgstr ""
+msgstr "Pe ciclu"
 
 msgctxt "selection:production.work.center,cost_method:"
 msgid "Per Hour"
-msgstr ""
+msgstr "Pe oră"
 
 msgctxt "selection:production.work.cycle,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Anulat"
 
-#, fuzzy
 msgctxt "selection:production.work.cycle,state:"
 msgid "Done"
-msgstr "完成"
+msgstr "Terminat"
 
-#, fuzzy
 msgctxt "selection:production.work.cycle,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
-#, fuzzy
 msgctxt "selection:production.work.cycle,state:"
 msgid "Running"
-msgstr "Running"
+msgstr "În derulare"
```

### Comparing `trytond_production_work-7.0.0/message.xml` & `trytond_production_work-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/production.py` & `trytond_production_work-7.2.0/production.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,25 +90,25 @@
         super(Production, cls).run(productions)
 
         Work.set_state([w for p in productions for w in p.works])
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, productions):
+    def do(cls, productions):
         pool = Pool()
         Work = pool.get('production.work')
         for production in productions:
             for work in production.works:
                 if work.state != 'finished':
                     raise AccessError(
                         gettext('production_work.msg_do_finished_work',
                             production=production.rec_name,
                             work=work.rec_name))
-        super(Production, cls).done(productions)
+        super().do(productions)
         Work.set_state([w for p in productions for w in p.works])
 
     @classmethod
     def copy(cls, productions, default=None):
         if default is None:
             default = {}
         else:
```

### Comparing `trytond_production_work-7.0.0/production.xml` & `trytond_production_work-7.2.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/routing.py` & `trytond_production_work-7.2.0/routing.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/routing.xml` & `trytond_production_work-7.2.0/routing.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/setup.py` & `trytond_production_work-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/tests/scenario_production_work.rst` & `trytond_production_work-7.2.0/tests/scenario_production_work.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Production Work Scenario
 ========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('production_work')
 
@@ -182,24 +182,20 @@
     'waiting'
     >>> production.cost
     Decimal('2.0000')
 
 Test works::
 
     >>> work1, work2 = production.works
-    >>> work1.operation == operation1
-    True
-    >>> work1.work_center == center1
-    True
+    >>> assertEqual(work1.operation, operation1)
+    >>> assertEqual(work1.work_center, center1)
     >>> work1.state
     'request'
-    >>> work2.operation == operation2
-    True
-    >>> work2.work_center == center2
-    True
+    >>> assertEqual(work2.operation, operation2)
+    >>> assertEqual(work2.work_center, center2)
     >>> work2.state
     'request'
 
 Run the production::
 
     >>> production.click('assign_try')
     >>> production.click('run')
@@ -216,31 +212,28 @@
 
 Run works::
 
     >>> cycle1 = work1.cycles.new()
     >>> cycle1.click('run')
     >>> cycle1.state
     'running'
-    >>> cycle1.run_by == employee
-    True
+    >>> assertEqual(cycle1.run_by, employee)
     >>> work1.reload()
     >>> work1.state
     'running'
     >>> cycle1.click('do')
     >>> cycle1.state
     'done'
-    >>> cycle1.done_by == employee
-    True
+    >>> assertEqual(cycle1.done_by, employee)
     >>> work1.reload()
     >>> work1.state
     'finished'
     >>> cycle2 = work2.cycles.new()
     >>> cycle2.click('cancel')
-    >>> cycle2.cancelled_by == employee
-    True
+    >>> assertEqual(cycle2.cancelled_by, employee)
     >>> cycle2.state
     'cancelled'
     >>> work2.reload()
     >>> work2.state
     'draft'
     >>> work2.click('start')
     >>> cycle2, = [c for c in work2.active_cycles]
@@ -276,15 +269,15 @@
     >>> work1.cost
     Decimal('10.0000')
     >>> work2.cost
     Decimal('5.0000')
 
 Do the production::
 
-    >>> production.click('done')
+    >>> production.click('do')
     >>> production.state
     'done'
 
 Work is now done::
 
     >>> work2.reload()
     >>> work2.state
```

### Comparing `trytond_production_work-7.0.0/tox.ini` & `trytond_production_work-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/trytond_production_work.egg-info/PKG-INFO` & `trytond_production_work-7.2.0/trytond_production_work.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-production-work
-Version: 7.0.0
+Name: trytond_production_work
+Version: 7.2.0
 Summary: Tryton module for production work
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_production_routing<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_production_routing<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Production Work Module
 ######################
 
 The production work module allows to manage work order for each production.
 It also adds in the production cost for the work cost.
```

### Comparing `trytond_production_work-7.0.0/trytond_production_work.egg-info/SOURCES.txt` & `trytond_production_work-7.2.0/trytond_production_work.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_production_work-7.0.0/view/production_form.xml` & `trytond_production_work-7.2.0/view/production_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/view/work_center_form.xml` & `trytond_production_work-7.2.0/view/work_center_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/view/work_cycle_form.xml` & `trytond_production_work-7.2.0/view/work_cycle_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/view/work_form.xml` & `trytond_production_work-7.2.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/work.py` & `trytond_production_work-7.2.0/work.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.0.0/work.xml` & `trytond_production_work-7.2.0/work.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_production_work-7.0.0/work.xml` & `trytond_production_work-7.2.0/work.xml`

```diff
@@ -55,31 +55,31 @@
     <record model="ir.action.act_window.view" id="act_work_center_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="work_center_view_form"/>
       <field name="act_window" ref="act_work_center_list"/>
     </record>
     <menuitem parent="menu_work_center_tree" action="act_work_center_list" sequence="10" id="menu_work_center_list"/>
     <record model="ir.model.access" id="access_work_center">
-      <field name="model" search="[('model', '=', 'production.work.center')]"/>
+      <field name="model">production.work.center</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_center_admin">
-      <field name="model" search="[('model', '=', 'production.work.center')]"/>
+      <field name="model">production.work.center</field>
       <field name="group" ref="production.group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_work_center_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'production.work.center')]"/>
+      <field name="model">production.work.center</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_work_center_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_work_center_companies"/>
     </record>
     <record model="ir.ui.view" id="work_center_category_view_list">
@@ -104,22 +104,22 @@
     <record model="ir.action.act_window.view" id="act_work_center_category_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="work_center_category_view_form"/>
       <field name="act_window" ref="act_work_center_category_list"/>
     </record>
     <menuitem parent="production.menu_configuration" action="act_work_center_category_list" sequence="50" id="menu_work_center_category_list"/>
     <record model="ir.model.access" id="access_work_center_category">
-      <field name="model" search="[('model', '=', 'production.work.center.category')]"/>
+      <field name="model">production.work.center.category</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_center_category_admin">
-      <field name="model" search="[('model', '=', 'production.work.center.category')]"/>
+      <field name="model">production.work.center.category</field>
       <field name="group" ref="production.group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="work_view_list">
@@ -182,41 +182,41 @@
     <record model="ir.action.act_window.domain" id="act_work_list_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="act_window" ref="act_work_list"/>
     </record>
     <menuitem parent="production.menu_production" action="act_work_list" sequence="20" id="menu_work_list"/>
     <record model="ir.model.access" id="access_work">
-      <field name="model" search="[('model', '=', 'production.work')]"/>
+      <field name="model">production.work</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_group_production">
-      <field name="model" search="[('model', '=', 'production.work')]"/>
+      <field name="model">production.work</field>
       <field name="group" ref="production.group_production"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="work_start_button">
+      <field name="model">production.work</field>
       <field name="name">start</field>
       <field name="string">Start</field>
-      <field name="model" search="[('model', '=', 'production.work')]"/>
     </record>
     <record model="ir.model.button" id="work_stop_button">
+      <field name="model">production.work</field>
       <field name="name">stop</field>
       <field name="string">Stop</field>
-      <field name="model" search="[('model', '=', 'production.work')]"/>
     </record>
     <record model="ir.rule.group" id="rule_group_work_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'production.work')]"/>
+      <field name="model">production.work</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_work_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_work_companies"/>
     </record>
     <record model="ir.ui.view" id="work_cycle_view_list">
@@ -226,46 +226,46 @@
     </record>
     <record model="ir.ui.view" id="work_cycle_view_form">
       <field name="model">production.work.cycle</field>
       <field name="type">form</field>
       <field name="name">work_cycle_form</field>
     </record>
     <record model="ir.model.access" id="access_work_cycle">
-      <field name="model" search="[('model', '=', 'production.work.cycle')]"/>
+      <field name="model">production.work.cycle</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_cycle_group_production">
-      <field name="model" search="[('model', '=', 'production.work.cycle')]"/>
+      <field name="model">production.work.cycle</field>
       <field name="group" ref="production.group_production"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="work_cycle_cancel_button">
+      <field name="model">production.work.cycle</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'production.work.cycle')]"/>
     </record>
     <record model="ir.model.button" id="work_cycle_do_button">
+      <field name="model">production.work.cycle</field>
       <field name="name">do</field>
       <field name="string">Do</field>
-      <field name="model" search="[('model', '=', 'production.work.cycle')]"/>
     </record>
     <record model="ir.model.button" id="work_cycle_run_button">
+      <field name="model">production.work.cycle</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'production.work.cycle')]"/>
     </record>
     <record model="ir.rule.group" id="rule_group_work_cycle_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'production.work.cycle')]"/>
+      <field name="model">production.work.cycle</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_work_cycle_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_work_cycle_companies"/>
     </record>
   </data>
```

