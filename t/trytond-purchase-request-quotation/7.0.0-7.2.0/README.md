# Comparing `tmp/trytond_purchase_request_quotation-7.0.0.tar.gz` & `tmp/trytond_purchase_request_quotation-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request_quotation-7.0.0.tar", last modified: Mon Oct 30 17:35:59 2023, max compression
+gzip compressed data, was "trytond_purchase_request_quotation-7.2.0.tar", last modified: Mon Apr 29 15:46:19 2024, max compression
```

## Comparing `trytond_purchase_request_quotation-7.0.0.tar` & `trytond_purchase_request_quotation-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:59.833862 trytond_purchase_request_quotation-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-22 17:23:15.000000 trytond_purchase_request_quotation-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1310 2023-10-30 17:10:53.000000 trytond_purchase_request_quotation-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-10-30 17:10:53.000000 trytond_purchase_request_quotation-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3838 2023-10-30 17:35:59.830529 trytond_purchase_request_quotation-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:59.830529 trytond_purchase_request_quotation-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-22 17:23:15.000000 trytond_purchase_request_quotation-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:15.000000 trytond_purchase_request_quotation-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:59.823862 trytond_purchase_request_quotation-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10041 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9941 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10057 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8380 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9454 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10663 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9878 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8625 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9186 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8876 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9807 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8416 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8364 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2023-10-30 16:47:45.000000 trytond_purchase_request_quotation-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23572 2023-10-24 07:56:52.000000 trytond_purchase_request_quotation-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11230 2023-10-07 15:40:36.000000 trytond_purchase_request_quotation-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2096 2023-10-07 15:40:36.000000 trytond_purchase_request_quotation-7.0.0/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    65125 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/quotation.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:35:59.833862 trytond_purchase_request_quotation-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4539 2023-10-27 17:38:49.000000 trytond_purchase_request_quotation-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:59.827195 trytond_purchase_request_quotation-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7774 2023-06-10 11:39:56.000000 trytond_purchase_request_quotation-7.0.0/tests/scenario_purchase_request_quotation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_request_quotation-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2023-10-30 17:10:50.000000 trytond_purchase_request_quotation-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:59.830529 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3838 2023-10-30 17:35:59.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2517 2023-10-30 17:35:59.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:35:59.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:35:59.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:35:59.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:35:59.000000 trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:59.830529 trytond_purchase_request_quotation-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_create_ask_suppliers_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_create_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      980 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_line_list_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:19.216863 trytond_purchase_request_quotation-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1411 2024-04-29 15:24:05.000000 trytond_purchase_request_quotation-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2024-04-29 15:24:05.000000 trytond_purchase_request_quotation-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3838 2024-04-29 15:46:19.216863 trytond_purchase_request_quotation-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-03-17 10:57:53.000000 trytond_purchase_request_quotation-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:19.210197 trytond_purchase_request_quotation-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_purchase_request_quotation-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-03-17 10:57:53.000000 trytond_purchase_request_quotation-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:22.000000 trytond_purchase_request_quotation-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-03-17 13:11:55.000000 trytond_purchase_request_quotation-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:19.213530 trytond_purchase_request_quotation-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10041 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9941 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10057 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8380 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9454 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10663 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9878 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8625 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9186 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8876 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9807 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8416 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8364 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-27 16:43:26.000000 trytond_purchase_request_quotation-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-03-17 13:11:55.000000 trytond_purchase_request_quotation-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    23676 2024-04-22 12:14:36.000000 trytond_purchase_request_quotation-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10879 2024-04-27 16:30:39.000000 trytond_purchase_request_quotation-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2096 2024-02-04 18:51:26.000000 trytond_purchase_request_quotation-7.2.0/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    65135 2024-04-29 13:17:17.000000 trytond_purchase_request_quotation-7.2.0/quotation.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:19.216863 trytond_purchase_request_quotation-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4539 2024-03-17 11:01:36.000000 trytond_purchase_request_quotation-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:19.213530 trytond_purchase_request_quotation-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7770 2024-04-22 12:14:36.000000 trytond_purchase_request_quotation-7.2.0/tests/scenario_purchase_request_quotation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:22.000000 trytond_purchase_request_quotation-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-29 15:24:01.000000 trytond_purchase_request_quotation-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:19.216863 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3838 2024-04-29 15:46:18.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2499 2024-04-29 15:46:19.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:18.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:46:18.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2024-04-29 15:46:18.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:18.000000 trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:19.216863 trytond_purchase_request_quotation-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_create_ask_suppliers_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_create_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      980 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_line_list_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-02-22 09:41:45.000000 trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_list.xml
```

### Comparing `trytond_purchase_request_quotation-7.0.0/CHANGELOG` & `trytond_purchase_request_quotation-7.2.0/CHANGELOG`

 * *Files 9% similar despite different names*

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
 * Add window tab for quotation and received states of Purchase Requests
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_purchase_request_quotation-7.0.0/COPYRIGHT` & `trytond_purchase_request_quotation-7.2.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Copyright (C) 2017-2021 Maxime Richez
 Copyright (C) 2017-2019 Thierry Bruyere
 Copyright (C) 2017-2021 SALUC SA
-Copyright (C) 2018-2023 Cédric Krier
-Copyright (C) 2018-2023 B2CK
+Copyright (C) 2018-2024 Cédric Krier
+Copyright (C) 2018-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_request_quotation-7.0.0/LICENSE` & `trytond_purchase_request_quotation-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/PKG-INFO` & `trytond_purchase_request_quotation-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request_quotation
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for purchase request quotation
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
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_requisition<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_requisition<7.3,>=7.2; extra == "test"
 
 Purchase Request For Quotation Module
 #####################################
 
 The Purchase Request for Quotation module allows users to ask quotations
 from selected purchase requests to different suppliers.
 Each request will collect quotation information from the supplier.
```

