# Comparing `tmp/trytond_edocument_unece-7.0.0.tar.gz` & `tmp/trytond_edocument_unece-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_edocument_unece-7.0.0.tar", last modified: Mon Oct 30 17:30:18 2023, max compression
+gzip compressed data, was "trytond_edocument_unece-7.2.0.tar", last modified: Mon Apr 29 15:40:48 2024, max compression
```

## Comparing `trytond_edocument_unece-7.0.0.tar` & `trytond_edocument_unece-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:18.725568 trytond_edocument_unece-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:23:04.000000 trytond_edocument_unece-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1043 2023-10-30 17:06:42.000000 trytond_edocument_unece-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:06:42.000000 trytond_edocument_unece-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2877 2023-10-30 17:30:18.725568 trytond_edocument_unece-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5488 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      756 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:18.722235 trytond_edocument_unece-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:23:04.000000 trytond_edocument_unece-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:04.000000 trytond_edocument_unece-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:18.718902 trytond_edocument_unece-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:22.000000 trytond_edocument_unece-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10156 2023-10-28 12:11:22.000000 trytond_edocument_unece-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:22.000000 trytond_edocument_unece-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9891 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10361 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8111 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11054 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10228 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7616 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8104 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10030 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7611 2023-10-28 12:11:23.000000 trytond_edocument_unece-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4738 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:30:18.725568 trytond_edocument_unece-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4371 2023-10-27 17:38:49.000000 trytond_edocument_unece-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:18.722235 trytond_edocument_unece-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_edocument_unece-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      100 2023-10-30 17:06:37.000000 trytond_edocument_unece-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:18.722235 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2877 2023-10-30 17:30:18.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-10-30 17:30:18.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:18.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:30:18.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:30:18.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:30:18.000000 trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:18.722235 trytond_edocument_unece-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/view/account_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/view/account_tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.0.0/view/product_uom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.0.0/view/product_uom_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:48.448848 trytond_edocument_unece-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-29 15:20:01.000000 trytond_edocument_unece-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:20:01.000000 trytond_edocument_unece-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-29 15:40:48.448848 trytond_edocument_unece-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-03-17 11:01:36.000000 trytond_edocument_unece-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5488 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      756 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:48.445514 trytond_edocument_unece-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_edocument_unece-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-03-17 11:01:36.000000 trytond_edocument_unece-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:10.000000 trytond_edocument_unece-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:48.445514 trytond_edocument_unece-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10156 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9891 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10361 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8111 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11054 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10228 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7616 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8104 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10030 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7611 2024-04-27 16:43:24.000000 trytond_edocument_unece-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4738 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:48.448848 trytond_edocument_unece-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4371 2024-03-17 11:01:36.000000 trytond_edocument_unece-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:48.445514 trytond_edocument_unece-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:10.000000 trytond_edocument_unece-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      100 2024-04-29 15:19:57.000000 trytond_edocument_unece-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:48.448848 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-29 15:40:48.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1600 2024-04-29 15:40:48.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:48.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:40:48.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:40:48.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:48.000000 trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:48.448848 trytond_edocument_unece-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/view/account_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/view/account_tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-01-16 14:00:20.000000 trytond_edocument_unece-7.2.0/view/product_uom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_edocument_unece-7.2.0/view/product_uom_tree.xml
```

### Comparing `trytond_edocument_unece-7.0.0/CHANGELOG` & `trytond_edocument_unece-7.2.0/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_edocument_unece-7.0.0/LICENSE` & `trytond_edocument_unece-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/PKG-INFO` & `trytond_edocument_unece-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_edocument_unece
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for electronic document UNECE codes
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
@@ -47,25 +47,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 EDocument UNECE Module
 ######################
 
 The module adds many codes from the UNECE:
 
     * `Recommendation N°. 20 Codes for Units of Measure Used in International
-      Trade <https://tfig.unece.org/contents/recommendation-20.htm>`_
+      Trade
+      <https://tfig.unece.org/instruments/recommendations-and-standards/unece-and-uncefact-recommendations/recommendation-no-20/>`_
 
     * `5153  Duty or tax or fee type name code
       <https://unece.org/fileadmin/DAM/trade/untdid/d16b/tred/tred5153.htm>`_
 
     * `5305  Duty or tax or fee category code
       <https://unece.org/fileadmin/DAM/trade/untdid/d16b/tred/tred5305.htm>`_
```

### Comparing `trytond_edocument_unece-7.0.0/__init__.py` & `trytond_edocument_unece-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/account.py` & `trytond_edocument_unece-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/account.xml` & `trytond_edocument_unece-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/doc/conf.py` & `trytond_edocument_unece-7.2.0/doc/conf.py`

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

### Comparing `trytond_edocument_unece-7.0.0/locale/bg.po` & `trytond_edocument_unece-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/ca.po` & `trytond_edocument_unece-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/cs.po` & `trytond_edocument_unece-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/de.po` & `trytond_edocument_unece-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/es.po` & `trytond_edocument_unece-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/es_419.po` & `trytond_edocument_unece-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/et.po` & `trytond_edocument_unece-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/fa.po` & `trytond_edocument_unece-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/fi.po` & `trytond_edocument_unece-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/fr.po` & `trytond_edocument_unece-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/hu.po` & `trytond_edocument_unece-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/id.po` & `trytond_edocument_unece-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/it.po` & `trytond_edocument_unece-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/lo.po` & `trytond_edocument_unece-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/lt.po` & `trytond_edocument_unece-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/nl.po` & `trytond_edocument_unece-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/pl.po` & `trytond_edocument_unece-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/pt.po` & `trytond_edocument_unece-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/ro.po` & `trytond_edocument_unece-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/ru.po` & `trytond_edocument_unece-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/sl.po` & `trytond_edocument_unece-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/tr.po` & `trytond_edocument_unece-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/uk.po` & `trytond_edocument_unece-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/locale/zh_CN.po` & `trytond_edocument_unece-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/product.xml` & `trytond_edocument_unece-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/setup.py` & `trytond_edocument_unece-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/tox.ini` & `trytond_edocument_unece-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/PKG-INFO` & `trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-edocument-unece
-Version: 7.0.0
+Name: trytond_edocument_unece
+Version: 7.2.0
 Summary: Tryton module for electronic document UNECE codes
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
@@ -47,25 +47,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 EDocument UNECE Module
 ######################
 
 The module adds many codes from the UNECE:
 
     * `Recommendation N°. 20 Codes for Units of Measure Used in International
-      Trade <https://tfig.unece.org/contents/recommendation-20.htm>`_
+      Trade
+      <https://tfig.unece.org/instruments/recommendations-and-standards/unece-and-uncefact-recommendations/recommendation-no-20/>`_
 
     * `5153  Duty or tax or fee type name code
       <https://unece.org/fileadmin/DAM/trade/untdid/d16b/tred/tred5153.htm>`_
 
     * `5305  Duty or tax or fee category code
       <https://unece.org/fileadmin/DAM/trade/untdid/d16b/tred/tred5305.htm>`_
```

### Comparing `trytond_edocument_unece-7.0.0/trytond_edocument_unece.egg-info/SOURCES.txt` & `trytond_edocument_unece-7.2.0/trytond_edocument_unece.egg-info/SOURCES.txt`

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

