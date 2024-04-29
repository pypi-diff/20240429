# Comparing `tmp/trytond_purchase_request-7.0.0.tar.gz` & `tmp/trytond_purchase_request-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request-7.0.0.tar", last modified: Mon Oct 30 17:35:50 2023, max compression
+gzip compressed data, was "trytond_purchase_request-7.2.0.tar", last modified: Mon Apr 29 15:46:12 2024, max compression
```

## Comparing `trytond_purchase_request-7.0.0.tar` & `trytond_purchase_request-7.2.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:50.863819 trytond_purchase_request-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:23:14.000000 trytond_purchase_request-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-10-30 17:10:49.000000 trytond_purchase_request-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-10-30 17:10:49.000000 trytond_purchase_request-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2023-10-30 17:35:50.863819 trytond_purchase_request-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:50.860486 trytond_purchase_request-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:23:14.000000 trytond_purchase_request-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:14.000000 trytond_purchase_request-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:50.860486 trytond_purchase_request-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6930 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7361 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7439 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7326 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6246 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6482 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7783 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7321 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6883 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6225 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7286 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6898 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6236 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7289 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6479 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7029 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5987 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7053 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6951 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5929 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6954 2023-10-30 16:47:45.000000 trytond_purchase_request-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2023-08-13 15:26:13.000000 trytond_purchase_request-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1086 2023-10-27 17:38:49.000000 trytond_purchase_request-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19555 2023-10-27 17:38:49.000000 trytond_purchase_request-7.0.0/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9390 2023-10-27 17:38:49.000000 trytond_purchase_request-7.0.0/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:35:50.863819 trytond_purchase_request-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4454 2023-10-27 17:38:49.000000 trytond_purchase_request-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:50.860486 trytond_purchase_request-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8543 2023-10-24 07:56:52.000000 trytond_purchase_request-7.0.0/tests/scenario_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_request-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-10-30 17:10:45.000000 trytond_purchase_request-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:50.863819 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2023-10-30 17:35:50.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2031 2023-10-30 17:35:50.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:35:50.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:35:50.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-10-30 17:35:50.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:35:50.000000 trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:35:50.860486 trytond_purchase_request-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_purchase_request-7.0.0/view/handle_purchase_cancellation_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 trytond_purchase_request-7.0.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-01-16 14:00:21.000000 trytond_purchase_request-7.0.0/view/purchase_request_create_purchase_ask_party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-10-24 07:56:52.000000 trytond_purchase_request-7.0.0/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-10-24 07:56:52.000000 trytond_purchase_request-7.0.0/view/purchase_request_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2024-04-29 15:24:00.000000 trytond_purchase_request-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-29 15:24:00.000000 trytond_purchase_request-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.507039 trytond_purchase_request-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_purchase_request-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:21.000000 trytond_purchase_request-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.510372 trytond_purchase_request-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6930 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7361 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7439 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7326 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6246 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6482 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7783 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7321 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6883 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6225 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7286 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6898 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6236 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6479 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7029 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7393 2024-04-29 13:17:17.000000 trytond_purchase_request-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7053 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6954 2024-04-27 16:43:26.000000 trytond_purchase_request-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3855 2024-04-22 12:14:36.000000 trytond_purchase_request-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1086 2024-02-04 18:51:26.000000 trytond_purchase_request-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19606 2024-04-22 12:14:36.000000 trytond_purchase_request-7.2.0/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9229 2024-04-27 16:30:39.000000 trytond_purchase_request-7.2.0/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4454 2024-03-17 11:01:36.000000 trytond_purchase_request-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.510372 trytond_purchase_request-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8378 2024-04-22 12:14:36.000000 trytond_purchase_request-7.2.0/tests/scenario_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-01-29 09:46:02.000000 trytond_purchase_request-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:21.000000 trytond_purchase_request-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2024-04-29 15:23:55.000000 trytond_purchase_request-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:12.000000 trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:12.513705 trytond_purchase_request-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_purchase_request-7.2.0/view/handle_purchase_cancellation_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 trytond_purchase_request-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-01-16 14:00:21.000000 trytond_purchase_request-7.2.0/view/purchase_request_create_purchase_ask_party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-02-04 18:51:26.000000 trytond_purchase_request-7.2.0/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-03-17 13:11:55.000000 trytond_purchase_request-7.2.0/view/purchase_request_tree.xml
```

### Comparing `trytond_purchase_request-7.0.0/CHANGELOG` & `trytond_purchase_request-7.2.0/CHANGELOG`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+Open purchases created from requests
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Rename UOM to Unit for purchase request
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_purchase_request-7.0.0/COPYRIGHT` & `trytond_purchase_request-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Copyright (C) 2016-2023 Nicolas Évrard.
 Copyright (C) 2013-2015 NaN-tic.
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_request-7.0.0/LICENSE` & `trytond_purchase_request-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/PKG-INFO` & `trytond_purchase_request-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for purchase requests
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
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Purchase Request Module
 #######################
 
 The Purchase Request module introduces the concept of Purchase Requests which
 are central points to collect purchase requests generated by other process from
 Tryton.
```