### Comparing `trytond_purchase_request_quotation-7.0.0/README.rst` & `trytond_purchase_request_quotation-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/__init__.py` & `trytond_purchase_request_quotation-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/doc/conf.py` & `trytond_purchase_request_quotation-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase_request_quotation-7.0.0/doc/index.rst` & `trytond_purchase_request_quotation-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/bg.po` & `trytond_purchase_request_quotation-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/ca.po` & `trytond_purchase_request_quotation-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/cs.po` & `trytond_purchase_request_quotation-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/de.po` & `trytond_purchase_request_quotation-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/es.po` & `trytond_purchase_request_quotation-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/es_419.po` & `trytond_purchase_request_quotation-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/et.po` & `trytond_purchase_request_quotation-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/fa.po` & `trytond_purchase_request_quotation-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/fi.po` & `trytond_purchase_request_quotation-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/fr.po` & `trytond_purchase_request_quotation-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/hu.po` & `trytond_purchase_request_quotation-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/id.po` & `trytond_purchase_request_quotation-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/it.po` & `trytond_purchase_request_quotation-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/lo.po` & `trytond_purchase_request_quotation-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/lt.po` & `trytond_purchase_request_quotation-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/nl.po` & `trytond_purchase_request_quotation-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/pl.po` & `trytond_purchase_request_quotation-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/pt.po` & `trytond_purchase_request_quotation-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/ro.po` & `trytond_purchase_request_quotation-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/ru.po` & `trytond_purchase_request_quotation-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/sl.po` & `trytond_purchase_request_quotation-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/tr.po` & `trytond_purchase_request_quotation-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/uk.po` & `trytond_purchase_request_quotation-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/locale/zh_CN.po` & `trytond_purchase_request_quotation-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/purchase.py` & `trytond_purchase_request_quotation-7.2.0/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 from functools import wraps
 from itertools import groupby
 
