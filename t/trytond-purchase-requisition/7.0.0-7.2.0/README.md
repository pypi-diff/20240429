# Comparing `tmp/trytond_purchase_requisition-7.0.0.tar.gz` & `tmp/trytond_purchase_requisition-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_requisition-7.0.0.tar", last modified: Mon Oct 30 17:36:08 2023, max compression
+gzip compressed data, was "trytond_purchase_requisition-7.2.0.tar", last modified: Mon Apr 29 15:46:26 2024, max compression
```

## Comparing `trytond_purchase_requisition-7.0.0.tar` & `trytond_purchase_requisition-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:08.500570 trytond_purchase_requisition-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:23:15.000000 trytond_purchase_requisition-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1864 2023-10-30 17:10:59.000000 trytond_purchase_requisition-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 17:10:58.000000 trytond_purchase_requisition-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_requisition-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2023-10-30 17:36:08.500570 trytond_purchase_requisition-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-10-27 17:38:49.000000 trytond_purchase_requisition-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:08.497237 trytond_purchase_requisition-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:23:15.000000 trytond_purchase_requisition-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:15.000000 trytond_purchase_requisition-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-10-27 17:38:49.000000 trytond_purchase_requisition-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:08.497237 trytond_purchase_requisition-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6834 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6970 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6840 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6050 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6555 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7142 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7009 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6139 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6823 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6522 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6907 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6687 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6871 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6012 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6785 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5890 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2023-10-30 16:47:45.000000 trytond_purchase_requisition-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    25871 2023-10-24 07:56:52.000000 trytond_purchase_requisition-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15898 2023-10-07 15:40:36.000000 trytond_purchase_requisition-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:36:08.500570 trytond_purchase_requisition-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4533 2023-10-27 17:38:49.000000 trytond_purchase_requisition-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:08.497237 trytond_purchase_requisition-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11510 2023-06-10 11:39:56.000000 trytond_purchase_requisition-7.0.0/tests/scenario_purchase_requisition.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_requisition-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:10:54.000000 trytond_purchase_requisition-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:08.500570 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2023-10-30 17:36:07.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2009 2023-10-30 17:36:08.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:36:07.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:36:07.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-10-30 17:36:07.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:36:07.000000 trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:08.497237 trytond_purchase_requisition-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:21.000000 trytond_purchase_requisition-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1837 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/view/purchase_requisition_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/view/purchase_requisition_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/view/purchase_requisition_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/view/purchase_requisition_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.0.0/view/purchase_requisition_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1965 2024-04-29 15:24:10.000000 trytond_purchase_requisition-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-29 15:24:10.000000 trytond_purchase_requisition-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_requisition-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2024-02-04 18:51:26.000000 trytond_purchase_requisition-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.080017 trytond_purchase_requisition-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_purchase_requisition-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:22.000000 trytond_purchase_requisition-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      822 2024-04-29 13:17:17.000000 trytond_purchase_requisition-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.080017 trytond_purchase_requisition-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6834 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6970 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6840 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6050 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6555 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7142 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7009 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6139 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6823 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6522 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6907 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6687 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6871 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6364 2024-04-29 13:17:17.000000 trytond_purchase_requisition-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6785 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5890 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    25975 2024-04-22 12:14:36.000000 trytond_purchase_requisition-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15423 2024-04-27 16:30:39.000000 trytond_purchase_requisition-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4533 2024-03-17 11:01:36.000000 trytond_purchase_requisition-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11285 2024-04-22 12:14:36.000000 trytond_purchase_requisition-7.2.0/tests/scenario_purchase_requisition.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:22.000000 trytond_purchase_requisition-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-29 15:24:06.000000 trytond_purchase_requisition-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1991 2024-04-29 15:46:26.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:21.000000 trytond_purchase_requisition-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1837 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_tree.xml
```

### Comparing `trytond_purchase_requisition-7.0.0/CHANGELOG` & `trytond_purchase_requisition-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_purchase_requisition-7.0.0/COPYRIGHT` & `trytond_purchase_requisition-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/LICENSE` & `trytond_purchase_requisition-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/PKG-INFO` & `trytond_purchase_requisition-7.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_requisition
-Version: 7.0.0
+Version: 7.2.0
 Summary: Allows users to enter requests for product supply (requisition). This will create a "Purchase request" by line which will be treated by the purchasing department.
 Home-page: http://www.tryton.org
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Purchase Requisition Module
 ###########################
 
 The Purchase Requisition module allows users to create their purchase
 requisitions.
 Those requisitions will be approved or rejected by the Approval group.