### Comparing `trytond_purchase_request-7.0.0/README.rst` & `trytond_purchase_request-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/__init__.py` & `trytond_purchase_request-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/doc/conf.py` & `trytond_purchase_request-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase_request-7.0.0/doc/index.rst` & `trytond_purchase_request-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/bg.po` & `trytond_purchase_request-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/ca.po` & `trytond_purchase_request-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/cs.po` & `trytond_purchase_request-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/de.po` & `trytond_purchase_request-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/es.po` & `trytond_purchase_request-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/es_419.po` & `trytond_purchase_request-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/et.po` & `trytond_purchase_request-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/fa.po` & `trytond_purchase_request-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/fi.po` & `trytond_purchase_request-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/fr.po` & `trytond_purchase_request-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/hu.po` & `trytond_purchase_request-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/id.po` & `trytond_purchase_request-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/it.po` & `trytond_purchase_request-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/lo.po` & `trytond_purchase_request-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/lt.po` & `trytond_purchase_request-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/nl.po` & `trytond_purchase_request-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/pl.po` & `trytond_purchase_request-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/pt.po` & `trytond_purchase_request-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/ro.po` & `trytond_purchase_request-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:purchase.line,requests:"
 msgid "Requests"
 msgstr ""
 
 msgctxt "field:purchase.request,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.request,computed_quantity:"
 msgid "Computed Quantity"
 msgstr ""
 
 msgctxt "field:purchase.request,computed_unit:"
 msgid "Computed Unit"
@@ -20,31 +20,31 @@
 
 msgctxt "field:purchase.request,default_uom:"
 msgid "Default UoM"
 msgstr ""
 
 msgctxt "field:purchase.request,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:purchase.request,exception_ignored:"
 msgid "Ignored Exception"
 msgstr ""
 
 msgctxt "field:purchase.request,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:purchase.request,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:purchase.request,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:purchase.request,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
 msgctxt "field:purchase.request,purchase:"
 msgid "Purchase"
@@ -92,27 +92,27 @@
 
 msgctxt "field:purchase.request,warehouse_required:"
 msgid "Warehouse Required"
 msgstr ""
 
 msgctxt "field:purchase.request.create_purchase.ask_party,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.request.create_purchase.ask_party,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:purchase.request.create_purchase.ask_party,party:"
 msgid "Supplier"
 msgstr ""
 
 msgctxt "field:purchase.request.create_purchase.ask_party,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "help:purchase.request,default_uom:"
 msgid "The default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.request,product_uom_category:"
 msgid "The category of Unit of Measure for the product."