+from sql import Null
 from sql.conditionals import Case
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Workflow, fields
 from trytond.modules.company import CompanyReport
 from trytond.modules.currency.fields import Monetary
@@ -174,15 +175,17 @@
                     'invisible': ~Eval('state').in_(['sent', 'received']),
                     },
                 })
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def default_state(cls):
```

### Comparing `trytond_purchase_request_quotation-7.0.0/purchase.xml` & `trytond_purchase_request_quotation-7.2.0/purchase.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_purchase_request_quotation-7.0.0/purchase.xml` & `trytond_purchase_request_quotation-7.2.0/purchase.xml`

```diff
@@ -45,32 +45,32 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_purchase_request_quotation_form"/>
     </record>
     <menuitem parent="purchase_request.menu_purchase_request_form" action="act_purchase_request_quotation_form" sequence="10" id="menu_purchase_request_quotation_form"/>
     <record model="ir.model.button" id="quotation_cancel_button">
+      <field name="model">purchase.request.quotation</field>
       <field name="name">cancel</field>
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
     </record>
     <record model="ir.model.button" id="quotation_draft_button">
+      <field name="model">purchase.request.quotation</field>
       <field name="name">draft</field>
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
     </record>
     <record model="ir.model.button" id="quotation_send_button">
+      <field name="model">purchase.request.quotation</field>
       <field name="name">send</field>
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
     </record>
     <record model="ir.model.button" id="quotation_receive_button">
+      <field name="model">purchase.request.quotation</field>
       <field name="name">receive</field>
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
     </record>
     <record model="ir.model.button" id="quotation_reject_button">
+      <field name="model">purchase.request.quotation</field>
       <field name="name">reject</field>
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
     </record>
     <record model="ir.ui.view" id="purchase_request_quotation_create_succeed">
       <field name="model">purchase.request.quotation.create.succeed</field>
       <field name="type">form</field>
       <field name="name">purchase_request_quotation_create_succeed_form</field>
     </record>
     <record model="ir.ui.view" id="purchase_request_quotation_create_ask_suppliers">
@@ -89,38 +89,38 @@
     </record>
     <record model="ir.action-res.group" id="wizard_create_quotation_group_purchase_request">
       <field name="action" ref="wizard_create_quotation"/>
       <field name="group" ref="purchase_request.group_purchase_request"/>
     </record>
     <record model="ir.rule.group" id="rule_group_request_quotation_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
+      <field name="model">purchase.request.quotation</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_request_quotation_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_request_quotation_companies"/>
     </record>
     <record model="ir.model.access" id="access_request_quotation">
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
+      <field name="model">purchase.request.quotation</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_request_quotation_purchase_request">
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
+      <field name="model">purchase.request.quotation</field>
       <field name="group" ref="purchase_request.group_purchase_request"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_request_quotation_purchase">
-      <field name="model" search="[('model', '=', 'purchase.request.quotation')]"/>
+      <field name="model">purchase.request.quotation</field>
       <field name="group" ref="purchase.group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="purchase_request_quotation_line_view_form">
```

### Comparing `trytond_purchase_request_quotation-7.0.0/purchase_request.xml` & `trytond_purchase_request_quotation-7.2.0/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/quotation.fodt` & `trytond_purchase_request_quotation-7.2.0/quotation.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_purchase_request_quotation-7.0.0/quotation.fodt` & `trytond_purchase_request_quotation-7.2.0/quotation.fodt`

```diff
@@ -608,15 +608,15 @@
   <office:master-styles>
     <style:master-page style:name="Standard" style:page-layout-name="pm1">
       <style:header>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -628,15 +628,15 @@
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P4">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P4">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P4">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P4">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
```

### Comparing `trytond_purchase_request_quotation-7.0.0/setup.py` & `trytond_purchase_request_quotation-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/tests/scenario_purchase_request_quotation.rst` & `trytond_purchase_request_quotation-7.2.0/tests/scenario_purchase_request_quotation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Purchase Request For Quotation Scenario
 =======================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+