```

### Comparing `trytond_purchase_requisition-7.0.0/README.rst` & `trytond_purchase_requisition-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/__init__.py` & `trytond_purchase_requisition-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/doc/conf.py` & `trytond_purchase_requisition-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase_requisition-7.0.0/doc/index.rst` & `trytond_purchase_requisition-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/ir.py` & `trytond_purchase_requisition-7.2.0/ir.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,14 @@
         User = pool.get('res.user')
         context = super()._get_context(model_name)
         if model_name == 'purchase.requisition':
             context['employees'] = User.get_employees()
         return context
 
     @classmethod
-    def _get_cache_key(cls, model_name):
+    def _get_cache_key(cls, model_names):
         pool = Pool()
         User = pool.get('res.user')
-        key = super()._get_cache_key(model_name)
-        if model_name == 'purchase.requisition':
+        key = super()._get_cache_key(model_names)
+        if 'purchase.requisition' in model_names:
             key = (*key, User.get_employees())
         return key
```

### Comparing `trytond_purchase_requisition-7.0.0/locale/bg.po` & `trytond_purchase_requisition-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/ca.po` & `trytond_purchase_requisition-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/cs.po` & `trytond_purchase_requisition-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/de.po` & `trytond_purchase_requisition-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/es.po` & `trytond_purchase_requisition-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/es_419.po` & `trytond_purchase_requisition-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/et.po` & `trytond_purchase_requisition-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/fa.po` & `trytond_purchase_requisition-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/fi.po` & `trytond_purchase_requisition-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/fr.po` & `trytond_purchase_requisition-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/hu.po` & `trytond_purchase_requisition-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/id.po` & `trytond_purchase_requisition-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/it.po` & `trytond_purchase_requisition-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/lo.po` & `trytond_purchase_requisition-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/lt.po` & `trytond_purchase_requisition-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/nl.po` & `trytond_purchase_requisition-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/pl.po` & `trytond_purchase_requisition-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/pt.po` & `trytond_purchase_requisition-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/ro.po` & `trytond_purchase_requisition-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 msgctxt "field:purchase.requisition,approved_by:"
 msgid "Approved By"
 msgstr ""
 
 msgctxt "field:purchase.requisition,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.requisition,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:purchase.requisition,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:purchase.requisition,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:purchase.requisition,lines:"
 msgid "Lines"
@@ -60,27 +60,27 @@
 
 msgctxt "field:purchase.requisition,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:purchase.requisition.line,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:purchase.requisition.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:purchase.requisition.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,purchase_requests:"
 msgid "Purchase Request"
@@ -122,18 +122,17 @@
 msgid "Requests"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_purchase_request_form2"
 msgid "Requests"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_requisition_form"
 msgid "Requisitions"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt ""
@@ -179,40 +178,37 @@
 msgid "Reject"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:requisition_wait_button"
 msgid "Wait"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_requisition_admin"
 msgid "Any requisition"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_requisition_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_requisition_employees"
 msgid "Own requisition"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_purchase_requisition"
 msgid "Purchase Requisition"
 msgstr ""
 
 msgctxt "model:ir.sequence.type,name:sequence_type_purchase_requisition"
 msgid "Purchase Requisition"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_requisition_form"
 msgid "Requisitions"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "model:purchase.requisition,name:"
 msgid "Purchase Requisition"
 msgstr ""
 
 msgctxt "model:purchase.requisition.line,name:"
 msgid "Purchase Requisition Line"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_purchase_requisition-7.0.0/locale/ru.po` & `trytond_purchase_requisition-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/sl.po` & `trytond_purchase_requisition-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/tr.po` & `trytond_purchase_requisition-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/locale/uk.po` & `trytond_purchase_requisition-7.2.0/locale/zh_CN.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:purchase.configuration,purchase_requisition_sequence:"
 msgid "Purchase Requisition Sequence"
-msgstr ""
+msgstr "Purchase Requisition"
 
+#, fuzzy
 msgctxt "field:purchase.configuration.sequence,purchase_requisition_sequence:"
 msgid "Purchase Requisition Sequence"
-msgstr ""
+msgstr "Purchase Requisition"
 
+#, fuzzy
 msgctxt "field:purchase.requisition,approved_by:"
 msgid "Approved By"