```

### Comparing `trytond_purchase_request-7.0.0/locale/ru.po` & `trytond_purchase_request-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/sl.po` & `trytond_purchase_request-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/tr.po` & `trytond_purchase_request-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/locale/uk.po` & `trytond_purchase_request-7.2.0/locale/ro.po`

 * *Files 26% similar despite different names*

```diff
@@ -4,257 +4,280 @@
 
 msgctxt "field:purchase.line,requests:"
 msgid "Requests"
 msgstr ""
 
 msgctxt "field:purchase.request,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:purchase.request,computed_quantity:"
 msgid "Computed Quantity"
-msgstr ""
+msgstr "Cantitate calculată"
 
 msgctxt "field:purchase.request,computed_unit:"
 msgid "Computed Unit"
-msgstr ""
+msgstr "Unitate calculată"
 
 msgctxt "field:purchase.request,default_uom:"
 msgid "Default UoM"
-msgstr ""
+msgstr "UM Implicită"
 
 msgctxt "field:purchase.request,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:purchase.request,exception_ignored:"
 msgid "Ignored Exception"
-msgstr ""
+msgstr "Excepție ignorată"
 
 msgctxt "field:purchase.request,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:purchase.request,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:purchase.request,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:purchase.request,product_uom_category:"
 msgid "Product UoM Category"
-msgstr ""
+msgstr "Categorie UM Produs"
 
 msgctxt "field:purchase.request,purchase:"
 msgid "Purchase"
-msgstr ""
+msgstr "Achiziție"
 
 msgctxt "field:purchase.request,purchase_date:"
 msgid "Best Purchase Date"
-msgstr ""
+msgstr "Cea mai bună dată de achiziție"
 
 msgctxt "field:purchase.request,purchase_line:"
 msgid "Purchase Line"
-msgstr ""
+msgstr "Rând de Achiziție"
 
 msgctxt "field:purchase.request,purchased_by:"
 msgid "Purchased By"
-msgstr ""
+msgstr "Achiziționat de"
 
 msgctxt "field:purchase.request,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:purchase.request,state:"
 msgid "State"
-msgstr ""
+msgstr "Stare"
 
 msgctxt "field:purchase.request,stock_level:"
 msgid "Stock at Supply Date"
-msgstr ""
+msgstr "Stoc la data aprovizionării"
 
 msgctxt "field:purchase.request,summary:"
 msgid "Summary"
-msgstr ""
+msgstr "Sumar"
 
 msgctxt "field:purchase.request,supply_date:"
 msgid "Expected Supply Date"
-msgstr ""
+msgstr "Data estimată de aprovizionare"
 
 msgctxt "field:purchase.request,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:purchase.request,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Depozit"
 
 msgctxt "field:purchase.request,warehouse_required:"
 msgid "Warehouse Required"
-msgstr ""
+msgstr "Depozit necesar"
 
 msgctxt "field:purchase.request.create_purchase.ask_party,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:purchase.request.create_purchase.ask_party,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:purchase.request.create_purchase.ask_party,party:"
 msgid "Supplier"
-msgstr ""
+msgstr "Furnizor"
 
 msgctxt "field:purchase.request.create_purchase.ask_party,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "help:purchase.request,default_uom:"
 msgid "The default Unit of Measure."
-msgstr ""
+msgstr "Unitatea de măsură implicită."
 
 msgctxt "help:purchase.request,product_uom_category:"
 msgid "The category of Unit of Measure for the product."
-msgstr ""
+msgstr "Categoria de unitate de măsură pentru produs."
 
 msgctxt "model:ir.action,name:act_open_purchase_form"
 msgid "Purchases"
-msgstr ""
+msgstr "Achiziții"
 
 msgctxt "model:ir.action,name:act_open_request_form"
 msgid "Purchase Requests"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_create_purchase"
 msgid "Create Purchase"
-msgstr ""
+msgstr "Creare achiziție"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_purchase_cancellation_handle_exception"
 msgid "Handle Purchase Cancellation"
-msgstr ""
+msgstr "Gestionați anularea achiziției"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_request_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_request_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Ciornă"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_request_form_domain_exception"
 msgid "Exception"