+    >>> from proteus import Model, Report, Wizard
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
 
 Activate purchase_request_quotation Module::
 
     >>> config = activate_modules(['purchase_request_quotation',
     ...     'purchase_requisition'])
@@ -121,16 +120,15 @@
 
     >>> PurchaseRequest = Model.get('purchase.request')
     >>> purchase_request, = PurchaseRequest.find([('state', '=', 'draft')])
     >>> purchase_request.state
     'draft'
     >>> create_quotation = Wizard(
     ...     'purchase.request.quotation.create', [purchase_request])
-    >>> [supplier] == create_quotation.form.suppliers
-    True
+    >>> assertEqual(create_quotation.form.suppliers, [supplier])
     >>> create_quotation.form.suppliers.append(Party(supplier2.id))
     >>> create_quotation.execute('create_quotations')
     >>> create_quotation.execute('end')
     >>> purchase_request.state
     'quotation'
 
 Check Quotation Lines (1 Request with 2 Suppliers = 2 Quotation Lines)::
@@ -164,21 +162,21 @@
     'Purchase Request Quotation-1'
 
 Suppliers will answer to quotation with their best unit price::
 
     >>> quotation, = Quotation.find([
     ...         ('state', '=', 'sent'),
     ...         ('supplier', '=', supplier.id)
-    ...     ])
+    ...         ])
     >>> quotation.lines[0].unit_price = Decimal('11.000')
     >>> quotation.click('receive')
     >>> quotation, = Quotation.find([
     ...         ('state', '=', 'sent'),
     ...         ('supplier', '=', supplier2.id)
-    ...     ])
+    ...         ])
     >>> quotation.lines[0].unit_price = Decimal('8.000')
     >>> quotation.click('receive')
 
 Purchase Request state is now 'received'::
 
     >>> PurchaseRequest = Model.get('purchase.request')
     >>> prequest, = PurchaseRequest.find([('state', '=', 'received')])
@@ -201,16 +199,15 @@
     >>> create_purchase = Wizard('purchase.request.create_purchase', [prequest])
     >>> prequest.state
     'purchased'
     >>> Purchase = Model.get('purchase.purchase')
     >>> purchase, = Purchase.find([
     ...         ('state', '=', 'draft'),
     ...         ])
-    >>> purchase.party == supplier2
-    True
+    >>> assertEqual(purchase.party, supplier2)
     >>> purchase.lines[0].unit_price
     Decimal('8.000')
 
 Create Purchase Order from Purchase Request having a preferred_quotation_line
 and check if supplier from this quotation was selected::
 
     >>> create_purchase = Wizard('purchase.request.create_purchase',
```

### Comparing `trytond_purchase_request_quotation-7.0.0/tox.ini` & `trytond_purchase_request_quotation-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/PKG-INFO` & `trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-request-quotation
-Version: 7.0.0
+Name: trytond_purchase_request_quotation
+Version: 7.2.0
 Summary: Tryton module for purchase request quotation
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
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_requisition<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_requisition<7.3,>=7.2; extra == "test"
 
 Purchase Request For Quotation Module
 #####################################
 
 The Purchase Request for Quotation module allows users to ask quotations
 from selected purchase requests to different suppliers.
 Each request will collect quotation information from the supplier.
```

### Comparing `trytond_purchase_request_quotation-7.0.0/trytond_purchase_request_quotation.egg-info/SOURCES.txt` & `trytond_purchase_request_quotation-7.2.0/trytond_purchase_request_quotation.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_purchase_request_quotation-7.0.0/view/purchase_request_form.xml` & `trytond_purchase_request_quotation-7.2.0/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_form.xml` & `trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.0.0/view/purchase_request_quotation_line_form.xml` & `trytond_purchase_request_quotation-7.2.0/view/purchase_request_quotation_line_form.xml`

 * *Files identical despite different names*

