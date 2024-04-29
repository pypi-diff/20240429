# Comparing `tmp/trytond_product_attribute-7.0.0.tar.gz` & `tmp/trytond_product_attribute-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_attribute-7.0.0.tar", last modified: Mon Oct 30 17:32:08 2023, max compression
+gzip compressed data, was "trytond_product_attribute-7.2.0.tar", last modified: Mon Apr 29 15:42:28 2024, max compression
```

## Comparing `trytond_product_attribute-7.0.0.tar` & `trytond_product_attribute-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:08.446092 trytond_product_attribute-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-22 17:23:08.000000 trytond_product_attribute-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-10-30 17:08:24.000000 trytond_product_attribute-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:08:24.000000 trytond_product_attribute-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_attribute-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2023-10-30 17:32:08.446092 trytond_product_attribute-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:08.446092 trytond_product_attribute-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-22 17:23:08.000000 trytond_product_attribute-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:08.000000 trytond_product_attribute-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:08.442758 trytond_product_attribute-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2652 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2673 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2708 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2293 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2923 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2721 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2153 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2661 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2737 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2635 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2683 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-10-30 16:47:45.000000 trytond_product_attribute-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2404 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2023-10-28 12:11:23.000000 trytond_product_attribute-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6051 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:32:08.446092 trytond_product_attribute-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4307 2023-10-27 17:38:49.000000 trytond_product_attribute-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:08.442758 trytond_product_attribute-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_attribute-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-10-30 17:08:15.000000 trytond_product_attribute-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:08.446092 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2023-10-30 17:32:08.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1842 2023-10-30 17:32:08.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:32:08.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-10-30 17:32:08.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-10-30 17:32:08.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:32:08.000000 trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:08.442758 trytond_product_attribute-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      789 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/attribute_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/attribute_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_product_attribute-7.0.0/view/attribute_set_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/product_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:20.000000 trytond_product_attribute-7.0.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_product_attribute-7.0.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2061 2024-04-29 15:21:19.000000 trytond_product_attribute-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:21:18.000000 trytond_product_attribute-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2745 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.619561 trytond_product_attribute-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_product_attribute-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:14.000000 trytond_product_attribute-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.622894 trytond_product_attribute-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2673 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2708 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2293 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2721 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2153 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2661 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2737 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2635 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2683 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2428 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2404 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2024-04-27 16:43:24.000000 trytond_product_attribute-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5959 2024-04-27 16:30:39.000000 trytond_product_attribute-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4307 2024-03-17 11:01:36.000000 trytond_product_attribute-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.622894 trytond_product_attribute-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:14.000000 trytond_product_attribute-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:21:14.000000 trytond_product_attribute-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2745 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1824 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:28.000000 trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:28.626227 trytond_product_attribute-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      789 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/view/attribute_set_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/product_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:20.000000 trytond_product_attribute-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_product_attribute-7.2.0/view/template_tree.xml
```

### Comparing `trytond_product_attribute-7.0.0/CHANGELOG` & `trytond_product_attribute-7.2.0/CHANGELOG`

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

### Comparing `trytond_product_attribute-7.0.0/LICENSE` & `trytond_product_attribute-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/PKG-INFO` & `trytond_product_attribute-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_attribute
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with product attributes
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
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Attribute Module
 ########################
 
 The Product Attribute module defines the following models: Attribute and
 Attribute Set.
```

### Comparing `trytond_product_attribute-7.0.0/doc/conf.py` & `trytond_product_attribute-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_product_attribute-7.0.0/locale/bg.po` & `trytond_product_attribute-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/ca.po` & `trytond_product_attribute-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/cs.po` & `trytond_product_attribute-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/de.po` & `trytond_product_attribute-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/es.po` & `trytond_product_attribute-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/es_419.po` & `trytond_product_attribute-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/et.po` & `trytond_product_attribute-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/fa.po` & `trytond_product_attribute-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/fi.po` & `trytond_product_attribute-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/fr.po` & `trytond_product_attribute-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/hu.po` & `trytond_product_attribute-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/id.po` & `trytond_product_attribute-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/it.po` & `trytond_product_attribute-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/lo.po` & `trytond_product_attribute-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/lt.po` & `trytond_product_attribute-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/nl.po` & `trytond_product_attribute-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/pl.po` & `trytond_product_attribute-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/pt.po` & `trytond_product_attribute-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/ro.po` & `trytond_product_attribute-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/ru.po` & `trytond_product_attribute-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/sl.po` & `trytond_product_attribute-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/tr.po` & `trytond_product_attribute-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/uk.po` & `trytond_product_attribute-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/locale/zh_CN.po` & `trytond_product_attribute-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/product.py` & `trytond_product_attribute-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/product.xml` & `trytond_product_attribute-7.2.0/product.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_product_attribute-7.0.0/product.xml` & `trytond_product_attribute-7.2.0/product.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_attribute_set_form_view">
       <field name="sequence" eval="20"/>
       <field name="view" ref="attribute_set_view_form"/>
       <field name="act_window" ref="act_attribute_set_form"/>
     </record>
     <menuitem parent="product.menu_configuration" action="act_attribute_set_form" sequence="50" id="menu_attribute_set"/>
     <record model="ir.model.access" id="access_attribute_set">
-      <field name="model" search="[('model', '=', 'product.attribute.set')]"/>
+      <field name="model">product.attribute.set</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_attribute_set_admin">
-      <field name="model" search="[('model', '=', 'product.attribute.set')]"/>
+      <field name="model">product.attribute.set</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="attribute_view_list_simple">
@@ -72,22 +72,22 @@
     <record model="ir.action.act_window.view" id="act_attribute_form_view">
       <field name="sequence" eval="20"/>
       <field name="view" ref="attribute_view_form"/>
       <field name="act_window" ref="act_attribute_form"/>
     </record>
     <menuitem parent="menu_attribute_set" action="act_attribute_form" sequence="10" id="menu_attribute"/>
     <record model="ir.model.access" id="access_attribute">
-      <field name="model" search="[('model', '=', 'product.attribute')]"/>
+      <field name="model">product.attribute</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_attribute_admin">
-      <field name="model" search="[('model', '=', 'product.attribute')]"/>
+      <field name="model">product.attribute</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="template_view_tree">
```

### Comparing `trytond_product_attribute-7.0.0/setup.py` & `trytond_product_attribute-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/tox.ini` & `trytond_product_attribute-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/PKG-INFO` & `trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-attribute
-Version: 7.0.0
+Name: trytond_product_attribute
+Version: 7.2.0
 Summary: Tryton module with product attributes
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
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Attribute Module
 ########################
 
 The Product Attribute module defines the following models: Attribute and
 Attribute Set.
```

### Comparing `trytond_product_attribute-7.0.0/trytond_product_attribute.egg-info/SOURCES.txt` & `trytond_product_attribute-7.2.0/trytond_product_attribute.egg-info/SOURCES.txt`

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
 message.xml
```

### Comparing `trytond_product_attribute-7.0.0/view/attribute_form.xml` & `trytond_product_attribute-7.2.0/view/attribute_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-7.0.0/view/product_form.xml` & `trytond_product_attribute-7.2.0/view/product_form.xml`

 * *Files identical despite different names*
