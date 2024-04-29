# Comparing `tmp/trytond_sale_complaint-7.0.0.tar.gz` & `tmp/trytond_sale_complaint-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_complaint-7.0.0.tar", last modified: Mon Oct 30 17:37:20 2023, max compression
+gzip compressed data, was "trytond_sale_complaint-7.2.0.tar", last modified: Mon Apr 29 15:47:30 2024, max compression
```

## Comparing `trytond_sale_complaint-7.0.0.tar` & `trytond_sale_complaint-7.2.0.tar`

### file list

```diff
@@ -1,77 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.257579 trytond_sale_complaint-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:16.000000 trytond_sale_complaint-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1989 2023-10-30 17:11:42.000000 trytond_sale_complaint-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:11:42.000000 trytond_sale_complaint-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4250 2023-10-30 17:37:20.257579 trytond_sale_complaint-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28807 2023-08-13 15:26:13.000000 trytond_sale_complaint-7.0.0/complaint.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13422 2023-10-27 17:38:49.000000 trytond_sale_complaint-7.0.0/complaint.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.254246 trytond_sale_complaint-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:16.000000 trytond_sale_complaint-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:16.000000 trytond_sale_complaint-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.254246 trytond_sale_complaint-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/icons/tryton-sale-complaint.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.250912 trytond_sale_complaint-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     9498 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9554 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8621 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9459 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9570 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8160 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9292 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9987 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8608 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9478 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9471 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8811 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9385 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9692 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8690 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9351 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8999 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9509 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8114 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9503 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9231 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8608 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8049 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8782 2023-10-30 16:47:45.000000 trytond_sale_complaint-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1957 2023-08-13 15:26:13.000000 trytond_sale_complaint-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:37:20.257579 trytond_sale_complaint-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4460 2023-10-27 17:38:49.000000 trytond_sale_complaint-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.250912 trytond_sale_complaint-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8133 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/tests/scenario_sale_complaint.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_complaint-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-10-30 17:11:37.000000 trytond_sale_complaint-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.254246 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4250 2023-10-30 17:37:19.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-10-30 17:37:20.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:37:19.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:37:19.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-10-30 17:37:19.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:37:19.000000 trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:20.254246 trytond_sale_complaint-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/action_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/action_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-08-21 07:34:17.000000 trytond_sale_complaint-7.0.0/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/complaint_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/complaint_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.0.0/view/type_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2024-04-29 15:24:52.000000 trytond_sale_complaint-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:24:51.000000 trytond_sale_complaint-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    28911 2024-04-22 12:14:36.000000 trytond_sale_complaint-7.2.0/complaint.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13169 2024-04-27 16:30:39.000000 trytond_sale_complaint-7.2.0/complaint.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.271671 trytond_sale_complaint-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_complaint-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:24.000000 trytond_sale_complaint-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.271671 trytond_sale_complaint-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/icons/tryton-sale-complaint.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.275005 trytond_sale_complaint-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9498 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9554 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8621 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9459 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9570 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8160 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9292 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9987 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8608 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9478 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9471 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8811 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9385 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9692 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8690 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9351 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8999 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9509 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9589 2024-04-29 13:17:17.000000 trytond_sale_complaint-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9503 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9231 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8608 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8049 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8782 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1957 2024-01-27 09:58:52.000000 trytond_sale_complaint-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4460 2024-03-17 11:01:36.000000 trytond_sale_complaint-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.275005 trytond_sale_complaint-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8106 2024-04-22 12:14:36.000000 trytond_sale_complaint-7.2.0/tests/scenario_sale_complaint.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:24.000000 trytond_sale_complaint-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:24:47.000000 trytond_sale_complaint-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2141 2024-04-29 15:47:30.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.275005 trytond_sale_complaint-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/action_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/action_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-01-27 09:58:52.000000 trytond_sale_complaint-7.2.0/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/complaint_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/complaint_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/type_list.xml
```

### Comparing `trytond_sale_complaint-7.0.0/CHANGELOG` & `trytond_sale_complaint-7.2.0/CHANGELOG`

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

### Comparing `trytond_sale_complaint-7.0.0/LICENSE` & `trytond_sale_complaint-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/PKG-INFO` & `trytond_sale_complaint-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_complaint
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for sale complaint
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
@@ -49,21 +49,21 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Complaint Module
 #####################
 
 The sale_complaint module defines Complaint model.
 
 Complaint