-msgstr ""
+msgstr "Approve"
 
 msgctxt "field:purchase.requisition,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:purchase.requisition,currency:"
 msgid "Currency"
@@ -34,17 +37,18 @@
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:purchase.requisition,number:"
 msgid "Number"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.requisition,rejected_by:"
 msgid "Rejected By"
-msgstr ""
+msgstr "Reject"
 
 msgctxt "field:purchase.requisition,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:purchase.requisition,supply_date:"
 msgid "Supply Date"
@@ -78,21 +82,23 @@
 msgid "Product"
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.requisition.line,purchase_requests:"
 msgid "Purchase Request"
-msgstr ""
+msgstr "Purchase Requisition"
 
+#, fuzzy
 msgctxt "field:purchase.requisition.line,purchase_requisition_state:"
 msgid "Purchase Requisition State"
-msgstr ""
+msgstr "Purchase Requisition"
 
 msgctxt "field:purchase.requisition.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,requisition:"
 msgid "Requisition"
@@ -116,143 +122,156 @@
 
 msgctxt "help:purchase.requisition.line,product_uom_category:"
 msgid "The category of Unit of Measure for the product."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_purchase_request_form"
 msgid "Requests"
-msgstr ""
+msgstr "Requests"
 
 msgctxt "model:ir.action,name:act_open_purchase_request_form2"
 msgid "Requests"
-msgstr ""
+msgstr "Requests"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_requisition_form"
 msgid "Requisitions"
-msgstr ""
+msgstr "Purchase Requisitions"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_open"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_sent"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_validated"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
 msgctxt "model:ir.message,text:msg_delete_cancel"
 msgid "To delete requisition \"%(requisition)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_warehouse_required"
 msgid "A warehouse must be defined for requisition \"%(requisition)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:requisition_approve_button"
 msgid "Approve"
-msgstr ""
+msgstr "Approve"
 
 msgctxt "model:ir.model.button,string:requisition_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:requisition_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:requisition_process_button"
 msgid "Process"
-msgstr ""
+msgstr "Processing"
 
 msgctxt "model:ir.model.button,string:requisition_reject_button"
 msgid "Reject"
-msgstr ""
+msgstr "Reject"
 
 msgctxt "model:ir.model.button,string:requisition_wait_button"
 msgid "Wait"
-msgstr ""
+msgstr "Wait"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_requisition_admin"
 msgid "Any requisition"
-msgstr ""
+msgstr "Purchase Requisitions"
 
 msgctxt "model:ir.rule.group,name:rule_group_requisition_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_requisition_employees"
 msgid "Own requisition"
-msgstr ""
+msgstr "Purchase Requisitions"
 
 msgctxt "model:ir.sequence,name:sequence_purchase_requisition"
 msgid "Purchase Requisition"
-msgstr ""
+msgstr "Purchase Requisition"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_purchase_requisition"
 msgid "Purchase Requisition"
-msgstr ""
+msgstr "Purchase Requisition"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_requisition_form"
 msgid "Requisitions"
-msgstr ""
+msgstr "Purchase Requisitions"
 
+#, fuzzy
 msgctxt "model:purchase.requisition,name:"
 msgid "Purchase Requisition"
-msgstr ""
+msgstr "Purchase Requisition"
 
+#, fuzzy
 msgctxt "model:purchase.requisition.line,name:"
 msgid "Purchase Requisition Line"
-msgstr ""
+msgstr "Purchase Requisition"
 
 msgctxt "model:res.group,name:group_purchase_requisition"
 msgid "Purchase Requisition"
-msgstr ""
+msgstr "Purchase Requisition"
 
 msgctxt "model:res.group,name:group_purchase_requisition_approval"
 msgid "Purchase Requisition Approval"
-msgstr ""
+msgstr "Purchase Requisition Approval"
 
+#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Approved"
-msgstr ""
+msgstr "Approve"
 
+#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "selection:purchase.requisition,state:"
 msgid "Done"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Rejected"
-msgstr ""
+msgstr "Reject"
 
+#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
 msgctxt "view:purchase.requisition.line:"
 msgid "General"
 msgstr ""
 
 msgctxt "view:purchase.requisition:"
 msgid "Other Info"
```

### Comparing `trytond_purchase_requisition-7.0.0/locale/zh_CN.po` & `trytond_purchase_requisition-7.2.0/locale/ro.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,282 +1,266 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:purchase.configuration,purchase_requisition_sequence:"
 msgid "Purchase Requisition Sequence"
