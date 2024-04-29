# Comparing `tmp/trytond_product_price_list-7.0.0.tar.gz` & `tmp/trytond_product_price_list-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_price_list-7.0.0.tar", last modified: Mon Oct 30 17:33:13 2023, max compression
+gzip compressed data, was "trytond_product_price_list-7.2.0.tar", last modified: Mon Apr 29 15:43:34 2024, max compression
```

## Comparing `trytond_product_price_list-7.0.0.tar` & `trytond_product_price_list-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:10.000000 trytond_product_price_list-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2914 2023-10-30 17:09:14.000000 trytond_product_price_list-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:09:14.000000 trytond_product_price_list-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2561 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:10.000000 trytond_product_price_list-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:10.000000 trytond_product_price_list-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3465 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4072 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3165 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4190 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4122 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3456 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3360 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3152 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4225 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3964 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3154 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3218 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3461 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3177 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4155 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3357 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3921 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4138 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3399 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3891 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3152 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3167 2023-10-30 16:47:45.000000 trytond_product_price_list-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7283 2023-10-07 15:40:36.000000 trytond_product_price_list-7.0.0/price_list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3923 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/price_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4291 2023-10-27 17:38:49.000000 trytond_product_price_list-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8440 2023-10-07 15:40:36.000000 trytond_product_price_list-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_price_list-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:09:11.000000 trytond_product_price_list-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2561 2023-10-30 17:33:13.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1731 2023-10-30 17:33:13.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:13.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:33:13.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2023-10-30 17:33:13.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:33:13.000000 trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:13.716403 trytond_product_price_list-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-10-07 15:40:36.000000 trytond_product_price_list-7.0.0/view/price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      615 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/view/price_list_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/view/price_list_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/view/price_list_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_product_price_list-7.0.0/view/price_list_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3015 2024-04-29 15:22:09.000000 trytond_product_price_list-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:22:09.000000 trytond_product_price_list-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2561 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.441173 trytond_product_price_list-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_product_price_list-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:16.000000 trytond_product_price_list-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.441173 trytond_product_price_list-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3465 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4072 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3165 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4190 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4122 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3456 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3360 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4178 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4225 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3964 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3154 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3461 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3177 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4155 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3357 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3921 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4169 2024-04-29 13:17:17.000000 trytond_product_price_list-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3399 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3891 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3167 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7283 2024-02-04 18:51:26.000000 trytond_product_price_list-7.2.0/price_list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3854 2024-04-27 16:30:39.000000 trytond_product_price_list-7.2.0/price_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4291 2024-03-17 11:01:36.000000 trytond_product_price_list-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.441173 trytond_product_price_list-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8440 2024-02-04 18:51:26.000000 trytond_product_price_list-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:16.000000 trytond_product_price_list-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-29 15:22:05.000000 trytond_product_price_list-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2561 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1713 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-02-04 18:51:26.000000 trytond_product_price_list-7.2.0/view/price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      615 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_tree.xml
```

### Comparing `trytond_product_price_list-7.0.0/CHANGELOG` & `trytond_product_price_list-7.2.0/CHANGELOG`

 * *Files 11% similar despite different names*

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
 * Define the value of 'unit_price' on price list
 * Remove unit price to compute price list
 * Remove party to compute price list
```

### Comparing `trytond_product_price_list-7.0.0/COPYRIGHT` & `trytond_product_price_list-7.2.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2023 Cédric Krier.
+Copyright (C) 2009-2024 Cédric Krier.
 Copyright (C) 2009-2013 Bertrand Chenal.
-Copyright (C) 2009-2023 B2CK SPRL.
+Copyright (C) 2009-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_price_list-7.0.0/LICENSE` & `trytond_product_price_list-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/PKG-INFO` & `trytond_product_price_list-7.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with price list
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
@@ -49,16 +49,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Price List Module
 #########################
 
 The product price list module provides formula to compute prices per product or
 category.
```

### Comparing `trytond_product_price_list-7.0.0/doc/conf.py` & `trytond_product_price_list-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_price_list-7.0.0/locale/bg.po` & `trytond_product_price_list-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/ca.po` & `trytond_product_price_list-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/cs.po` & `trytond_product_price_list-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/de.po` & `trytond_product_price_list-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/es.po` & `trytond_product_price_list-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/es_419.po` & `trytond_product_price_list-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/et.po` & `trytond_product_price_list-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/fa.po` & `trytond_product_price_list-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/fi.po` & `trytond_product_price_list-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/fr.po` & `trytond_product_price_list-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/hu.po` & `trytond_product_price_list-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/id.po` & `trytond_product_price_list-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/it.po` & `trytond_product_price_list-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/lo.po` & `trytond_product_price_list-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/lt.po` & `trytond_product_price_list-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/nl.po` & `trytond_product_price_list-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/pl.po` & `trytond_product_price_list-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/pt.po` & `trytond_product_price_list-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/ro.po` & `trytond_product_price_list-7.2.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 
 msgctxt "field:product.price_list,lines:"
 msgid "Lines"
 msgstr "Rânduri"
 
 msgctxt "field:product.price_list,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr "Nume"
 
-#, fuzzy
 msgctxt "field:product.price_list,price:"
 msgid "Price"