```

### Comparing `trytond_sale_complaint-7.0.0/README.rst` & `trytond_sale_complaint-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/__init__.py` & `trytond_sale_complaint-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/complaint.py` & `trytond_sale_complaint-7.2.0/complaint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from collections import defaultdict
 from decimal import Decimal
 
+from sql import Null
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, Workflow, fields)
 from trytond.model.exceptions import AccessError
 from trytond.modules.company.model import (
@@ -211,15 +212,17 @@
             'account.invoice': ['credit_note'],
             'account.invoice.line': ['credit_note'],
             }
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @staticmethod
     def default_date():
         pool = Pool()
         Date = pool.get('ir.date')
         return Date.today()
```

### Comparing `trytond_sale_complaint-7.0.0/complaint.xml` & `trytond_sale_complaint-7.2.0/complaint.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_sale_complaint-7.0.0/complaint.xml` & `trytond_sale_complaint-7.2.0/complaint.xml`

```diff
@@ -26,22 +26,22 @@
     <record model="ir.action.act_window.view" id="act_type_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="type_view_form"/>
       <field name="act_window" ref="act_type_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_type_form" sequence="10" id="menu_type"/>
     <record model="ir.model.access" id="access_type">
-      <field name="model" search="[('model', '=', 'sale.complaint.type')]"/>
+      <field name="model">sale.complaint.type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_type_admin">
-      <field name="model" search="[('model', '=', 'sale.complaint.type')]"/>
+      <field name="model">sale.complaint.type</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="complaint_view_form">
@@ -135,73 +135,73 @@
     <record model="ir.action.keyword" id="act_complaint_relate_sale_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">sale.sale,-1</field>
       <field name="action" ref="act_complaint_relate_sale"/>
     </record>
     <record model="ir.rule.group" id="rule_group_complaint_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
+      <field name="model">sale.complaint</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_complaint_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_complaint_companies"/>
     </record>
     <record model="ir.model.access" id="access_complaint">
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
+      <field name="model">sale.complaint</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_complaint_sale">
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
+      <field name="model">sale.complaint</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="complaint_cancel_button">
+      <field name="model">sale.complaint</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
     </record>
     <record model="ir.model.button" id="complaint_draft_button">
+      <field name="model">sale.complaint</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
     </record>
     <record model="ir.model.button" id="complaint_wait_button">
+      <field name="model">sale.complaint</field>
       <field name="name">wait</field>
       <field name="string">Wait</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
     </record>
     <record model="ir.model.button" id="complaint_approve_button">
+      <field name="model">sale.complaint</field>
       <field name="name">approve</field>
       <field name="string">Approve</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
     </record>
     <record model="ir.model.button-res.group" id="complaint_approve_button_group_sale_admin">
       <field name="button" ref="complaint_approve_button"/>
       <field name="group" ref="sale.group_sale_admin"/>
     </record>
     <record model="ir.model.button" id="complaint_reject_button">
+      <field name="model">sale.complaint</field>
       <field name="name">reject</field>
       <field name="string">Reject</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
     </record>
     <record model="ir.model.button-res.group" id="complaint_reject_button_group_sale_admin">
       <field name="button" ref="complaint_reject_button"/>
       <field name="group" ref="sale.group_sale_admin"/>
     </record>
     <record model="ir.model.button" id="complaint_do_button">