-msgstr "Purchase Requisition"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.configuration.sequence,purchase_requisition_sequence:"
 msgid "Purchase Requisition Sequence"
-msgstr "Purchase Requisition"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.requisition,approved_by:"
 msgid "Approved By"
-msgstr "Approve"
+msgstr "Aprobat de"
 
 msgctxt "field:purchase.requisition,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:purchase.requisition,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valută"
 
 msgctxt "field:purchase.requisition,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:purchase.requisition,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Angajat"
 
 msgctxt "field:purchase.requisition,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
 msgctxt "field:purchase.requisition,number:"
 msgid "Number"
-msgstr ""
+msgstr "Număr"
 
-#, fuzzy
 msgctxt "field:purchase.requisition,rejected_by:"
 msgid "Rejected By"
-msgstr "Reject"
+msgstr "Respins de"
 
 msgctxt "field:purchase.requisition,state:"
 msgid "State"
-msgstr ""
+msgstr "Stare"
 
 msgctxt "field:purchase.requisition,supply_date:"
 msgid "Supply Date"
-msgstr ""
+msgstr "Data aprovizionării"
 
 msgctxt "field:purchase.requisition,total_amount:"
 msgid "Total"
-msgstr ""
+msgstr "Total"
 
 msgctxt "field:purchase.requisition,total_amount_cache:"
 msgid "Total Cache"
 msgstr ""
 
 msgctxt "field:purchase.requisition,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Depozit"
 
 msgctxt "field:purchase.requisition.line,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:purchase.requisition.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valută"
 
 msgctxt "field:purchase.requisition.line,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:purchase.requisition.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:purchase.requisition.line,product_uom_category:"
 msgid "Product UoM Category"
-msgstr ""
+msgstr "Categorie UM Produs"
 
-#, fuzzy
 msgctxt "field:purchase.requisition.line,purchase_requests:"
 msgid "Purchase Request"
-msgstr "Purchase Requisition"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.requisition.line,purchase_requisition_state:"
 msgid "Purchase Requisition State"
-msgstr "Purchase Requisition"
+msgstr ""
 
 msgctxt "field:purchase.requisition.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:purchase.requisition.line,requisition:"
 msgid "Requisition"
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,summary:"
 msgid "Summary"
-msgstr ""
+msgstr "Sumar"
 
 msgctxt "field:purchase.requisition.line,supplier:"
 msgid "Supplier"
-msgstr ""
+msgstr "Furnizor"
 
 msgctxt "field:purchase.requisition.line,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:purchase.requisition.line,unit_price:"
 msgid "Unit Price"
-msgstr ""
+msgstr "Preț unitar"
 
 msgctxt "help:purchase.requisition.line,product_uom_category:"
 msgid "The category of Unit of Measure for the product."
-msgstr ""
+msgstr "Categoria de unitate de măsură pentru produs."
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_open_purchase_request_form"
 msgid "Requests"
-msgstr "Requests"
+msgstr "Cereri"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_open_purchase_request_form2"
 msgid "Requests"
-msgstr "Requests"
+msgstr "Cereri"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_requisition_form"
 msgid "Requisitions"
-msgstr "Purchase Requisitions"
+msgstr ""
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_open"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_sent"
 msgid "Processing"
-msgstr "Processing"
+msgstr "În curs de procesare"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_requisition_form_view1_domain_validated"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
 msgctxt "model:ir.message,text:msg_delete_cancel"
 msgid "To delete requisition \"%(requisition)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_warehouse_required"
 msgid "A warehouse must be defined for requisition \"%(requisition)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:requisition_approve_button"
 msgid "Approve"
-msgstr "Approve"
+msgstr "Aprobare"
 
 msgctxt "model:ir.model.button,string:requisition_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:requisition_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:requisition_process_button"
 msgid "Process"
-msgstr "Processing"
+msgstr "Procesare"
 
 msgctxt "model:ir.model.button,string:requisition_reject_button"
 msgid "Reject"
-msgstr "Reject"
+msgstr "Respinge"
 
 msgctxt "model:ir.model.button,string:requisition_wait_button"
 msgid "Wait"
-msgstr "Wait"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_requisition_admin"
 msgid "Any requisition"
-msgstr "Purchase Requisitions"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_requisition_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_requisition_employees"
 msgid "Own requisition"
