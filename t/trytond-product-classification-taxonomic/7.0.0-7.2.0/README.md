# Comparing `tmp/trytond_product_classification_taxonomic-7.0.0.tar.gz` & `tmp/trytond_product_classification_taxonomic-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_classification_taxonomic-7.0.0.tar", last modified: Mon Oct 30 17:32:20 2023, max compression
+gzip compressed data, was "trytond_product_classification_taxonomic-7.2.0.tar", last modified: Mon Apr 29 15:42:41 2024, max compression
```

## Comparing `trytond_product_classification_taxonomic-7.0.0.tar` & `trytond_product_classification_taxonomic-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:20.602816 trytond_product_classification_taxonomic-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-10-22 17:23:08.000000 trytond_product_classification_taxonomic-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1440 2023-10-30 17:08:38.000000 trytond_product_classification_taxonomic-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:08:37.000000 trytond_product_classification_taxonomic-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2867 2023-10-30 17:32:20.602816 trytond_product_classification_taxonomic-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:20.602816 trytond_product_classification_taxonomic-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2833 2023-10-22 17:23:08.000000 trytond_product_classification_taxonomic-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:08.000000 trytond_product_classification_taxonomic-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:20.599483 trytond_product_classification_taxonomic-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3299 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3096 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3007 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3119 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3117 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3044 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3296 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2968 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3116 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2883 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3238 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3007 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3117 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3149 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3178 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3116 2023-10-30 16:47:45.000000 trytond_product_classification_taxonomic-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3220 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3163 2023-10-28 12:11:23.000000 trytond_product_classification_taxonomic-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2167 2023-08-13 15:26:13.000000 trytond_product_classification_taxonomic-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8421 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:32:20.602816 trytond_product_classification_taxonomic-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4334 2023-10-27 17:38:49.000000 trytond_product_classification_taxonomic-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:20.599483 trytond_product_classification_taxonomic-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_classification_taxonomic-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       87 2023-10-30 17:08:32.000000 trytond_product_classification_taxonomic-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:20.602816 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2867 2023-10-30 17:32:20.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1795 2023-10-30 17:32:20.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:32:20.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-10-30 17:32:20.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       59 2023-10-30 17:32:20.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:32:20.000000 trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:20.602816 trytond_product_classification_taxonomic-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/view/cultivar_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/view/cultivar_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.0.0/view/cultivar_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/view/cultivar_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/view/taxon_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/view/taxon_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.0.0/view/taxon_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:41.899214 trytond_product_classification_taxonomic-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1541 2024-04-29 15:21:29.000000 trytond_product_classification_taxonomic-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:21:28.000000 trytond_product_classification_taxonomic-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2867 2024-04-29 15:42:41.899214 trytond_product_classification_taxonomic-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:41.895880 trytond_product_classification_taxonomic-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3095 2024-04-27 16:30:39.000000 trytond_product_classification_taxonomic-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:14.000000 trytond_product_classification_taxonomic-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:41.895880 trytond_product_classification_taxonomic-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3299 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3096 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3007 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3119 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3117 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2818 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3044 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3296 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2968 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3116 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3202 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2883 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3238 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3007 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3117 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3149 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3178 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2994 2024-04-29 13:17:17.000000 trytond_product_classification_taxonomic-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3116 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3220 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2818 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3163 2024-04-27 16:43:24.000000 trytond_product_classification_taxonomic-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2167 2024-01-27 09:58:52.000000 trytond_product_classification_taxonomic-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8283 2024-04-27 16:30:39.000000 trytond_product_classification_taxonomic-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:41.899214 trytond_product_classification_taxonomic-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4334 2024-03-17 11:01:36.000000 trytond_product_classification_taxonomic-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:41.899214 trytond_product_classification_taxonomic-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:14.000000 trytond_product_classification_taxonomic-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       87 2024-04-29 15:21:24.000000 trytond_product_classification_taxonomic-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:41.899214 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2867 2024-04-29 15:42:41.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1777 2024-04-29 15:42:41.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:41.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-29 15:42:41.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       59 2024-04-29 15:42:41.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:41.000000 trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:41.899214 trytond_product_classification_taxonomic-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/view/cultivar_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/view/cultivar_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-7.2.0/view/cultivar_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/view/cultivar_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/view/taxon_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/view/taxon_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-7.2.0/view/taxon_tree.xml
```

### Comparing `trytond_product_classification_taxonomic-7.0.0/CHANGELOG` & `trytond_product_classification_taxonomic-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_product_classification_taxonomic-7.0.0/LICENSE` & `trytond_product_classification_taxonomic-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/PKG-INFO` & `trytond_product_classification_taxonomic-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_classification_taxonomic
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to implement product classification taxonomic
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
@@ -45,16 +45,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product_classification<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product_classification<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Classification Taxonomic Module
 #######################################
 
 The Product Classification Taxonomic module adds the taxonomic classification
 to the products.
