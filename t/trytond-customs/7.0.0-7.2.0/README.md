# Comparing `tmp/trytond_customs-7.0.0.tar.gz` & `tmp/trytond_customs-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_customs-7.0.0.tar", last modified: Mon Oct 30 17:29:30 2023, max compression
+gzip compressed data, was "trytond_customs-7.2.0.tar", last modified: Mon Apr 29 15:40:02 2024, max compression
```

## Comparing `trytond_customs-7.0.0.tar` & `trytond_customs-7.2.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:30.102003 trytond_customs-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-22 17:23:03.000000 trytond_customs-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-10-30 17:06:10.000000 trytond_customs-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:06:10.000000 trytond_customs-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_customs-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_customs-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3389 2023-10-30 17:29:30.102003 trytond_customs-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_customs-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8820 2023-10-24 07:56:52.000000 trytond_customs-7.0.0/customs.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5966 2023-10-27 17:38:49.000000 trytond_customs-7.0.0/customs.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:30.098670 trytond_customs-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-22 17:23:03.000000 trytond_customs-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:03.000000 trytond_customs-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:30.098670 trytond_customs-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6545 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6605 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5980 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6545 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6704 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6057 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6237 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6616 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6270 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5790 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6536 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6648 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6225 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6590 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6622 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5725 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6611 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6596 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5568 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6060 2023-10-30 16:47:45.000000 trytond_customs-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7102 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1638 2023-01-16 14:00:20.000000 trytond_customs-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:29:30.102003 trytond_customs-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4277 2023-10-27 17:38:49.000000 trytond_customs-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:30.098670 trytond_customs-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_customs-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9525 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_customs-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      121 2023-10-30 17:06:06.000000 trytond_customs-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:30.102003 trytond_customs-7.0.0/trytond_customs.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3389 2023-10-30 17:29:29.000000 trytond_customs-7.0.0/trytond_customs.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1860 2023-10-30 17:29:30.000000 trytond_customs-7.0.0/trytond_customs.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:29.000000 trytond_customs-7.0.0/trytond_customs.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-10-30 17:29:29.000000 trytond_customs-7.0.0/trytond_customs.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_customs-7.0.0/trytond_customs.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      124 2023-10-30 17:29:29.000000 trytond_customs-7.0.0/trytond_customs.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:29:29.000000 trytond_customs-7.0.0/trytond_customs.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:30.098670 trytond_customs-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-01-16 14:00:20.000000 trytond_customs-7.0.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      890 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/view/duty_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/view/duty_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_customs-7.0.0/view/product-tariff_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/view/product-tariff_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/view/product-tariff_code_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/view/tariff_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-08-13 15:26:13.000000 trytond_customs-7.0.0/view/tariff_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_customs-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:02.783375 trytond_customs-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2024-04-29 15:19:26.000000 trytond_customs-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:19:26.000000 trytond_customs-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_customs-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_customs-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3389 2024-04-29 15:40:02.783375 trytond_customs-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_customs-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8820 2024-02-04 18:51:26.000000 trytond_customs-7.2.0/customs.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5874 2024-04-27 16:30:39.000000 trytond_customs-7.2.0/customs.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:02.780042 trytond_customs-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_customs-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:09.000000 trytond_customs-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:02.780042 trytond_customs-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6545 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6605 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5980 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6545 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6704 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6057 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6237 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5895 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6616 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6270 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5790 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6536 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6648 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6225 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6590 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6220 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6622 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6528 2024-04-29 13:17:17.000000 trytond_customs-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6611 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6596 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5895 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5568 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6060 2024-04-27 16:43:24.000000 trytond_customs-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7102 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1638 2023-01-16 14:00:20.000000 trytond_customs-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:02.783375 trytond_customs-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4277 2024-03-17 11:01:36.000000 trytond_customs-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:02.783375 trytond_customs-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_customs-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9525 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:09.000000 trytond_customs-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      121 2024-04-29 15:19:21.000000 trytond_customs-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:02.783375 trytond_customs-7.2.0/trytond_customs.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3389 2024-04-29 15:40:02.000000 trytond_customs-7.2.0/trytond_customs.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1842 2024-04-29 15:40:02.000000 trytond_customs-7.2.0/trytond_customs.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:02.000000 trytond_customs-7.2.0/trytond_customs.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:40:02.000000 trytond_customs-7.2.0/trytond_customs.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_customs-7.2.0/trytond_customs.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      124 2024-04-29 15:40:02.000000 trytond_customs-7.2.0/trytond_customs.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:02.000000 trytond_customs-7.2.0/trytond_customs.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:02.783375 trytond_customs-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-01-16 14:00:20.000000 trytond_customs-7.2.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      890 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/view/duty_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/view/duty_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_customs-7.2.0/view/product-tariff_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/view/product-tariff_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/view/product-tariff_code_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/view/tariff_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-01-27 09:58:52.000000 trytond_customs-7.2.0/view/tariff_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_customs-7.2.0/view/template_form.xml
```

### Comparing `trytond_customs-7.0.0/CHANGELOG` & `trytond_customs-7.2.0/CHANGELOG`

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
 * Add access rules
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_customs-7.0.0/LICENSE` & `trytond_customs-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/PKG-INFO` & `trytond_customs-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_customs
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for customs
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
@@ -50,18 +50,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Customs Module
 ##############
 
 The customs module allows to define customs duty based on the tariff code.
```