+      <field name="model">sale.complaint</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'sale.complaint')]"/>
     </record>
     <record model="ir.model.button-res.group" id="complaint_do_button_group_sale_admin">
       <field name="button" ref="complaint_do_button"/>
       <field name="group" ref="sale.group_sale_admin"/>
     </record>
     <record model="ir.ui.view" id="action_view_form">
       <field name="model">sale.complaint.action</field>
```

### Comparing `trytond_sale_complaint-7.0.0/doc/conf.py` & `trytond_sale_complaint-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_complaint-7.0.0/doc/index.rst` & `trytond_sale_complaint-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/icons/LICENSE` & `trytond_sale_complaint-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/bg.po` & `trytond_sale_complaint-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/ca.po` & `trytond_sale_complaint-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/cs.po` & `trytond_sale_complaint-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/de.po` & `trytond_sale_complaint-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/es.po` & `trytond_sale_complaint-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/es_419.po` & `trytond_sale_complaint-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/et.po` & `trytond_sale_complaint-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/fa.po` & `trytond_sale_complaint-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/fi.po` & `trytond_sale_complaint-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/fr.po` & `trytond_sale_complaint-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/hu.po` & `trytond_sale_complaint-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/id.po` & `trytond_sale_complaint-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/it.po` & `trytond_sale_complaint-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/lo.po` & `trytond_sale_complaint-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/lt.po` & `trytond_sale_complaint-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/nl.po` & `trytond_sale_complaint-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/pl.po` & `trytond_sale_complaint-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/pt.po` & `trytond_sale_complaint-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/ro.po` & `trytond_sale_complaint-7.2.0/locale/uk.po`

 * *Files 5% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 
 msgctxt "field:sale.complaint,cancelled_by:"
 msgid "Cancelled By"
 msgstr ""
 
 msgctxt "field:sale.complaint,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.complaint,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:sale.complaint,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:sale.complaint,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.complaint,number:"
 msgid "Number"
-msgstr "Număr"
+msgstr ""
 
 msgctxt "field:sale.complaint,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:sale.complaint,origin_id:"
 msgid "Origin ID"
 msgstr ""
 
 msgctxt "field:sale.complaint,origin_model:"
 msgid "Origin Model"
@@ -64,15 +64,15 @@
 
 msgctxt "field:sale.complaint,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:sale.complaint.action,action:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:sale.complaint.action,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:sale.complaint.action,complaint:"
 msgid "Complaint"
@@ -108,15 +108,15 @@
 
 msgctxt "field:sale.complaint.action,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-account.invoice.line,action:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:sale.complaint.action-account.invoice.line,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt ""
 "field:sale.complaint.action-account.invoice.line,complaint_origin_id:"
@@ -145,15 +145,15 @@
 
 msgctxt "field:sale.complaint.action-account.invoice.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-sale.line,action:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:sale.complaint.action-sale.line,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-sale.line,complaint_origin_id:"
 msgid "Complaint Origin ID"
@@ -185,15 +185,15 @@
 
 msgctxt "field:sale.complaint.type,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:sale.complaint.type,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:sale.configuration,complaint_sequence:"
 msgid "Complaint Sequence"
 msgstr ""
 
 msgctxt "field:sale.configuration.sequence,complaint_sequence:"
 msgid "Complaint Sequence"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_complaint-7.0.0/locale/ru.po` & `trytond_sale_complaint-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/sl.po` & `trytond_sale_complaint-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/tr.po` & `trytond_sale_complaint-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/locale/uk.po` & `trytond_sale_complaint-7.2.0/locale/zh_CN.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:sale.complaint,actions:"
 msgid "Actions"
-msgstr ""
+msgstr "操作"
 
+#, fuzzy
 msgctxt "field:sale.complaint,approved_by:"
 msgid "Approved By"
-msgstr ""
+msgstr "Approved"
 
+#, fuzzy
 msgctxt "field:sale.complaint,cancelled_by:"
 msgid "Cancelled By"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "field:sale.complaint,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.complaint,customer:"
 msgid "Customer"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:sale.complaint,description:"
 msgid "Description"
-msgstr ""
+msgstr "描述"
 
 msgctxt "field:sale.complaint,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:sale.complaint,origin:"
 msgid "Origin"
@@ -46,45 +51,51 @@
 msgid "Origin Model"
 msgstr ""
 
 msgctxt "field:sale.complaint,reference:"
 msgid "Reference"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint,rejected_by:"
 msgid "Rejected By"
-msgstr ""
+msgstr "Reject"
 
+#, fuzzy
 msgctxt "field:sale.complaint,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
 msgctxt "field:sale.complaint,submitted_by:"
 msgid "Submitted By"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint,type:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "field:sale.complaint.action,action:"
 msgid "Action"
-msgstr ""
+msgstr "操作"
 
 msgctxt "field:sale.complaint.action,amount:"
 msgid "Amount"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint.action,complaint:"
 msgid "Complaint"
-msgstr ""
+msgstr "Complaints"
 
+#, fuzzy
 msgctxt "field:sale.complaint.action,complaint_state:"
 msgid "Complaint State"
-msgstr ""
+msgstr "Complaints"
 
 msgctxt "field:sale.complaint.action,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:sale.complaint.action,invoice_lines:"
 msgid "Invoice Lines"
@@ -106,30 +117,33 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.complaint.action,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint.action-account.invoice.line,action:"
 msgid "Action"
-msgstr ""
+msgstr "操作"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,amount:"
 msgid "Amount"
 msgstr ""
 
+#, fuzzy
 msgctxt ""
 "field:sale.complaint.action-account.invoice.line,complaint_origin_id:"
 msgid "Complaint Origin ID"
-msgstr ""
+msgstr "Complaints"
 
+#, fuzzy
 msgctxt "field:sale.complaint.action-account.invoice.line,complaint_state:"
 msgid "Complaint State"
-msgstr ""
+msgstr "Complaints"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-account.invoice.line,line:"
 msgid "Invoice Line"
@@ -143,29 +157,32 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-account.invoice.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint.action-sale.line,action:"
 msgid "Action"
-msgstr ""
+msgstr "操作"
 
 msgctxt "field:sale.complaint.action-sale.line,amount:"
 msgid "Amount"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint.action-sale.line,complaint_origin_id:"
 msgid "Complaint Origin ID"
-msgstr ""
+msgstr "Complaints"
 
+#, fuzzy
 msgctxt "field:sale.complaint.action-sale.line,complaint_state:"
 msgid "Complaint State"
-msgstr ""
+msgstr "Complaints"
 
 msgctxt "field:sale.complaint.action-sale.line,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-sale.line,line:"
 msgid "Sale Line"
@@ -179,17 +196,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.complaint.action-sale.line,unit_price:"
 msgid "Unit Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.complaint.type,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
 msgctxt "field:sale.complaint.type,origin:"
 msgid "Origin"
 msgstr ""
 
 msgctxt "field:sale.configuration,complaint_sequence:"
 msgid "Complaint Sequence"
@@ -221,159 +239,174 @@
 
 msgctxt "help:sale.complaint.action-sale.line,unit_price:"
 msgid "Leave empty for the same price."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_complaint_form"
 msgid "Complaints"
-msgstr ""
+msgstr "Complaints"
 
 msgctxt "model:ir.action,name:act_complaint_relate_party"
 msgid "Customer Complaints"
-msgstr ""
+msgstr "Customer Complaints"
 
 msgctxt "model:ir.action,name:act_complaint_relate_sale"
 msgid "Complaints"
-msgstr ""
+msgstr "Complaints"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_type_form"
 msgid "Types"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_complaint_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "全部"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_complaint_form_domain_approved"
 msgid "Approved"
-msgstr ""
+msgstr "Approved"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_complaint_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_complaint_form_domain_waiting"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
 msgctxt "model:ir.message,text:msg_action_delete_result"
 msgid "You cannot delete action \"%(action)s\" because it has a result."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_complaint_delete_draft"
 msgid "To delete complaint \"%(complaint)s\" you must reset it to draft state."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:complaint_approve_button"
 msgid "Approve"
-msgstr ""
+msgstr "Approve"
 
 msgctxt "model:ir.model.button,string:complaint_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:complaint_do_button"
 msgid "Process"
-msgstr ""
+msgstr "Process"
 
 msgctxt "model:ir.model.button,string:complaint_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:complaint_reject_button"
 msgid "Reject"
-msgstr ""
+msgstr "Reject"
 
 msgctxt "model:ir.model.button,string:complaint_wait_button"
 msgid "Wait"
-msgstr ""
+msgstr "Wait"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_complaint_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Customer Complaint"
 
 msgctxt "model:ir.sequence,name:sequence_complaint"
 msgid "Customer Complaint"
-msgstr ""
+msgstr "Customer Complaint"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_complaint"
 msgid "Customer Complaint"
-msgstr ""
+msgstr "Customer Complaint"
 
 msgctxt "model:ir.ui.menu,name:menu_complaint"
 msgid "Complaints"
-msgstr ""
+msgstr "Complaints"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Customer Complaint"
-msgstr ""
+msgstr "Customer Complaint"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_type"
 msgid "Types"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "model:sale.complaint,name:"
 msgid "Customer Complaint"
-msgstr ""
+msgstr "Customer Complaint"
 
+#, fuzzy
 msgctxt "model:sale.complaint.action,name:"
 msgid "Customer Complaint Action"
-msgstr ""
+msgstr "Customer Complaint"
 
 msgctxt "model:sale.complaint.action-account.invoice.line,name:"
 msgid "Customer Complaint Action - Invoice Line"
 msgstr ""
 
 msgctxt "model:sale.complaint.action-sale.line,name:"
 msgid "Customer Complaint Action - Sale Line"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:sale.complaint.type,name:"
 msgid "Customer Complaint Type"
-msgstr ""
+msgstr "Customer Complaint"
 
+#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Approved"
-msgstr ""
+msgstr "Approve"
 
 msgctxt "selection:sale.complaint,state:"
 msgid "Cancelled"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Done"
-msgstr ""
+msgstr "完成"
 
+#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Rejected"
-msgstr ""
+msgstr "Reject"
 
+#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
 msgctxt "selection:sale.complaint.action,action:"
 msgid "Create Credit Note"
 msgstr ""
 
 msgctxt "selection:sale.complaint.action,action:"
 msgid "Create Sale Return"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:sale.complaint:"
 msgid "Complaint"
-msgstr ""
+msgstr "Complaints"
 
 msgctxt "view:sale.complaint:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:sale.complaint:"
 msgid "Process"
-msgstr ""
+msgstr "Process"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_complaint-7.0.0/locale/zh_CN.po` & `trytond_sale_complaint-7.2.0/locale/ro.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,412 +1,394 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:sale.complaint,actions:"
 msgid "Actions"
-msgstr "操作"
+msgstr "Acțiuni"
 
-#, fuzzy
 msgctxt "field:sale.complaint,approved_by:"
 msgid "Approved By"
-msgstr "Approved"
+msgstr "Aprobat de"
 
-#, fuzzy
 msgctxt "field:sale.complaint,cancelled_by:"
 msgid "Cancelled By"
-msgstr "Cancel"
+msgstr "Anulat de"
 
 msgctxt "field:sale.complaint,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:sale.complaint,customer:"
 msgid "Customer"
-msgstr ""
+msgstr "Client"
 
-#, fuzzy
 msgctxt "field:sale.complaint,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:sale.complaint,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descriere"
 
 msgctxt "field:sale.complaint,number:"
 msgid "Number"
-msgstr ""
+msgstr "Număr"
 
 msgctxt "field:sale.complaint,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
+#, fuzzy
 msgctxt "field:sale.complaint,origin_id:"
 msgid "Origin ID"
-msgstr ""
+msgstr "ID de origine"
 
 msgctxt "field:sale.complaint,origin_model:"
 msgid "Origin Model"
-msgstr ""
+msgstr "Model de origine"
 
 msgctxt "field:sale.complaint,reference:"
 msgid "Reference"
-msgstr ""
+msgstr "Referinţă"
 
-#, fuzzy
 msgctxt "field:sale.complaint,rejected_by:"
 msgid "Rejected By"
-msgstr "Reject"
+msgstr "Respins de"
 
-#, fuzzy
 msgctxt "field:sale.complaint,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
+#, fuzzy
 msgctxt "field:sale.complaint,submitted_by:"
 msgid "Submitted By"
-msgstr ""
+msgstr "Depus de"
 
-#, fuzzy
 msgctxt "field:sale.complaint,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action,action:"
 msgid "Action"
-msgstr "操作"
+msgstr "Acțiune"
 
 msgctxt "field:sale.complaint.action,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action,complaint:"
 msgid "Complaint"
-msgstr "Complaints"
+msgstr "Reclamație"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action,complaint_state:"
 msgid "Complaint State"
-msgstr "Complaints"
+msgstr "Starea Reclamației"
 
 msgctxt "field:sale.complaint.action,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:sale.complaint.action,invoice_lines:"
 msgid "Invoice Lines"
-msgstr ""
+msgstr "Rânduri Factură"
 
 msgctxt "field:sale.complaint.action,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:sale.complaint.action,result:"
 msgid "Result"
-msgstr ""
+msgstr "Rezultat"
 
 msgctxt "field:sale.complaint.action,sale_lines:"
 msgid "Sale Lines"
-msgstr ""
+msgstr "Rânduri de vânzare"
 
 msgctxt "field:sale.complaint.action,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:sale.complaint.action,unit_price:"
 msgid "Unit Price"
-msgstr ""
+msgstr "Preț unitar"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action-account.invoice.line,action:"
 msgid "Action"
-msgstr "操作"
+msgstr "Acțiune"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 #, fuzzy
 msgctxt ""
 "field:sale.complaint.action-account.invoice.line,complaint_origin_id:"
 msgid "Complaint Origin ID"
-msgstr "Complaints"
+msgstr "ID de origine a reclamației"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action-account.invoice.line,complaint_state:"
 msgid "Complaint State"
-msgstr "Complaints"
+msgstr "Starea Reclamației"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,line:"
 msgid "Invoice Line"
-msgstr ""
+msgstr "Rând Factură"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:sale.complaint.action-account.invoice.line,unit_price:"
 msgid "Unit Price"
-msgstr ""
+msgstr "Preț unitar"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action-sale.line,action:"
 msgid "Action"
-msgstr "操作"
+msgstr "Acțiune"
 
 msgctxt "field:sale.complaint.action-sale.line,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 #, fuzzy
 msgctxt "field:sale.complaint.action-sale.line,complaint_origin_id:"
 msgid "Complaint Origin ID"
-msgstr "Complaints"
+msgstr "ID de origine a reclamației"
 
-#, fuzzy
 msgctxt "field:sale.complaint.action-sale.line,complaint_state:"
 msgid "Complaint State"
-msgstr "Complaints"
+msgstr "Starea Reclamației"
 
 msgctxt "field:sale.complaint.action-sale.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:sale.complaint.action-sale.line,line:"
 msgid "Sale Line"
-msgstr ""
+msgstr "Rând de vânzare"
 
 msgctxt "field:sale.complaint.action-sale.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:sale.complaint.action-sale.line,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:sale.complaint.action-sale.line,unit_price:"
 msgid "Unit Price"
-msgstr ""
+msgstr "Preț unitar"
 
-#, fuzzy
 msgctxt "field:sale.complaint.type,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nume"
 
 msgctxt "field:sale.complaint.type,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
+#, fuzzy
 msgctxt "field:sale.configuration,complaint_sequence:"
 msgid "Complaint Sequence"
-msgstr ""
+msgstr "Secvența Reclamației"
 
+#, fuzzy
 msgctxt "field:sale.configuration.sequence,complaint_sequence:"
 msgid "Complaint Sequence"
-msgstr ""
+msgstr "Secvența Reclamației"
 
 msgctxt "help:sale.complaint.action,invoice_lines:"
 msgid "Leave empty for all lines."
-msgstr ""
+msgstr "Lăsați gol pentru toate rândurile."
 
 msgctxt "help:sale.complaint.action,quantity:"
 msgid "Leave empty for the same quantity."
-msgstr ""
+msgstr "Lăsați gol pentru aceeași cantitate."
 
 msgctxt "help:sale.complaint.action,sale_lines:"
 msgid "Leave empty for all lines."
-msgstr ""
+msgstr "Lăsați gol pentru toate rândurile."
 
 msgctxt "help:sale.complaint.action,unit_price:"
 msgid "Leave empty for the same price."
-msgstr ""
+msgstr "Lăsați gol pentru același preț."
 
 msgctxt "help:sale.complaint.action-account.invoice.line,unit_price:"
 msgid "Leave empty for the same price."
-msgstr ""
+msgstr "Lăsați gol pentru același preț."
 
 msgctxt "help:sale.complaint.action-sale.line,unit_price:"
 msgid "Leave empty for the same price."
-msgstr ""
+msgstr "Lăsați gol pentru același preț."
 
 msgctxt "model:ir.action,name:act_complaint_form"
 msgid "Complaints"
-msgstr "Complaints"
+msgstr "Reclamații"
 
 msgctxt "model:ir.action,name:act_complaint_relate_party"
 msgid "Customer Complaints"
-msgstr "Customer Complaints"
+msgstr "Reclamațiile clienților"
 
 msgctxt "model:ir.action,name:act_complaint_relate_sale"
 msgid "Complaints"
-msgstr "Complaints"
+msgstr "Reclamații"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_type_form"
 msgid "Types"
-msgstr "类型"
+msgstr "Tipuri"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_complaint_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Tot"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_complaint_form_domain_approved"
 msgid "Approved"
-msgstr "Approved"
+msgstr "Aprobat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_complaint_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_complaint_form_domain_waiting"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
 msgctxt "model:ir.message,text:msg_action_delete_result"
 msgid "You cannot delete action \"%(action)s\" because it has a result."
-msgstr ""
+msgstr "Nu se poate șterge acțiunea \"%(action)s\" deoarece are un rezultat."
 
 msgctxt "model:ir.message,text:msg_complaint_delete_draft"
 msgid "To delete complaint \"%(complaint)s\" you must reset it to draft state."
 msgstr ""
+"Pentru a șterge reclamația \"%(complaint)s\", trebuie resetată la starea de "
+"ciornă."
 
 msgctxt "model:ir.model.button,string:complaint_approve_button"
 msgid "Approve"
-msgstr "Approve"
+msgstr "Aprobare"
 
 msgctxt "model:ir.model.button,string:complaint_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:complaint_do_button"
 msgid "Process"
-msgstr "Process"
+msgstr "Procesare"
 
 msgctxt "model:ir.model.button,string:complaint_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 msgctxt "model:ir.model.button,string:complaint_reject_button"
 msgid "Reject"
-msgstr "Reject"
+msgstr "Respinge"
 
 msgctxt "model:ir.model.button,string:complaint_wait_button"
 msgid "Wait"
-msgstr "Wait"
+msgstr "Așteptare"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_complaint_companies"
 msgid "User in companies"
-msgstr "Customer Complaint"
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.sequence,name:sequence_complaint"
 msgid "Customer Complaint"
-msgstr "Customer Complaint"
+msgstr "Reclamație client"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_complaint"
 msgid "Customer Complaint"
-msgstr "Customer Complaint"
+msgstr "Reclamație client"
 
 msgctxt "model:ir.ui.menu,name:menu_complaint"
 msgid "Complaints"
-msgstr "Complaints"
+msgstr "Reclamații"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Customer Complaint"
-msgstr "Customer Complaint"
+msgstr "Reclamație client"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_type"
 msgid "Types"
-msgstr "类型"
+msgstr "Tipuri"
 
-#, fuzzy
 msgctxt "model:sale.complaint,name:"
 msgid "Customer Complaint"
-msgstr "Customer Complaint"
+msgstr "Reclamație client"
 
 #, fuzzy
 msgctxt "model:sale.complaint.action,name:"
 msgid "Customer Complaint Action"
-msgstr "Customer Complaint"
+msgstr "Acțiune Reclamație Client"
 
+#, fuzzy
 msgctxt "model:sale.complaint.action-account.invoice.line,name:"
 msgid "Customer Complaint Action - Invoice Line"
-msgstr ""
+msgstr "Acțiune Reclamație Client - Rând Factură"
 
 msgctxt "model:sale.complaint.action-sale.line,name:"
 msgid "Customer Complaint Action - Sale Line"
-msgstr ""
+msgstr "Acțiune Reclamație Client - Rând Vânzare"
 
 #, fuzzy
 msgctxt "model:sale.complaint.type,name:"
 msgid "Customer Complaint Type"
-msgstr "Customer Complaint"
+msgstr "Tip Reclamație Client"
 
-#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Approved"
-msgstr "Approve"
+msgstr "Aprobat"
 
 msgctxt "selection:sale.complaint,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Anulat"
 
-#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Done"
-msgstr "完成"
+msgstr "Terminat"
 
-#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
-#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Rejected"
-msgstr "Reject"
+msgstr "Respins"
 
-#, fuzzy
 msgctxt "selection:sale.complaint,state:"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
+#, fuzzy
 msgctxt "selection:sale.complaint.action,action:"
 msgid "Create Credit Note"
-msgstr ""
+msgstr "Creare notă de credit"
 
+#, fuzzy
 msgctxt "selection:sale.complaint.action,action:"
 msgid "Create Sale Return"
-msgstr ""
+msgstr "Creare retur de vânzare"
 
-#, fuzzy
 msgctxt "view:sale.complaint:"
 msgid "Complaint"
-msgstr "Complaints"
+msgstr "Reclamație"
 
 msgctxt "view:sale.complaint:"
 msgid "Other Info"
-msgstr ""
+msgstr "Alte informații"
 
 #, fuzzy
 msgctxt "view:sale.complaint:"
 msgid "Process"
-msgstr "Process"
+msgstr "Procesare"
```

