# Comparing `tmp/trytond_project_revenue-7.0.0.tar.gz` & `tmp/trytond_project_revenue-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_revenue-7.0.0.tar", last modified: Mon Oct 30 17:34:45 2023, max compression
+gzip compressed data, was "trytond_project_revenue-7.2.0.tar", last modified: Mon Apr 29 15:45:01 2024, max compression
```

## Comparing `trytond_project_revenue-7.0.0.tar` & `trytond_project_revenue-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:45.453507 trytond_project_revenue-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:23:13.000000 trytond_project_revenue-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2551 2023-10-30 17:10:14.000000 trytond_project_revenue-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:10:14.000000 trytond_project_revenue-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_revenue-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3140 2023-10-30 17:34:45.453507 trytond_project_revenue-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:45.450174 trytond_project_revenue-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:23:13.000000 trytond_project_revenue-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:13.000000 trytond_project_revenue-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:45.450174 trytond_project_revenue-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      888 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-10-30 16:47:45.000000 trytond_project_revenue-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      863 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      764 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      858 2023-10-30 16:47:45.000000 trytond_project_revenue-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      995 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      778 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-10-28 12:11:24.000000 trytond_project_revenue-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:21.000000 trytond_project_revenue-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:34:45.453507 trytond_project_revenue-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4463 2023-10-27 17:38:49.000000 trytond_project_revenue-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:45.450174 trytond_project_revenue-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3850 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/tests/scenario_project_revenue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_project_revenue-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      171 2023-10-30 17:10:10.000000 trytond_project_revenue-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:45.453507 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3140 2023-10-30 17:34:45.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1790 2023-10-30 17:34:45.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:34:45.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:34:45.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:34:45.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:34:45.000000 trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:45.450174 trytond_project_revenue-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-01-16 14:00:21.000000 trytond_project_revenue-7.0.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-01-16 14:00:21.000000 trytond_project_revenue-7.0.0/view/work_form_purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/view/work_list_children.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_project_revenue-7.0.0/view/work_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8171 2023-10-07 15:40:36.000000 trytond_project_revenue-7.0.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1512 2023-01-16 14:00:21.000000 trytond_project_revenue-7.0.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-29 15:23:19.000000 trytond_project_revenue-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:23:18.000000 trytond_project_revenue-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_revenue-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3140 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:01.375566 trytond_project_revenue-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_project_revenue-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:19.000000 trytond_project_revenue-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      888 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      863 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      764 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      858 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      995 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      778 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      824 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-29 13:17:17.000000 trytond_project_revenue-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      895 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2024-04-27 16:43:25.000000 trytond_project_revenue-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:21.000000 trytond_project_revenue-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4463 2024-03-17 11:01:36.000000 trytond_project_revenue-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3819 2024-04-22 12:14:36.000000 trytond_project_revenue-7.2.0/tests/scenario_project_revenue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:19.000000 trytond_project_revenue-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      171 2024-04-29 15:23:14.000000 trytond_project_revenue-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3140 2024-04-29 15:45:00.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1772 2024-04-29 15:45:01.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:00.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:45:00.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2024-04-29 15:45:00.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:00.000000 trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:01.378899 trytond_project_revenue-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-01-16 14:00:21.000000 trytond_project_revenue-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-01-16 14:00:21.000000 trytond_project_revenue-7.2.0/view/work_form_purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/view/work_list_children.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_project_revenue-7.2.0/view/work_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7783 2024-04-27 16:30:39.000000 trytond_project_revenue-7.2.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1512 2023-01-16 14:00:21.000000 trytond_project_revenue-7.2.0/work.xml
```

### Comparing `trytond_project_revenue-7.0.0/CHANGELOG` & `trytond_project_revenue-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_project_revenue-7.0.0/COPYRIGHT` & `trytond_project_revenue-7.2.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2008-2023 Cédric Krier.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 Cédric Krier.
+Copyright (C) 2008-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_project_revenue-7.0.0/LICENSE` & `trytond_project_revenue-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/PKG-INFO` & `trytond_project_revenue-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_project_revenue
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add revenue on project
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
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_project<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond_timesheet_cost<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_project<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond_timesheet_cost<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Project Revenue Module
 ######################
 
 The project revenue module computes revenue and cost per task and project.
 The revenue uses the list price of the product. If the product's unit of
 measure is time based, the revenue is computed as the product of the price and
```

### Comparing `trytond_project_revenue-7.0.0/doc/conf.py` & `trytond_project_revenue-7.2.0/doc/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_project_revenue-7.0.0/locale/bg.po` & `trytond_project_revenue-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/ca.po` & `trytond_project_revenue-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/cs.po` & `trytond_project_revenue-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/de.po` & `trytond_project_revenue-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/es.po` & `trytond_project_revenue-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/es_419.po` & `trytond_project_revenue-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/et.po` & `trytond_project_revenue-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/fa.po` & `trytond_project_revenue-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/fi.po` & `trytond_project_revenue-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/fr.po` & `trytond_project_revenue-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/hu.po` & `trytond_project_revenue-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/id.po` & `trytond_project_revenue-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/it.po` & `trytond_project_revenue-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/lo.po` & `trytond_project_revenue-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/lt.po` & `trytond_project_revenue-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/nl.po` & `trytond_project_revenue-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/pl.po` & `trytond_project_revenue-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/pt.po` & `trytond_project_revenue-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/ro.po` & `trytond_project_revenue-7.2.0/locale/tr.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,cost:"
 msgid "Cost"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:project.work,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
 msgctxt "field:project.work,list_price:"
 msgid "List Price"