-msgstr "Purchase Requisitions"
+msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_purchase_requisition"
 msgid "Purchase Requisition"
-msgstr "Purchase Requisition"
+msgstr ""
 
 msgctxt "model:ir.sequence.type,name:sequence_type_purchase_requisition"
 msgid "Purchase Requisition"
-msgstr "Purchase Requisition"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_requisition_form"
 msgid "Requisitions"
-msgstr "Purchase Requisitions"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.requisition,name:"
 msgid "Purchase Requisition"
-msgstr "Purchase Requisition"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.requisition.line,name:"
 msgid "Purchase Requisition Line"
-msgstr "Purchase Requisition"
+msgstr ""
 
 msgctxt "model:res.group,name:group_purchase_requisition"
 msgid "Purchase Requisition"
-msgstr "Purchase Requisition"
+msgstr ""
 
 msgctxt "model:res.group,name:group_purchase_requisition_approval"
 msgid "Purchase Requisition Approval"
-msgstr "Purchase Requisition Approval"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Approved"
-msgstr "Approve"
+msgstr "Aprobat"
 
-#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "Anulat"
 
 msgctxt "selection:purchase.requisition,state:"
 msgid "Done"
-msgstr ""
+msgstr "Terminat"
 
-#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
-#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Processing"
-msgstr "Processing"
+msgstr "În curs de procesare"
 
-#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Rejected"
-msgstr "Reject"
+msgstr "Respins"
 
-#, fuzzy
 msgctxt "selection:purchase.requisition,state:"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
 msgctxt "view:purchase.requisition.line:"
 msgid "General"
-msgstr ""
+msgstr "General"
 
 msgctxt "view:purchase.requisition:"
 msgid "Other Info"
-msgstr ""
+msgstr "Alte informații"
 
 msgctxt "view:purchase.requisition:"
 msgid "Requisition"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_purchase_requisition-7.0.0/message.xml` & `trytond_purchase_requisition-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/purchase.py` & `trytond_purchase_requisition-7.2.0/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from decimal import Decimal
 from itertools import chain
 