### Comparing `trytond_sale_complaint-7.0.0/message.xml` & `trytond_sale_complaint-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/sale.py` & `trytond_sale_complaint-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/sale.xml` & `trytond_sale_complaint-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/setup.py` & `trytond_sale_complaint-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/tests/scenario_sale_complaint.rst` & `trytond_sale_complaint-7.2.0/tests/scenario_sale_complaint.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =======================
 Sale Complaint Scenario
 =======================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_complaint')
 
 Create company::
```

### Comparing `trytond_sale_complaint-7.0.0/tox.ini` & `trytond_sale_complaint-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/PKG-INFO` & `trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-complaint
-Version: 7.0.0
+Name: trytond_sale_complaint
+Version: 7.2.0
 Summary: Tryton module for sale complaint
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
@@ -49,21 +49,21 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Complaint Module
 #####################
 
 The sale_complaint module defines Complaint model.
 
 Complaint
```

### Comparing `trytond_sale_complaint-7.0.0/trytond_sale_complaint.egg-info/SOURCES.txt` & `trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_sale_complaint-7.0.0/view/action_form.xml` & `trytond_sale_complaint-7.2.0/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/view/complaint_form.xml` & `trytond_sale_complaint-7.2.0/view/complaint_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.0.0/view/complaint_list.xml` & `trytond_sale_complaint-7.2.0/view/complaint_list.xml`

 * *Files identical despite different names*