-msgstr "Lista de preturi"
+msgstr ""
 
 msgctxt "field:project.work,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:project.work,purchase_lines:"
 msgid "Purchase Lines"
 msgstr ""
 
 msgctxt "field:project.work,revenue:"
 msgid "Revenue"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_project_revenue-7.0.0/locale/ru.po` & `trytond_project_revenue-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/sl.po` & `trytond_project_revenue-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/tr.po` & `trytond_project_revenue-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/uk.po` & `trytond_project_revenue-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/locale/zh_CN.po` & `trytond_project_revenue-7.2.0/locale/ro.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,cost:"
 msgid "Cost"
-msgstr ""
+msgstr "Cost"
 
 msgctxt "field:project.work,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:project.work,list_price:"
 msgid "List Price"
-msgstr ""
+msgstr "Lista de preturi"
 
 msgctxt "field:project.work,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:project.work,purchase_lines:"
 msgid "Purchase Lines"
-msgstr ""
+msgstr "Rânduri de Achiziție"
 
+#, fuzzy
 msgctxt "field:project.work,revenue:"
 msgid "Revenue"
-msgstr ""
+msgstr "Venit"
 
+#, fuzzy
 msgctxt "field:purchase.line,work:"
 msgid "Work Effort"
-msgstr ""
+msgstr "Efort de muncă"
 
+#, fuzzy
 msgctxt "help:purchase.line,work:"
 msgid "Add to the cost of the work effort."
-msgstr ""
+msgstr "Adaugă la costul efortului de muncă."
 
 msgctxt "view:project.work:"
 msgid "Purchases"
-msgstr ""
+msgstr "Achiziții"
 
 msgctxt "view:purchase.line:"
 msgid "Project"
-msgstr ""
+msgstr "Proiect"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_project_revenue-7.0.0/purchase.py` & `trytond_project_revenue-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/setup.py` & `trytond_project_revenue-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/tests/scenario_project_revenue.rst` & `trytond_project_revenue-7.2.0/tests/scenario_project_revenue.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Project Revenue Scenario
 ========================
 
 Imports::
 
     >>> import datetime
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('project_revenue')
 
 Create company::
```

### Comparing `trytond_project_revenue-7.0.0/tox.ini` & `trytond_project_revenue-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/PKG-INFO` & `trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-project-revenue
-Version: 7.0.0
+Name: trytond_project_revenue
+Version: 7.2.0
 Summary: Tryton module to add revenue on project
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
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_project<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond_timesheet_cost<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_project<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond_timesheet_cost<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Project Revenue Module
 ######################
 
 The project revenue module computes revenue and cost per task and project.
 The revenue uses the list price of the product. If the product's unit of
 measure is time based, the revenue is computed as the product of the price and
```

### Comparing `trytond_project_revenue-7.0.0/trytond_project_revenue.egg-info/SOURCES.txt` & `trytond_project_revenue-7.2.0/trytond_project_revenue.egg-info/SOURCES.txt`

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
 purchase.py
```

### Comparing `trytond_project_revenue-7.0.0/view/work_form.xml` & `trytond_project_revenue-7.2.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-7.0.0/work.py` & `trytond_project_revenue-7.2.0/work.py`

 * *Files 6% similar despite different names*

```diff
@@ -168,40 +168,31 @@
             revenues[work.id] = work.company.currency.round(revenue)
         return revenues
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
         return self.company.currency if self.company else None
 
-    @fields.depends('product', 'company')
+    @fields.depends('product')
     def on_change_product(self):
         pool = Pool()
-        User = pool.get('res.user')
         ModelData = pool.get('ir.model.data')
         Uom = pool.get('product.uom')
-        Currency = pool.get('currency.currency')
 
         if not self.product:
             return
 
-        if self.price_list_hour:
-            hour_uom = Uom(ModelData.get_id('product', 'uom_hour'))
-            self.list_price = Uom.compute_price(
-                self.product.default_uom, self.product.list_price, hour_uom)
-        else:
-            self.list_price = self.product.list_price
-
-        if self.company:
-            user = User(Transaction().user)
-            if user.company != self.company:
-                if user.company.currency != self.company.currency:
-                    self.list_price = Currency.compute(user.company.currency,
-                        self.list_price, self.company.currency, round=False)
-
-        self.list_price = round_price(self.list_price)
+        list_price = self.product.list_price_used
+        if list_price is not None:
+            if self.price_list_hour:
+                hour_uom = Uom(ModelData.get_id('product', 'uom_hour'))
+                list_price = Uom.compute_price(
+                    self.product.default_uom, list_price, hour_uom)
+            list_price = round_price(list_price)
+        self.list_price = list_price
 
     @property
     def price_list_hour(self):
         pool = Pool()
         ModelData = pool.get('ir.model.data')
         Category = pool.get('product.uom.category')
         if not self.product:
```

### Comparing `trytond_project_revenue-7.0.0/work.xml` & `trytond_project_revenue-7.2.0/work.xml`

 * *Files identical despite different names*