-msgstr ""
+msgstr "Excepție"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_purchase_delete_request"
 msgid ""
 "You cannot delete purchase \"%(purchase)s\" because it is linked to purchase"
 " requests."
 msgstr ""
+"Nu puteți șterge achiziția \"%(purchase)s\" deoarece este legată de "
+"solicitările de achiziție."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_purchase_request_warehouse"
 msgid ""
 "Warehouse \"%(purchase_warehouse)s\" on purchase \"%(purchase)s\" is "
 "different to warehouse \"%(request_warehouse)s\" on linked purchase request "
 "\"%(request)s\"."
 msgstr ""
+"Depozitul \"%(purchase_warehouse)s\" la achiziția \"%(purchase)s\" este "
+"diferit de depozitul \"%(request_warehouse)s\" la cererea de achiziție "
+"aferentă \"%(request)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_request_delete_purchased"
 msgid ""
 "You cannot delete purchase request \"%(request)s\" because it is purchased."
 msgstr ""
+"Nu puteți șterge solicitarea de achiziție \"%(request)s\" deoarece este "
+"achiziționată."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_request_no_create"
 msgid "Purchase requests can only be created by the system."
-msgstr ""
+msgstr "Solicitările de achiziție pot fi create numai de sistem."
 
+#, fuzzy
 msgctxt ""
 "model:ir.model.button,string:purchase_hande_purchase_cancellation_exception_button"
 msgid "Handle Purchase Cancellation"
-msgstr ""
+msgstr "Gestionați anularea achiziției"
 
 msgctxt "model:ir.rule.group,name:rule_group_purchase_request_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_request_form"
 msgid "Purchase Requests"
-msgstr ""
+msgstr "Cereri de achiziție"
 
+#, fuzzy
 msgctxt "model:purchase.request,name:"
 msgid "Purchase Request"
-msgstr ""
+msgstr "Cerere de achiziție"
 
 msgctxt "model:purchase.request.create_purchase.ask_party,name:"
 msgid "Create Purchase Ask Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:purchase.request.handle.purchase.cancellation.start,name:"
 msgid "Handle Purchase Cancellation Exception - Start"
-msgstr ""
+msgstr "Gestionare excepție de anulare a achiziției - Start"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_purchase_request"
 msgid "Purchase Request"
-msgstr ""
+msgstr "Cerere de achiziție"
 
 msgctxt "selection:purchase.request,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Anulat"
 
 msgctxt "selection:purchase.request,state:"
 msgid "Done"
-msgstr ""
+msgstr "Terminat"
 
 msgctxt "selection:purchase.request,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Ciornă"
 
 msgctxt "selection:purchase.request,state:"
 msgid "Exception"
-msgstr ""
+msgstr "Excepție"
 
+#, fuzzy
 msgctxt "selection:purchase.request,state:"
 msgid "Purchased"
-msgstr ""
+msgstr "Achiziționat"
 
+#, fuzzy
 msgctxt "view:purchase.request.handle.purchase.cancellation.start:"
 msgid "Do you want to cancel the request or to reset it to draft?"
-msgstr ""
+msgstr "Doriți să anulați solicitarea sau să o resetați la ciornă?"
 
 msgctxt "view:purchase.request:"
 msgid "Product Info"
-msgstr ""
+msgstr "Informații produs"
 
+#, fuzzy
 msgctxt "view:purchase.request:"
 msgid "Supply Info"
-msgstr ""
+msgstr "Informații de aprovizionare"
 
 msgctxt "wizard_button:purchase.request.create_purchase,ask_party,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:purchase.request.create_purchase,ask_party,start:"
 msgid "Continue"
-msgstr ""
+msgstr "Continuare"
 
+#, fuzzy
 msgctxt ""
 "wizard_button:purchase.request.handle.purchase.cancellation,start,cancel_request:"
 msgid "Cancel Request"
-msgstr ""
+msgstr "Anulare solicitare"
 
 msgctxt ""
 "wizard_button:purchase.request.handle.purchase.cancellation,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
