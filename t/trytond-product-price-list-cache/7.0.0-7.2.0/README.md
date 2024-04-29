# Comparing `tmp/trytond_product_price_list_cache-7.0.0.tar.gz` & `tmp/trytond_product_price_list_cache-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_price_list_cache-7.0.0.tar", last modified: Mon Oct 30 17:33:20 2023, max compression
+gzip compressed data, was "trytond_product_price_list_cache-7.2.0.tar", last modified: Mon Apr 29 15:43:40 2024, max compression
```

## Comparing `trytond_product_price_list_cache-7.0.0.tar` & `trytond_product_price_list_cache-7.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-10-22 17:23:10.000000 trytond_product_price_list_cache-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2023-10-30 17:09:19.000000 trytond_product_price_list_cache-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2023-10-30 17:09:19.000000 trytond_product_price_list_cache-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-10-22 17:23:10.000000 trytond_product_price_list_cache-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:10.000000 trytond_product_price_list_cache-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      932 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      969 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      959 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 16:47:45.000000 trytond_product_price_list_cache-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7256 2023-10-24 07:56:52.000000 trytond_product_price_list_cache-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4660 2023-10-27 17:38:49.000000 trytond_product_price_list_cache-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5019 2023-10-07 15:40:36.000000 trytond_product_price_list_cache-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_price_list_cache-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       95 2023-10-30 17:09:15.000000 trytond_product_price_list_cache-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:20.476435 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1443 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      100 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:40.907670 trytond_product_price_list_cache-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:22:14.000000 trytond_product_price_list_cache-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:22:14.000000 trytond_product_price_list_cache-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2667 2024-04-29 15:43:40.907670 trytond_product_price_list_cache-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:40.904337 trytond_product_price_list_cache-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3087 2024-04-27 16:30:39.000000 trytond_product_price_list_cache-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:17.000000 trytond_product_price_list_cache-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:40.904337 trytond_product_price_list_cache-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      932 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      969 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      959 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2024-04-27 16:43:25.000000 trytond_product_price_list_cache-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7256 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:40.907670 trytond_product_price_list_cache-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4651 2024-04-27 16:30:39.000000 trytond_product_price_list_cache-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:40.904337 trytond_product_price_list_cache-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5019 2024-02-04 18:51:26.000000 trytond_product_price_list_cache-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:17.000000 trytond_product_price_list_cache-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       95 2024-04-29 15:22:10.000000 trytond_product_price_list_cache-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:40.904337 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2667 2024-04-29 15:43:40.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1425 2024-04-29 15:43:40.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:40.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-04-29 15:43:40.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:20.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      100 2024-04-29 15:43:40.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:40.000000 trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/top_level.txt
```

### Comparing `trytond_product_price_list_cache-7.0.0/COPYRIGHT` & `trytond_product_price_list_cache-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2023 Cédric Krier
-Copyright (C) 2023 B2CK
+Copyright (C) 2023-2024 Cédric Krier
+Copyright (C) 2023-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_price_list_cache-7.0.0/LICENSE` & `trytond_product_price_list_cache-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/PKG-INFO` & `trytond_product_price_list_cache-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list_cache
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to cache price lists
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-price-list-cache
+Project-URL: Documentation, https://docs.tryton.org/modules-product-price-list-cache
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product price list cache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,17 +48,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 ###############################
 Product Price List Cache Module
 ###############################
 
 The *Product Price List Cache Module* pre-computes an stores prices for each
```

### Comparing `trytond_product_price_list_cache-7.0.0/doc/conf.py` & `trytond_product_price_list_cache-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_price_list_cache-7.0.0/locale/bg.po` & `trytond_product_price_list_cache-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/ca.po` & `trytond_product_price_list_cache-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/cs.po` & `trytond_product_price_list_cache-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/de.po` & `trytond_product_price_list_cache-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/es.po` & `trytond_product_price_list_cache-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/es_419.po` & `trytond_product_price_list_cache-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/et.po` & `trytond_product_price_list_cache-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/fa.po` & `trytond_product_price_list_cache-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/fi.po` & `trytond_product_price_list_cache-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/fr.po` & `trytond_product_price_list_cache-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/hu.po` & `trytond_product_price_list_cache-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/id.po` & `trytond_product_price_list_cache-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/it.po` & `trytond_product_price_list_cache-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/lo.po` & `trytond_product_price_list_cache-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/lt.po` & `trytond_product_price_list_cache-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/nl.po` & `trytond_product_price_list_cache-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/pl.po` & `trytond_product_price_list_cache-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/pt.po` & `trytond_product_price_list_cache-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/ro.po` & `trytond_product_price_list_cache-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/ru.po` & `trytond_product_price_list_cache-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/sl.po` & `trytond_product_price_list_cache-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/tr.po` & `trytond_product_price_list_cache-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/uk.po` & `trytond_product_price_list_cache-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/locale/zh_CN.po` & `trytond_product_price_list_cache-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/product.py` & `trytond_product_price_list_cache-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/setup.py` & `trytond_product_price_list_cache-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-product-price-list-cache'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product price list cache',
     package_dir={'trytond.modules.product_price_list_cache': '.'},
     packages=(
```

### Comparing `trytond_product_price_list_cache-7.0.0/tests/test_module.py` & `trytond_product_price_list_cache-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/tox.ini` & `trytond_product_price_list_cache-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/PKG-INFO` & `trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-product-price-list-cache
-Version: 7.0.0
+Name: trytond_product_price_list_cache
+Version: 7.2.0
 Summary: Tryton module to cache price lists
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-price-list-cache
+Project-URL: Documentation, https://docs.tryton.org/modules-product-price-list-cache
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product price list cache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,17 +48,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 ###############################
 Product Price List Cache Module
 ###############################
 
 The *Product Price List Cache Module* pre-computes an stores prices for each
```

### Comparing `trytond_product_price_list_cache-7.0.0/trytond_product_price_list_cache.egg-info/SOURCES.txt` & `trytond_product_price_list_cache-7.2.0/trytond_product_price_list_cache.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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

