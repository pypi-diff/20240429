# Comparing `tmp/trytond_production_split-7.0.0.tar.gz` & `tmp/trytond_production_split-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_split-7.0.0.tar", last modified: Mon Oct 30 17:34:02 2023, max compression
+gzip compressed data, was "trytond_production_split-7.2.0.tar", last modified: Mon Apr 29 15:44:21 2024, max compression
```

## Comparing `trytond_production_split-7.0.0.tar` & `trytond_production_split-7.2.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.083300 trytond_production_split-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:23:11.000000 trytond_production_split-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1367 2023-10-30 17:09:47.000000 trytond_production_split-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-10-30 17:09:46.000000 trytond_production_split-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_split-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_split-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2023-10-30 17:34:02.083300 trytond_production_split-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_production_split-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_production_split-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.079967 trytond_production_split-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:23:11.000000 trytond_production_split-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_production_split-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:11.000000 trytond_production_split-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.079967 trytond_production_split-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_production_split-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_production_split-7.0.0/icons/tryton-production-split.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.079967 trytond_production_split-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1145 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1157 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1120 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1181 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1157 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1113 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      993 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1113 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1165 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1165 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1115 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-10-30 16:47:45.000000 trytond_production_split-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3634 2023-10-24 07:56:52.000000 trytond_production_split-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1477 2023-01-16 14:00:21.000000 trytond_production_split-7.0.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:34:02.083300 trytond_production_split-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4333 2023-10-27 17:38:49.000000 trytond_production_split-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.079967 trytond_production_split-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_split-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1551 2023-10-07 17:14:58.000000 trytond_production_split-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_production_split-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:09:43.000000 trytond_production_split-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.083300 trytond_production_split-7.0.0/trytond_production_split.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2023-10-30 17:34:01.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-10-30 17:34:02.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:34:01.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:34:01.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-10-30 17:34:01.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:34:01.000000 trytond_production_split-7.0.0/trytond_production_split.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:02.079967 trytond_production_split-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_production_split-7.0.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-07 17:14:58.000000 trytond_production_split-7.0.0/view/split_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1468 2024-04-29 15:22:45.000000 trytond_production_split-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2024-04-29 15:22:45.000000 trytond_production_split-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_split-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_production_split-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.876599 trytond_production_split-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_production_split-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_production_split-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:18.000000 trytond_production_split-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.876599 trytond_production_split-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/icons/tryton-production-split.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1145 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1157 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1120 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1181 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1157 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      993 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1207 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1165 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1165 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1115 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3634 2024-02-04 18:51:26.000000 trytond_production_split-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1438 2024-04-27 16:30:39.000000 trytond_production_split-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4333 2024-03-17 11:01:36.000000 trytond_production_split-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2024-02-04 18:51:26.000000 trytond_production_split-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:18.000000 trytond_production_split-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:22:41.000000 trytond_production_split-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/trytond_production_split.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1525 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       55 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-02-04 18:51:26.000000 trytond_production_split-7.2.0/view/split_start_form.xml
```

### Comparing `trytond_production_split-7.0.0/CHANGELOG` & `trytond_production_split-7.2.0/CHANGELOG`

 * *Files 18% similar despite different names*

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

### Comparing `trytond_production_split-7.0.0/COPYRIGHT` & `trytond_production_split-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2016-2023 Cédric Krier
-Copyright (C) 2016-2023 B2CK
+Copyright (C) 2016-2024 Cédric Krier
+Copyright (C) 2016-2024 B2CK
 Copyright (C) 2014 NaN·tic
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_production_split-7.0.0/LICENSE` & `trytond_production_split-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/PKG-INFO` & `trytond_production_split-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_production_split
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to split production
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
@@ -46,16 +46,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Production Split Module
 #######################
 
 The Production Split module adds on the production a wizard that allows to
 split it.
```

### Comparing `trytond_production_split-7.0.0/doc/conf.py` & `trytond_production_split-7.2.0/doc/conf.py`

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

### Comparing `trytond_production_split-7.0.0/icons/LICENSE` & `trytond_production_split-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/bg.po` & `trytond_production_split-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/ca.po` & `trytond_production_split-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/cs.po` & `trytond_production_split-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/de.po` & `trytond_production_split-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/es.po` & `trytond_production_split-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/es_419.po` & `trytond_production_split-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/et.po` & `trytond_production_split-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/fa.po` & `trytond_production_split-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/fi.po` & `trytond_production_split-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/fr.po` & `trytond_production_split-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/hu.po` & `trytond_production_split-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/id.po` & `trytond_production_split-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/it.po` & `trytond_production_split-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/lo.po` & `trytond_production_split-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/lt.po` & `trytond_production_split-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/nl.po` & `trytond_production_split-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/pl.po` & `trytond_production_split-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/pt.po` & `trytond_production_split-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/ro.po` & `trytond_production_split-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/ru.po` & `trytond_production_split-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/sl.po` & `trytond_production_split-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/tr.po` & `trytond_production_split-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/uk.po` & `trytond_production_split-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/locale/zh_CN.po` & `trytond_production_split-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/production.py` & `trytond_production_split-7.2.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/production.xml` & `trytond_production_split-7.2.0/production.xml`

 * *Files 15% similar despite different names*

#### Comparing `trytond_production_split-7.0.0/production.xml` & `trytond_production_split-7.2.0/production.xml`

```diff
@@ -19,13 +19,13 @@
     </record>
     <record model="ir.ui.view" id="split_start_view_form">
       <field name="model">production.split.start</field>
       <field name="type">form</field>
       <field name="name">split_start_form</field>
     </record>
     <record model="ir.model.button" id="production_split_wizard_button">
+      <field name="model">production</field>
       <field name="name">split_wizard</field>
       <field name="string">Split</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_production_split-7.0.0/setup.py` & `trytond_production_split-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/tests/test_module.py` & `trytond_production_split-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/tox.ini` & `trytond_production_split-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.0.0/trytond_production_split.egg-info/PKG-INFO` & `trytond_production_split-7.2.0/trytond_production_split.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-production-split
-Version: 7.0.0
+Name: trytond_production_split
+Version: 7.2.0
 Summary: Tryton module to split production
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
@@ -46,16 +46,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Production Split Module
 #######################
 
 The Production Split module adds on the production a wizard that allows to
 split it.
```

### Comparing `trytond_production_split-7.0.0/trytond_production_split.egg-info/SOURCES.txt` & `trytond_production_split-7.2.0/trytond_production_split.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 production.py
```