```

### Comparing `trytond_product_classification_taxonomic-7.0.0/README.rst` & `trytond_product_classification_taxonomic-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/doc/conf.py` & `trytond_product_classification_taxonomic-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_classification_taxonomic-7.0.0/doc/index.rst` & `trytond_product_classification_taxonomic-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/bg.po` & `trytond_product_classification_taxonomic-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/ca.po` & `trytond_product_classification_taxonomic-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/cs.po` & `trytond_product_classification_taxonomic-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/de.po` & `trytond_product_classification_taxonomic-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/es.po` & `trytond_product_classification_taxonomic-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/es_419.po` & `trytond_product_classification_taxonomic-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/et.po` & `trytond_product_classification_taxonomic-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/fa.po` & `trytond_product_classification_taxonomic-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/fi.po` & `trytond_product_classification_taxonomic-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/fr.po` & `trytond_product_classification_taxonomic-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/hu.po` & `trytond_product_classification_taxonomic-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/id.po` & `trytond_product_classification_taxonomic-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/it.po` & `trytond_product_classification_taxonomic-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/lo.po` & `trytond_product_classification_taxonomic-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/lt.po` & `trytond_product_classification_taxonomic-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/nl.po` & `trytond_product_classification_taxonomic-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/pl.po` & `trytond_product_classification_taxonomic-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/pt.po` & `trytond_product_classification_taxonomic-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/ro.po` & `trytond_product_classification_taxonomic-7.2.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:product.cultivar.group,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:product.taxon,childs:"
 msgid "Children"
-msgstr "Copii"
+msgstr ""
 
 msgctxt "field:product.taxon,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:product.taxon,parent:"
 msgid "Parent"
@@ -108,23 +108,23 @@
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Division"
 msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Domain"
-msgstr "Domeniu"
+msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Family"
-msgstr "Familie"
+msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Form"
-msgstr "Formular"
+msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Genus"
 msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Kingdom"
```

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/ru.po` & `trytond_product_classification_taxonomic-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/sl.po` & `trytond_product_classification_taxonomic-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/tr.po` & `trytond_product_classification_taxonomic-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/uk.po` & `trytond_product_classification_taxonomic-7.2.0/locale/ro.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.cultivar,groups:"
 msgid "Groups"
-msgstr ""
+msgstr "Grupuri"
 
 msgctxt "field:product.cultivar,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nume"
 
 msgctxt "field:product.cultivar,selectable:"
 msgid "Selectable"
-msgstr ""
+msgstr "Selectabil"
 
 msgctxt "field:product.cultivar,taxon:"
 msgid "Taxon"
 msgstr ""
 
 msgctxt "field:product.cultivar-product.cultivar.group,cultivar:"
 msgid "Cultivar"
 msgstr ""
 
 msgctxt "field:product.cultivar-product.cultivar.group,group:"
 msgid "Group"
-msgstr ""
+msgstr "Grup"
 
 msgctxt "field:product.cultivar.group,cultivars:"
 msgid "Cultivars"
 msgstr ""
 
 msgctxt "field:product.cultivar.group,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nume"
 
 msgctxt "field:product.taxon,childs:"
 msgid "Children"
-msgstr ""
+msgstr "Copii"
 
 msgctxt "field:product.taxon,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nume"
 
+#, fuzzy
 msgctxt "field:product.taxon,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "Părinte"
 
 msgctxt "field:product.taxon,rank:"
 msgid "Type"
-msgstr ""
+msgstr "Tip"
 
 msgctxt "field:product.taxon,selectable:"
 msgid "Selectable"
-msgstr ""
+msgstr "Selectabil"
 
 msgctxt "model:ir.action,name:act_cultivar_form"
 msgid "Cultivars"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_cultivar_group_form"
 msgid "Groups"
-msgstr ""
+msgstr "Grupuri"
 
 msgctxt "model:ir.action,name:act_taxon_form"
 msgid "Taxons"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_taxon_tree"
 msgid "Taxons"
@@ -72,15 +73,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_cultivar"
 msgid "Cultivars"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_cultivar_group"
 msgid "Groups"
-msgstr ""
+msgstr "Grupuri"
 
 msgctxt "model:ir.ui.menu,name:menu_taxon"
 msgid "Taxons"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_taxon_tree"
 msgid "Taxons"
@@ -100,60 +101,62 @@
 
 msgctxt "model:product.taxon,name:"
 msgid "Taxon"
 msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Class"
-msgstr ""
+msgstr "Clasă"
 
+#, fuzzy
 msgctxt "selection:product.taxon,rank:"
 msgid "Division"
-msgstr ""
+msgstr "Divizie"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Domain"
-msgstr ""
+msgstr "Domeniu"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Family"
-msgstr ""
+msgstr "Familie"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Form"
-msgstr ""
+msgstr "Formular"
 
+#, fuzzy
 msgctxt "selection:product.taxon,rank:"
 msgid "Genus"
-msgstr ""
+msgstr "Gen"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Kingdom"
 msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Order"
-msgstr ""
+msgstr "Ordin"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Phylum"
 msgstr ""
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Section"
-msgstr ""
+msgstr "Secțiune"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Series"
-msgstr ""
+msgstr "Serie"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Species"
-msgstr ""
+msgstr "Specie"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Tribe"
-msgstr ""
+msgstr "Trib"
 
 msgctxt "selection:product.taxon,rank:"
 msgid "Variety"
-msgstr ""
+msgstr "varietate"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_product_classification_taxonomic-7.0.0/locale/zh_CN.po` & `trytond_product_classification_taxonomic-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/product.py` & `trytond_product_classification_taxonomic-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/product.xml` & `trytond_product_classification_taxonomic-7.2.0/product.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_product_classification_taxonomic-7.0.0/product.xml` & `trytond_product_classification_taxonomic-7.2.0/product.xml`