-msgstr "Listă de prețuri"
+msgstr "Pret"
 
 msgctxt "field:product.price_list,tax_included:"
 msgid "Tax Included"
 msgstr "Taxă inclusă"
 
 msgctxt "field:product.price_list,unit:"
 msgid "Unit"
@@ -65,19 +64,19 @@
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "Identificatorul principal al listei de prețuri."
 
 msgctxt "help:product.price_list,price:"
 msgid "The value used for 'unit_price'."
-msgstr ""
+msgstr "Valoarea utilizata pentru 'unit_price'."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
-msgstr "Verificare dacă rezultatul al formulei include taxe."
+msgstr "Verificare dacă formula rezultatului include taxe."
 
 msgctxt "help:product.price_list,unit:"
 msgid "The unit in which the quantity is expressed."
 msgstr "Unitatea în care este exprimată cantitatea."
 
 msgctxt "help:product.price_list.line,category:"
 msgid "Apply only to products of this category."
@@ -93,15 +92,15 @@
 "Expresia Python care va fi evaluată cu:\n"
 "- unit_price: preț unitar original\n"
 "- cost_price: preț de cost al produsului\n"
 "- list_price: prețul de lista al produsului"
 
 msgctxt "help:product.price_list.line,price_list:"
 msgid "The price list to which the line belongs."
-msgstr "Lista de prețuri la care aparține rândul."
+msgstr "Lista de prețuri de care aparține rândul."
 
 msgctxt "help:product.price_list.line,product:"
 msgid "Apply only to this product."
 msgstr "Aplicare numai acestui produs."
 
 msgctxt "help:product.price_list.line,quantity:"
 msgid "Apply only when quantity is greater."
@@ -112,15 +111,15 @@
 msgstr "Liste de prețuri"
 
 msgctxt "model:ir.message,text:msg_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in price list line \"%(line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Formula nevalidă \"%(formula)s\" din linia listei de prețuri \"%(line)s\" cu"
+"Formula invalidă \"%(formula)s\" din linia listei de prețuri \"%(line)s\" cu"
 " excepția \"%(exception)s\"."
 
 msgctxt "model:ir.rule.group,name:rule_group_price_list_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.ui.menu,name:menu_price_list"
@@ -129,20 +128,20 @@
 
 msgctxt "model:product.price_list,name:"
 msgid "Price List"
 msgstr "Listă de prețuri"
 
 msgctxt "model:product.price_list.line,name:"
 msgid "Price List Line"
-msgstr "Rândul al listei de prețuri"
+msgstr "Rând al listei de prețuri"
 
 msgctxt "selection:product.price_list,price:"
 msgid "Cost Price"
-msgstr ""
+msgstr "Preţ Cost"
 
 msgctxt "selection:product.price_list,price:"
 msgid "List price"
-msgstr ""
+msgstr "Pret de Lista"
 
 msgctxt "selection:product.price_list,unit:"
 msgid "Product Default"
 msgstr "Implicit pentru produs"
```

### Comparing `trytond_product_price_list-7.0.0/locale/ru.po` & `trytond_product_price_list-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/sl.po` & `trytond_product_price_list-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/tr.po` & `trytond_product_price_list-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/uk.po` & `trytond_product_price_list-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/locale/zh_CN.po` & `trytond_product_price_list-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/price_list.py` & `trytond_product_price_list-7.2.0/price_list.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/price_list.xml` & `trytond_product_price_list-7.2.0/price_list.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_product_price_list-7.0.0/price_list.xml` & `trytond_product_price_list-7.2.0/price_list.xml`

```diff
@@ -26,31 +26,31 @@
     <record model="ir.action.act_window.view" id="act_price_list_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="price_list_view_form"/>
       <field name="act_window" ref="act_price_list_form"/>
     </record>
     <menuitem parent="product.menu_main_product" action="act_price_list_form" sequence="30" id="menu_price_list"/>
     <record model="ir.model.access" id="access_price_list">
-      <field name="model" search="[('model', '=', 'product.price_list')]"/>
+      <field name="model">product.price_list</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_price_list_admin">
-      <field name="model" search="[('model', '=', 'product.price_list')]"/>
+      <field name="model">product.price_list</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_price_list_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'product.price_list')]"/>
+      <field name="model">product.price_list</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_price_list_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_price_list_companies"/>
     </record>
     <record model="ir.ui.view" id="price_list_line_view_form">
```

### Comparing `trytond_product_price_list-7.0.0/setup.py` & `trytond_product_price_list-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/tests/test_module.py` & `trytond_product_price_list-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/tox.ini` & `trytond_product_price_list-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/PKG-INFO` & `trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-price-list
-Version: 7.0.0
+Name: trytond_product_price_list
+Version: 7.2.0
 Summary: Tryton module with price list
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
@@ -49,16 +49,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Price List Module
 #########################
 
 The product price list module provides formula to compute prices per product or
 category.
```

### Comparing `trytond_product_price_list-7.0.0/trytond_product_price_list.egg-info/SOURCES.txt` & `trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/SOURCES.txt`

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

### Comparing `trytond_product_price_list-7.0.0/view/price_list_form.xml` & `trytond_product_price_list-7.2.0/view/price_list_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.0.0/view/price_list_line_form.xml` & `trytond_product_price_list-7.2.0/view/price_list_line_form.xml`

 * *Files identical despite different names*