+#, fuzzy
 msgctxt ""
 "wizard_button:purchase.request.handle.purchase.cancellation,start,reset:"
 msgid "Reset to draft"
-msgstr ""
+msgstr "Resetare la ciornă"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_purchase_request-7.0.0/locale/zh_CN.po` & `trytond_purchase_request-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/message.xml` & `trytond_purchase_request-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/purchase.py` & `trytond_purchase_request-7.2.0/purchase.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,20 @@
     # Must be run after the purchase transition
     # such as purchase has the proper state
     @wraps(func)
     def wrapper(cls, purchases):
         pool = Pool()
         Request = pool.get('purchase.request')
         func(cls, purchases)
-        requests = [r for p in purchases for l in p.lines for r in l.requests]
-        Request.update_state(requests)
+        with without_check_access():
+            requests = [
+                r for p in cls.browse(purchases)
+                for l in p.lines
+                for r in l.requests]
+            Request.update_state(requests)
     return wrapper
 
 
 class Purchase(metaclass=PoolMeta):
     __name__ = 'purchase.purchase'
 
     @classmethod
@@ -73,18 +77,18 @@
     @ModelView.button
     @process_request
     @Workflow.transition('cancelled')
     def cancel(cls, purchases):
         super(Purchase, cls).cancel(purchases)
 
     @classmethod
+    @ModelView.button
     @process_request