### Comparing `trytond_customs-7.0.0/README.rst` & `trytond_customs-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/customs.py` & `trytond_customs-7.2.0/customs.py`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/customs.xml` & `trytond_customs-7.2.0/customs.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_customs-7.0.0/customs.xml` & `trytond_customs-7.2.0/customs.xml`

```diff
@@ -33,22 +33,22 @@
     <record model="ir.action.act_window.view" id="act_tariff_code_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="tariff_code_view_form"/>
       <field name="act_window" ref="act_tariff_code_form"/>
     </record>
     <menuitem parent="menu_customs" action="act_tariff_code_form" sequence="10" id="menu_tariff_code_form"/>
     <record model="ir.model.access" id="access_tariff_code">
-      <field name="model" search="[('model', '=', 'customs.tariff.code')]"/>
+      <field name="model">customs.tariff.code</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_tariff_code_admin">
-      <field name="model" search="[('model', '=', 'customs.tariff.code')]"/>
+      <field name="model">customs.tariff.code</field>
       <field name="group" ref="group_customs_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="duty_rate_view_form">
@@ -86,22 +86,22 @@
       <field name="name">Export</field>
       <field name="sequence" eval="20"/>
       <field name="domain" eval="[('type', '=', 'export')]" pyson="1"/>
       <field name="act_window" ref="act_duty_rate_form"/>
     </record>
     <menuitem parent="menu_customs" action="act_duty_rate_form" sequence="20" id="menu_duty_rate_form"/>
     <record model="ir.model.access" id="access_duty_rate">
-      <field name="model" search="[('model', '=', 'customs.duty.rate')]"/>
+      <field name="model">customs.duty.rate</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_duty_rate_admin">
-      <field name="model" search="[('model', '=', 'customs.duty.rate')]"/>
+      <field name="model">customs.duty.rate</field>
       <field name="group" ref="group_customs_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_customs-7.0.0/doc/conf.py` & `trytond_customs-7.2.0/doc/conf.py`

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

### Comparing `trytond_customs-7.0.0/doc/index.rst` & `trytond_customs-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/bg.po` & `trytond_customs-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/ca.po` & `trytond_customs-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/cs.po` & `trytond_customs-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/de.po` & `trytond_customs-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/es.po` & `trytond_customs-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/es_419.po` & `trytond_customs-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/et.po` & `trytond_customs-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/fa.po` & `trytond_customs-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/fi.po` & `trytond_customs-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/fr.po` & `trytond_customs-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/hu.po` & `trytond_customs-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/id.po` & `trytond_customs-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/it.po` & `trytond_customs-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/lo.po` & `trytond_customs-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/lt.po` & `trytond_customs-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/nl.po` & `trytond_customs-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/pl.po` & `trytond_customs-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/pt.po` & `trytond_customs-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/ro.po` & `trytond_customs-7.2.0/locale/tr.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Țară"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,organization:"
 msgid "Organization"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "UoM"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Țară"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
@@ -74,18 +76,17 @@
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product-customs.tariff.code,country:"
 msgid "Country"
-msgstr "Țară"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,end_month:"
 msgid "End Month"
@@ -93,69 +94,72 @@
 
 msgctxt "field:product-customs.tariff.code,organization:"
 msgid "Organization"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr ""
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Țară"
+msgstr ""
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Țară"
+msgstr ""
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
 msgctxt "help:customs.duty.rate,uom:"
 msgid "The Unit of Measure."
@@ -181,94 +185,100 @@
 msgid "The country of origin of the product."
 msgstr ""
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr ""
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
 msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Vamă"
+msgstr "Customs"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
 msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr ""
+msgstr "Customs Administration"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
 msgstr "Export"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Categorie"
+msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Șablon"
+msgstr ""
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Calcul"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "De la"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "La"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Vamă"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Vamă"
+msgstr "Customs"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-7.0.0/locale/ru.po` & `trytond_customs-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/sl.po` & `trytond_customs-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/tr.po` & `trytond_customs-7.2.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr ""
+msgstr "考文垂郡"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
@@ -31,33 +32,37 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "UoM"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr ""
+msgstr "语言编码"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr ""
+msgstr "考文垂郡"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr ""
+msgstr "描述"
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "field:customs.tariff.code,end_day:"
@@ -76,17 +81,18 @@
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,country:"
 msgid "Country"