+from sql import Null
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import (
     Index, ModelSQL, ModelView, Workflow, fields, sequence_ordered)
 from trytond.model.exceptions import AccessError, RequiredValidationError
 from trytond.modules.company.model import (
@@ -202,15 +203,17 @@
         cursor.execute(*table.update(
                 [table.state], ['cancelled'],
                 where=table.state == 'cancel'))
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_state(cls):
         return 'draft'
 
     @classmethod
     def default_company(cls):
```

### Comparing `trytond_purchase_requisition-7.0.0/purchase.xml` & `trytond_purchase_requisition-7.2.0/purchase.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_purchase_requisition-7.0.0/purchase.xml` & `trytond_purchase_requisition-7.2.0/purchase.xml`

```diff
@@ -131,67 +131,67 @@
       <field name="group" ref="purchase.group_purchase_admin"/>
     </record>
     <record model="ir.sequence" id="sequence_purchase_requisition">
       <field name="name">Purchase Requisition</field>
       <field name="sequence_type" ref="sequence_type_purchase_requisition"/>
     </record>
     <record model="ir.model.button" id="requisition_cancel_button">
+      <field name="model">purchase.requisition</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
     </record>
     <record model="ir.model.button" id="requisition_draft_button">
+      <field name="model">purchase.requisition</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
     </record>
     <record model="ir.model.button" id="requisition_wait_button">
+      <field name="model">purchase.requisition</field>
       <field name="name">wait</field>
       <field name="string">Wait</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
     </record>
     <record model="ir.model.button" id="requisition_approve_button">
+      <field name="model">purchase.requisition</field>
       <field name="name">approve</field>
       <field name="string">Approve</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
     </record>
     <record model="ir.model.button-res.group" id="requisition_approve_button_group_purchase_requisition_approval">
       <field name="button" ref="requisition_approve_button"/>
       <field name="group" ref="group_purchase_requisition_approval"/>
     </record>
     <record model="ir.model.button" id="requisition_process_button">
+      <field name="model">purchase.requisition</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
     </record>
     <record model="ir.model.button-res.group" id="requisition_process_button_group_purchase_requisition_approval">
       <field name="button" ref="requisition_process_button"/>
       <field name="group" ref="group_purchase_requisition_approval"/>
     </record>
     <record model="ir.model.button" id="requisition_reject_button">
+      <field name="model">purchase.requisition</field>
       <field name="name">reject</field>
       <field name="string">Reject</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
     </record>
     <record model="ir.model.button-res.group" id="requisition_reject_button_group_purchase_requisition_approval">
       <field name="button" ref="requisition_reject_button"/>
       <field name="group" ref="group_purchase_requisition_approval"/>
     </record>
     <record model="ir.rule.group" id="rule_group_requisition_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_requisition_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_requisition_companies"/>
     </record>
     <record model="ir.rule.group" id="rule_group_requisition_employees">
       <field name="name">Own requisition</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_requisition_employees">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_requisition_employees"/>
@@ -199,15 +199,15 @@
     <record model="ir.rule.group-res.group" id="rule_group_requisition_employees_group_purchase_requisition">
       <field name="rule_group" ref="rule_group_requisition_employees"/>
       <field name="group" ref="group_purchase_requisition"/>
     </record>
     <!-- Give access to user who could trigger requisition work-flow -->
     <record model="ir.rule.group" id="rule_group_requisition_admin">
       <field name="name">Any requisition</field>
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="global_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_requisition_admin_group_purchase_requisition_approval">
       <field name="rule_group" ref="rule_group_requisition_admin"/>
       <field name="group" ref="group_purchase_requisition_approval"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_requisition_admin_group_purchase_request">
@@ -215,35 +215,35 @@
       <field name="group" ref="purchase_request.group_purchase_request"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_requisition_admin_group_purchase">
       <field name="rule_group" ref="rule_group_requisition_admin"/>
       <field name="group" ref="purchase.group_purchase"/>
     </record>
     <record model="ir.model.access" id="access_requisition">
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_requisition_purchase_requisition">
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="group" ref="group_purchase_requisition"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_requisition_purchase_requisition_approval">
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="group" ref="group_purchase_requisition_approval"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_requisition_purchase_request">
-      <field name="model" search="[('model', '=', 'purchase.requisition')]"/>
+      <field name="model">purchase.requisition</field>
       <field name="group" ref="purchase_request.group_purchase_request"/>
       <field name="perm_read" eval="True"/>
     </record>
     <record model="ir.ui.view" id="purchase_configuration_view_form">
       <field name="model">purchase.configuration</field>
       <field name="name">configuration_form</field>
       <field name="inherit" ref="purchase.purchase_configuration_view_form"/>
```

### Comparing `trytond_purchase_requisition-7.0.0/setup.py` & `trytond_purchase_requisition-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/tests/scenario_purchase_requisition.rst` & `trytond_purchase_requisition-7.2.0/tests/scenario_purchase_requisition.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Purchase Requisition Scenario
 =============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import (create_company,
-    ...     get_company)
-    >>> from trytond.modules.account.tests.tools import (create_chart,
-    ...     get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
 
 Activate purchase_requisition Module::
 
     >>> config = activate_modules(['purchase_requisition'])
 
@@ -46,15 +45,15 @@
     >>> employee_party.save()
     >>> employee = Employee(party=employee_party)
     >>> employee.save()
     >>> requisition_user.employees.append(employee)
     >>> requisition_user.employee = employee
     >>> requisition_user.save()
 
-    >>> party_approval, = Party.duplicate([employee_party],  {
+    >>> party_approval, = Party.duplicate([employee_party], {
     ...         'name': 'Employee Approval',
     ...         })
     >>> employee_approval, = Employee.duplicate([employee], {
     ...         'party': party_approval.id,
     ...         })
     >>> requisition_approval_user, = User.duplicate([requisition_user], {
     ...         'name': 'Requisition Approval',
@@ -130,34 +129,34 @@
     >>> requisition.employee = employee
     >>> requisition.supply_date = today
     >>> requisition_line = requisition.lines.new()
     >>> requisition_line.product = None
     >>> requisition_line.description = None
     >>> requisition_line.supplier = supplier
     >>> requisition_line.unit_price = Decimal('10')
-    >>> requisition.click('wait')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> requisition.click('wait')
     Traceback (most recent call last):
         ...
     RequiredValidationError: ...
 
 Create purchase requisition without product and quantity::
 
     >>> requisition_line.description = 'Description'
-    >>> requisition.click('wait')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> requisition.click('wait')
     Traceback (most recent call last):
         ...
     RequiredValidationError: ...
 
 Create purchase requisition with product goods and without warehouse::
 
     >>> requisition.warehouse = None
     >>> requisition_line.product = product
     >>> requisition_line.description = 'Requisition Test'
     >>> requisition_line.quantity = 2.0
-    >>> requisition.click('wait')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> requisition.click('wait')
     Traceback (most recent call last):
         ...
     RequiredValidationError: ...
 
 Create purchase requisition with supplier and price::
 
     >>> Location = Model.get('stock.location')
@@ -167,24 +166,24 @@
     >>> requisition.state
     'waiting'
 
 Approve workflow by requisition user raise an exception because he's not in
 approval_group::
 
     >>> set_user(requisition_user)
-    >>> requisition.click('approve')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> requisition.click('approve')
     Traceback (most recent call last):
         ...
     AccessButtonError: ...
 
 Approve workflow by purchaser raise an exception because he's not in
 approval_group::
 
     >>> set_user(purchase_user)
-    >>> requisition.click('approve')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> requisition.click('approve')
     Traceback (most recent call last):
         ...
     AccessButtonError: ...
 
 Approve workflow with user in approval_group::
 
     >>> set_user(requisition_approval_user)
@@ -197,26 +196,22 @@
 Create Purchase order from Request::
 
     >>> set_user(purchase_user)
     >>> PurchaseRequest = Model.get('purchase.request')
     >>> pr, = PurchaseRequest.find([('state', '=', 'draft')])
     >>> pr.state
     'draft'
-    >>> pr.product == product
-    True
-    >>> pr.party == supplier
-    True
+    >>> assertEqual(pr.product, product)
+    >>> assertEqual(pr.party, supplier)
     >>> pr.quantity
     2.0
     >>> pr.computed_quantity
     2.0
-    >>> pr.supply_date == today
-    True
-    >>> pr.warehouse == warehouse_loc
-    True
+    >>> assertEqual(pr.supply_date, today)
+    >>> assertEqual(pr.warehouse, warehouse_loc)
     >>> create_purchase = Wizard('purchase.request.create_purchase', [pr])
     >>> pr.state
     'purchased'
     >>> requisition.state
     'processing'
 
 Cancel the purchase order::
@@ -267,15 +262,15 @@
     >>> requisition.reload()
     >>> requisition.state
     'done'
 
 Try to delete requisition done::
 
     >>> set_user(requisition_user)
-    >>> PurchaseRequisition.delete([requisition])  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> PurchaseRequisition.delete([requisition])
     Traceback (most recent call last):
         ...
     AccessError: ...
 
 Delete draft requisition::
 
     >>> requisition = PurchaseRequisition()
@@ -304,18 +299,16 @@
     >>> set_user(requisition_approval_user)
     >>> requisition.click('approve')
 
     >>> set_user(purchase_user)
     >>> pr = PurchaseRequest.find([('state', '=', 'draft')])
     >>> len(pr)
     2
-    >>> pr[0].party == supplier2
-    True
-    >>> pr[1].party == supplier
-    True
+    >>> assertEqual(pr[0].party, supplier2)
+    >>> assertEqual(pr[1].party, supplier)
     >>> create_purchase = Wizard('purchase.request.create_purchase', pr)
     >>> purchase, = Purchase.find([
     ...         ('state', '=', 'draft'),
     ...         ('party', '=', supplier.id),
     ...         ])
     >>> purchase.click('cancel')
     >>> requisition.reload()
```

### Comparing `trytond_purchase_requisition-7.0.0/tox.ini` & `trytond_purchase_requisition-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/PKG-INFO` & `trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-requisition
-Version: 7.0.0
+Name: trytond_purchase_requisition
+Version: 7.2.0
 Summary: Allows users to enter requests for product supply (requisition). This will create a "Purchase request" by line which will be treated by the purchasing department.
 Home-page: http://www.tryton.org
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Purchase Requisition Module
 ###########################
 
 The Purchase Requisition module allows users to create their purchase
 requisitions.
 Those requisitions will be approved or rejected by the Approval group.
```

### Comparing `trytond_purchase_requisition-7.0.0/trytond_purchase_requisition.egg-info/SOURCES.txt` & `trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/SOURCES.txt`

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
 ir.py
```

### Comparing `trytond_purchase_requisition-7.0.0/view/purchase_requisition_form.xml` & `trytond_purchase_requisition-7.2.0/view/purchase_requisition_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.0.0/view/purchase_requisition_line_form.xml` & `trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_form.xml`

 * *Files identical despite different names*