-    @Workflow.transition('done')
-    def do(cls, purchases):
-        super(Purchase, cls).do(purchases)
+    def process(cls, purchases):
+        super().process(purchases)
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'purchase.line'
 
     requests = fields.One2Many(
         'purchase.request', 'purchase_line', "Requests", readonly=True,
```

### Comparing `trytond_purchase_request-7.0.0/purchase.xml` & `trytond_purchase_request-7.2.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/purchase_request.py` & `trytond_purchase_request-7.2.0/purchase_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from trytond.modules.company.model import (
     employee_field, reset_employee, set_employee)
 from trytond.modules.product import round_price
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
 from trytond.tools import firstline, sortable_values
 from trytond.transaction import Transaction
-from trytond.wizard import Button, StateTransition, StateView, Wizard
+from trytond.wizard import (
+    Button, StateAction, StateTransition, StateView, Wizard)
 
 STATES = {
     'readonly': Eval('state') != 'draft',
     }
 
 
 class PurchaseRequest(ModelSQL, ModelView):
@@ -196,18 +197,15 @@
 
     @classmethod
     def search_purchase(cls, name, clause):
         return [('purchase_line.' + clause[0],) + tuple(clause[1:])]
 
     @property
     def currency(self):
-        currency = self.company.currency
-        if self.party and self.party.supplier_currency:
-            currency = self.party.supplier_currency
-        return currency
+        return
 
     @classmethod
     def default_state(cls):
         return 'draft'
 
     def get_state(self):
         if self.purchase_line:
@@ -355,14 +353,15 @@
     __name__ = 'purchase.request.create_purchase'
     start = StateTransition()
     ask_party = StateView('purchase.request.create_purchase.ask_party',
         'purchase_request.purchase_request_create_purchase_ask_party', [
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('Continue', 'start', 'tryton-forward', default=True),
             ])
+    open_ = StateAction('purchase.act_purchase_form')
 
     def default_ask_party(self, fields):
         for request in self.records:
             if request.purchase_line:
                 continue
             if not request.party:
                 break
@@ -377,18 +376,16 @@
         '''
         The key to group lines by purchases
         A list of key-value as tuples of the purchase
         '''
         return (
             ('company', request.company),
             ('party', request.party),
-            ('payment_term', request.party.supplier_payment_term),
             ('warehouse', request.warehouse),
             ('currency', request.currency),
-            ('invoice_address', request.party.address_get(type='invoice')),
             )
 
     def _group_purchase_line_key(self, request):
         '''
         The key to group requests by lines
         A list of key-value as tuples of the purchase line
         '''
@@ -459,27 +456,28 @@
             except ValueError:
                 purchase_date = today
             if purchase_date < today:
                 purchase_date = today
             purchase = Purchase(purchase_date=purchase_date)
             for f, v in key.items():
                 setattr(purchase, f, v)
+            purchase.on_change_party()
             purchases.append(purchase)
             for line_key, line_requests in groupby(
                     grouped_requests, key=self._group_purchase_line_key):
                 line_requests = list(line_requests)
                 line = self.compute_purchase_line(
                     line_key, line_requests, purchase)
                 line.purchase = purchase
                 line.requests = line_requests
                 lines.append(line)
         Purchase.save(purchases)
         Line.save(lines)
         Request.set_purchased(requests)
-        return 'end'
+        return 'open_'
 
     @classmethod
     def compute_purchase_line(cls, key, requests, purchase):
         pool = Pool()
         Line = pool.get('purchase.line')
 
         line = Line()
@@ -504,14 +502,22 @@
         Uom = pool.get('product.uom')
         unit = line.unit
         compute_qty = Uom.compute_qty
         return sum(
             compute_qty(r.unit, r.quantity, unit, round=False)
             for r in requests)
 
+    def do_open_(self, action):
+        purchase_ids = list({
+                r.purchase.id for r in self.records if r.purchase})
+        action['domains'] = []
+        return action, {
+            'res_id': purchase_ids,
+            }
+
     def end(self):
         return 'reload'
 
 
 class HandlePurchaseCancellationException(Wizard):
     'Handle Purchase Cancellation Exception'
     __name__ = 'purchase.request.handle.purchase.cancellation'
```

### Comparing `trytond_purchase_request-7.0.0/purchase_request.xml` & `trytond_purchase_request-7.2.0/purchase_request.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_purchase_request-7.0.0/purchase_request.xml` & `trytond_purchase_request-7.2.0/purchase_request.xml`

```diff
@@ -85,65 +85,65 @@
     </record>
     <record model="ir.action.wizard" id="wizard_purchase_cancellation_handle_exception">
       <field name="name">Handle Purchase Cancellation</field>
       <field name="wiz_name">purchase.request.handle.purchase.cancellation</field>
       <field name="model">purchase.request</field>
     </record>
     <record model="ir.model.button" id="purchase_hande_purchase_cancellation_exception_button">
+      <field name="model">purchase.request</field>
       <field name="name">handle_purchase_cancellation_exception</field>
       <field name="string">Handle Purchase Cancellation</field>
-      <field name="model" search="[('model', '=', 'purchase.request')]"/>
     </record>
     <record model="ir.action.keyword" id="wizard_purchase_cancellation_handle_exception_keyword">
       <field name="action" ref="wizard_purchase_cancellation_handle_exception"/>
       <field name="keyword">form_action</field>
       <field name="model">purchase.request,-1</field>
     </record>
     <record model="ir.rule.group" id="rule_group_purchase_request_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.request')]"/>
+      <field name="model">purchase.request</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_purchase_request_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_purchase_request_companies"/>
     </record>
     <record model="ir.model.access" id="access_purchase_request">
-      <field name="model" search="[('model', '=', 'purchase.request')]"/>
+      <field name="model">purchase.request</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_request_purchase">
-      <field name="model" search="[('model', '=', 'purchase.request')]"/>
+      <field name="model">purchase.request</field>
       <field name="group" ref="purchase.group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_request_admin">
-      <field name="model" search="[('model', '=', 'purchase.request')]"/>
+      <field name="model">purchase.request</field>
       <field name="group" ref="group_purchase_request"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_purchase_purchase_request">
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="model">purchase.purchase</field>
       <field name="group" ref="group_purchase_request"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_line_purchase_request">
-      <field name="model" search="[('model', '=', 'purchase.line')]"/>
+      <field name="model">purchase.line</field>
       <field name="group" ref="group_purchase_request"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.act_window" id="act_open_purchase_form">
```

### Comparing `trytond_purchase_request-7.0.0/setup.py` & `trytond_purchase_request-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/tests/scenario_purchase_request.rst` & `trytond_purchase_request-7.2.0/tests/scenario_purchase_request.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Purchase Request Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import (create_chart,
-    ...     get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['purchase_request', 'stock_supply'])
 
@@ -153,30 +152,27 @@
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
 
 There is now a draft purchase request::
 
     >>> set_user(purchase_user)
     >>> pr, = PurchaseRequest.find([('state', '=', 'draft')])
-    >>> pr.product == product
-    True
+    >>> assertEqual(pr.product, product)
     >>> pr.quantity
     1.0
 
 Create the purchase then cancel it::
 
     >>> create_purchase = Wizard('purchase.request.create_purchase',
     ...     [pr])
     >>> create_purchase.form.party = supplier
     >>> create_purchase.execute('start')
     >>> pr.state
     'purchased'
-
-    >>> Purchase = Model.get('purchase.purchase')
-    >>> purchase, = Purchase.find()
+    >>> (purchase,), = create_purchase.actions
     >>> purchase.click('cancel')
     >>> pr.reload()
     >>> pr.state
     'exception'
 
 Handle the exception::
 
@@ -188,16 +184,15 @@
 
 Recreate a purchase and cancel it again::
 
     >>> create_purchase = Wizard('purchase.request.create_purchase',
     ...     [pr])
     >>> pr.state
     'purchased'
-
-    >>> purchase, = Purchase.find([('state', '=', 'draft')])
+    >>> (purchase,), = create_purchase.actions
     >>> purchase.click('cancel')
     >>> pr.reload()
     >>> pr.state
     'exception'
 
 Handle again the exception::
 
@@ -236,26 +231,22 @@
 Create the purchase with a unique line::
 
     >>> create_purchase = Wizard('purchase.request.create_purchase', prs)
     >>> create_purchase.form.party = supplier
     >>> create_purchase.execute('start')
     >>> pr.state
     'purchased'
-
-    >>> Purchase = Model.get('purchase.purchase')
-    >>> purchase, = Purchase.find([('state', '=', 'draft')])
+    >>> (purchase,), = create_purchase.actions
     >>> len(purchase.lines)
     1
     >>> line, = purchase.lines
-    >>> line.product == product
-    True
+    >>> assertEqual(line.product, product)
     >>> line.quantity
     2.0
-    >>> line.unit == unit
-    True
+    >>> assertEqual(line.unit, unit)
 
 Create a purchase request without product::
 
     >>> set_user(0)  # root
     >>> pr_id, = PurchaseRequest.create([{
     ...             'description': "Custom product",
     ...             'quantity': 1,
@@ -280,11 +271,11 @@
     1.0
     >>> pr.purchase_line.unit
     >>> pr.purchase_line.unit_price
     Decimal('0.0000')
 
 It's not possible to delete a purchase linked to a purchase_request::
 
-    >>> pr.purchase_line.purchase.delete()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> pr.purchase_line.purchase.delete()
     Traceback (most recent call last):
         ...
     AccessError: ...
```

### Comparing `trytond_purchase_request-7.0.0/tox.ini` & `trytond_purchase_request-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/PKG-INFO` & `trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-request
-Version: 7.0.0
+Name: trytond_purchase_request
+Version: 7.2.0
 Summary: Tryton module for purchase requests
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
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Purchase Request Module
 #######################
 
 The Purchase Request module introduces the concept of Purchase Requests which
 are central points to collect purchase requests generated by other process from
 Tryton.
```

### Comparing `trytond_purchase_request-7.0.0/trytond_purchase_request.egg-info/SOURCES.txt` & `trytond_purchase_request-7.2.0/trytond_purchase_request.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_purchase_request-7.0.0/view/purchase_request_form.xml` & `trytond_purchase_request-7.2.0/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.0.0/view/purchase_request_tree.xml` & `trytond_purchase_request-7.2.0/view/purchase_request_tree.xml`

 * *Files identical despite different names*