-msgstr ""
+msgstr "考文垂郡"
 
 msgctxt "field:product-customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,end_month:"
 msgid "End Month"
@@ -123,34 +129,36 @@
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr ""
+msgstr "考文垂郡"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr ""
+msgstr "考文垂郡"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,tariff_codes:"
@@ -203,17 +211,18 @@
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Export"
+msgstr "导出"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
@@ -242,15 +251,15 @@
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Export"
+msgstr "导出"
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "selection:product-customs.tariff.code,product:"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_customs-7.0.0/locale/uk.po` & `trytond_customs-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/locale/zh_CN.po` & `trytond_customs-7.2.0/locale/ro.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,293 +1,292 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr ""
+msgstr "Tipul de calcul"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr "Țară"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data de sfârșit"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,organization:"
 msgid "Organization"
-msgstr ""
+msgstr "Organizație"
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data de început"
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr "Codul de tarif"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "UoM"
-msgstr ""
+msgstr "UM"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "语言编码"
+msgstr "Cod"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr "Țară"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,organization:"
 msgid "Organization"
-msgstr ""
+msgstr "Organizație"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr ""
+msgstr "Ziua de început"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr ""
+msgstr "Luna de început"
 
-#, fuzzy
 msgctxt "field:product-customs.tariff.code,country:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr "Țară"
 
 msgctxt "field:product-customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,organization:"
 msgid "Organization"
-msgstr ""
+msgstr "Organizație"
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:product-customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr "Codul de tarif"
 
-#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
 
 #, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr "Coduri tarifare"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr "Țară"
 
+#, fuzzy
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr ""
+msgstr "Categoria vamală"
 
 #, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr "Coduri tarifare"
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Utilizați codurile tarifare ale categoriei"
 
-#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr "Țară"
 
+#, fuzzy
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr ""
+msgstr "Categoria vamală"
 
 #, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr "Coduri tarifare"
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Utilizați codurile tarifare ale categoriei"
 
 msgctxt "help:customs.duty.rate,uom:"
 msgid "The Unit of Measure."
-msgstr ""
+msgstr "Unitatea de Măsură."
 
+#, fuzzy
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr ""
+msgstr "Codul din Sistemul Armonizat de Nomenclatură."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
 msgctxt "help:product.product,country_of_origin:"
 msgid "The country of origin of the product."
-msgstr ""
+msgstr "Țara de origine a produsului."
 
+#, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr ""
+msgstr "Utilizați codurile tarifare definite pe categorie."
 
 msgctxt "help:product.template,country_of_origin:"
 msgid "The country of origin of the product."
-msgstr ""
+msgstr "Țara de origine a produsului."
 
+#, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr ""
+msgstr "Utilizați codurile tarifare definite pe categorie."
 
-#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Duty Rates"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr "Codul de tarif"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr "Coduri tarifare"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "导出"
+msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr "Coduri tarifare"
 
+#, fuzzy
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr ""
+msgstr "Produs - Cod Tarif"
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Customs Administration"
+msgstr "Administrația vamală"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "导出"
+msgstr "Export"
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr ""
+msgstr "Categorie"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr ""
+msgstr "Șablon"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr ""
+msgstr "Calcul"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr ""
+msgstr "De la"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr ""
+msgstr "La"
 
-#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
 
-#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
```

### Comparing `trytond_customs-7.0.0/product.py` & `trytond_customs-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/product.xml` & `trytond_customs-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/setup.py` & `trytond_customs-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/tests/test_module.py` & `trytond_customs-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/tox.ini` & `trytond_customs-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/trytond_customs.egg-info/PKG-INFO` & `trytond_customs-7.2.0/trytond_customs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-customs
-Version: 7.0.0
+Name: trytond_customs
+Version: 7.2.0
 Summary: Tryton module for customs
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
@@ -50,18 +50,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Customs Module
 ##############
 
 The customs module allows to define customs duty based on the tariff code.
```

### Comparing `trytond_customs-7.0.0/trytond_customs.egg-info/SOURCES.txt` & `trytond_customs-7.2.0/trytond_customs.egg-info/SOURCES.txt`

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
 customs.py
```

### Comparing `trytond_customs-7.0.0/view/category_form.xml` & `trytond_customs-7.2.0/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/view/duty_rate_form.xml` & `trytond_customs-7.2.0/view/duty_rate_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/view/product-tariff_code_list.xml` & `trytond_customs-7.2.0/view/product-tariff_code_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/view/product-tariff_code_list_sequence.xml` & `trytond_customs-7.2.0/view/product-tariff_code_list_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/view/tariff_code_form.xml` & `trytond_customs-7.2.0/view/tariff_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-7.0.0/view/template_form.xml` & `trytond_customs-7.2.0/view/template_form.xml`

 * *Files identical despite different names*