```diff
@@ -49,22 +49,22 @@
     <record model="ir.action.act_window.view" id="act_taxon_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="taxon_view_form"/>
       <field name="act_window" ref="act_taxon_form"/>
     </record>
     <menuitem parent="menu_taxon_tree" action="act_taxon_form" sequence="10" id="menu_taxon" icon="tryton-list"/>
     <record model="ir.model.access" id="access_taxon">
-      <field name="model" search="[('model', '=', 'product.taxon')]"/>
+      <field name="model">product.taxon</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_taxon_admin">
-      <field name="model" search="[('model', '=', 'product.taxon')]"/>
+      <field name="model">product.taxon</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="cultivar_view_list">
@@ -89,22 +89,22 @@
     <record model="ir.action.act_window.view" id="act_cultivar_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="cultivar_view_form"/>
       <field name="act_window" ref="act_cultivar_form"/>
     </record>
     <menuitem parent="product_classification.menu_classification" action="act_cultivar_form" sequence="20" id="menu_cultivar" icon="tryton-list"/>
     <record model="ir.model.access" id="access_cultivar">
-      <field name="model" search="[('model', '=', 'product.cultivar')]"/>
+      <field name="model">product.cultivar</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_cultivar_admin">
-      <field name="model" search="[('model', '=', 'product.cultivar')]"/>
+      <field name="model">product.cultivar</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="cultivar_group_view_list">
@@ -129,22 +129,22 @@
     <record model="ir.action.act_window.view" id="act_cultivar_group_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="cultivar_group_view_form"/>
       <field name="act_window" ref="act_cultivar_group_form"/>
     </record>
     <menuitem parent="menu_cultivar" action="act_cultivar_group_form" sequence="10" id="menu_cultivar_group"/>
     <record model="ir.model.access" id="access_cultivar_group">
-      <field name="model" search="[('model', '=', 'product.cultivar.group')]"/>
+      <field name="model">product.cultivar.group</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_cultivar_group_admin">
-      <field name="model" search="[('model', '=', 'product.cultivar.group')]"/>
+      <field name="model">product.cultivar.group</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_product_classification_taxonomic-7.0.0/setup.py` & `trytond_product_classification_taxonomic-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/tox.ini` & `trytond_product_classification_taxonomic-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/PKG-INFO` & `trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-classification-taxonomic
-Version: 7.0.0
+Name: trytond_product_classification_taxonomic
+Version: 7.2.0
 Summary: Tryton module to implement product classification taxonomic
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
@@ -45,16 +45,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product_classification<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product_classification<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Classification Taxonomic Module
 #######################################
 
 The Product Classification Taxonomic module adds the taxonomic classification
 to the products.
```

### Comparing `trytond_product_classification_taxonomic-7.0.0/trytond_product_classification_taxonomic.egg-info/SOURCES.txt` & `trytond_product_classification_taxonomic-7.2.0/trytond_product_classification_taxonomic.egg-info/SOURCES.txt`

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
 product.py
```

