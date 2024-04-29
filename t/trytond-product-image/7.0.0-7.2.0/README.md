# Comparing `tmp/trytond_product_image-7.0.0.tar.gz` & `tmp/trytond_product_image-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_image-7.0.0.tar", last modified: Mon Oct 30 17:32:47 2023, max compression
+gzip compressed data, was "trytond_product_image-7.2.0.tar", last modified: Mon Apr 29 15:43:07 2024, max compression
```

## Comparing `trytond_product_image-7.0.0.tar` & `trytond_product_image-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:47.266277 trytond_product_image-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-22 17:23:09.000000 trytond_product_image-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      627 2023-10-30 17:08:57.000000 trytond_product_image-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:08:56.000000 trytond_product_image-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-10-30 17:32:47.266277 trytond_product_image-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:47.262943 trytond_product_image-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-10-22 17:23:09.000000 trytond_product_image-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:09.000000 trytond_product_image-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:47.262943 trytond_product_image-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1477 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1403 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1444 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1262 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1477 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-10-30 16:47:45.000000 trytond_product_image-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1232 2023-10-28 12:11:23.000000 trytond_product_image-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7800 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1410 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2107 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:32:47.266277 trytond_product_image-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4560 2023-10-27 17:38:49.000000 trytond_product_image-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:47.262943 trytond_product_image-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2080 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_image-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-10-30 17:08:53.000000 trytond_product_image-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:47.266277 trytond_product_image-7.0.0/trytond_product_image.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-10-30 17:32:46.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1602 2023-10-30 17:32:47.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:32:46.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:32:46.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       59 2023-10-30 17:32:46.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:32:46.000000 trytond_product_image-7.0.0/trytond_product_image.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:47.262943 trytond_product_image-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/view/image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/view/image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_product_image-7.0.0/view/template_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      783 2024-04-29 15:21:49.000000 trytond_product_image-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:21:49.000000 trytond_product_image-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2530 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.775204 trytond_product_image-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1228 2024-03-17 11:01:36.000000 trytond_product_image-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      627 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:15.000000 trytond_product_image-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.775204 trytond_product_image-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1545 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1468 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1499 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1524 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1334 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1312 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1542 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10700 2024-04-29 13:17:17.000000 trytond_product_image-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2689 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2896 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4551 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.775204 trytond_product_image-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3646 2024-03-17 11:01:36.000000 trytond_product_image-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:15.000000 trytond_product_image-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:21:45.000000 trytond_product_image-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/trytond_product_image.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2530 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       59 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:07.000000 trytond_product_image-7.2.0/trytond_product_image.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:07.778537 trytond_product_image-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      603 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-27 16:30:39.000000 trytond_product_image-7.2.0/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_product_image-7.2.0/view/template_list.xml
```

### Comparing `trytond_product_image-7.0.0/COPYRIGHT` & `trytond_product_image-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_image-7.0.0/LICENSE` & `trytond_product_image-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.0.0/PKG-INFO` & `trytond_product_image-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_product_image
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that adds images to products
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-image
+Project-URL: Documentation, https://docs.tryton.org/modules-product-image
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product image thumbnail
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pillow
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 ####################
 Product Image Module
 ####################
 
 The *Product Image Module* adds images to each product and variant.
```

### Comparing `trytond_product_image-7.0.0/doc/conf.py` & `trytond_product_image-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_image-7.0.0/doc/configuration.rst` & `trytond_product_image-7.2.0/doc/configuration.rst`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,24 @@
 
 This is the prefix to use with the :py:mod:`trytond:trytond.filestore`.
 This value is only used when the `image_filestore
 <config-product-image_filestore>` setting is in use.
 
 The default value is: ``None``
 
+.. _config-product-image_size_max:
+
+``image_size_max``
+==================
+
+The is the maximal horizontal and vertical size in pixels for the stored
+images.
+
+The default value is: ``2048``
+
 ``image_base``
 ==============
 
 The base URL for the images, without the path.
 
 The default value is generated from the `hostname
 <trytond:topics-configuration>` configuration setting.
```

### Comparing `trytond_product_image-7.0.0/locale/bg.po` & `trytond_product_image-7.2.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/ca.po` & `trytond_product_image-7.2.0/locale/fr.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Memòria cau"
+msgstr "Cache"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Imatge"
+msgstr "Image"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "ID de la imatge"
+msgstr "ID de l'image"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variant"
+msgstr "Variante"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Producte"
+msgstr "Produit"
+
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr "Hauteur"
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Imatge"
+msgstr "Image"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "ID de la imatge"
+msgstr "ID de l'image"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Imatge del producte"
+msgstr "Image du produit"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Mida"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr "Largeur"
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "URL de la imatge"
+msgstr "URL de l'image"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Imatges"
+msgstr "Images"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "URL de la imatge"
+msgstr "URL de l'image"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Imatges"
+msgstr "Images"
 
 msgctxt "model:ir.message,text:msg_product_image_size_unique"
 msgid "The size of a product image must be unique."
-msgstr "La mida d'una imatge de producte ha de ser única."
+msgstr "La taille d'une image de produit doit être unique."
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Imatge del producte"
+msgstr "Image du produit"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Memòria cau de la imatge del producte"
+msgstr "Cache de l'image du produit"
```

### Comparing `trytond_product_image-7.0.0/locale/cs.po` & `trytond_product_image-7.2.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/de.po` & `trytond_product_image-7.2.0/locale/de.po`

 * *Files 5% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 msgid "Variant"
 msgstr "Variante"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr "Artikel"
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr "Bild"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr "Bild ID"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr "Artikelbild"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Größe"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr "Bild-URL"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
```

### Comparing `trytond_product_image-7.0.0/locale/es.po` & `trytond_product_image-7.2.0/locale/es.po`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 msgid "Variant"
 msgstr "Variante"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr "Producto"
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr "Imagen"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr "ID Imagen"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr "Imagen producto"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Tamaño"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr "URL Imagen"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
```

### Comparing `trytond_product_image-7.0.0/locale/es_419.po` & `trytond_product_image-7.2.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/et.po` & `trytond_product_image-7.2.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/fa.po` & `trytond_product_image-7.2.0/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/fi.po` & `trytond_product_image-7.2.0/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/fr.po` & `trytond_product_image-7.2.0/locale/nl.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,64 +4,68 @@
 
 msgctxt "field:product.image,cache:"
 msgid "Cache"
 msgstr "Cache"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Image"
+msgstr "Afbeelding"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "ID de l'image"
+msgstr "Afbeeldings-ID"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variante"
+msgstr "Variant"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Produit"
+msgstr "Product"
+
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Image"
+msgstr "Afbeelding"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "ID de l'image"
+msgstr "Afbeeldings-ID"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Image du produit"
+msgstr "Product afbeelding"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Taille"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "URL de l'image"
+msgstr "Afbeelding URL"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Images"
+msgstr "Afbeeldingen"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "URL de l'image"
+msgstr "Afbeelding URL"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Images"
+msgstr "Afbeeldingen"
 
 msgctxt "model:ir.message,text:msg_product_image_size_unique"
 msgid "The size of a product image must be unique."
-msgstr "La taille d'une image de produit doit être unique."
+msgstr "De grootte van een product afbeelding moet uniek zijn."
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Image du produit"
+msgstr "Product afbeelding"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Cache de l'image du produit"
+msgstr "Cache van productafbeeldingen"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_product_image-7.0.0/locale/hu.po` & `trytond_product_image-7.2.0/locale/hu.po`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr "Termék"
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr "Termékkép"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/id.po` & `trytond_product_image-7.2.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/it.po` & `trytond_product_image-7.2.0/locale/it.po`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr "Prodotto"
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Dimensione"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
 msgid "Images"
```

### Comparing `trytond_product_image-7.0.0/locale/lo.po` & `trytond_product_image-7.2.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/lt.po` & `trytond_product_image-7.2.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/nl.po` & `trytond_product_image-7.2.0/locale/sl.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Cache"
+msgstr "Predpomnilnik"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Afbeelding"
+msgstr "Podoba"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "Afbeeldings-ID"
+msgstr "ID podobe"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Variant"
+msgstr "Različica"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Product"
+msgstr "Izdelek"
+
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Afbeelding"
+msgstr "Podoba"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "Afbeeldings-ID"
+msgstr "ID podobe"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Product afbeelding"
+msgstr "Podoba produkta"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Grootte"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "Afbeelding URL"
+msgstr "URL podobe"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Afbeeldingen"
+msgstr "Podobe"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "Afbeelding URL"
+msgstr "URL podobe"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Afbeeldingen"
+msgstr "Podobe"
 
 msgctxt "model:ir.message,text:msg_product_image_size_unique"
 msgid "The size of a product image must be unique."
-msgstr "De grootte van een product afbeelding moet uniek zijn."
+msgstr "Velikost podobe izdelka mora biti edinstvena."
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Product afbeelding"
+msgstr "Podoba izdelka"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Cache van productafbeeldingen"
+msgstr "Predpomnilnik podobe izdelka"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_product_image-7.0.0/locale/pl.po` & `trytond_product_image-7.2.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/pt.po` & `trytond_product_image-7.2.0/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/ro.po` & `trytond_product_image-7.2.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/ru.po` & `trytond_product_image-7.2.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/sl.po` & `trytond_product_image-7.2.0/locale/ca.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.image,cache:"
 msgid "Cache"
-msgstr "Predpomnilnik"
+msgstr "Memòria cau"
 
 msgctxt "field:product.image,image:"
 msgid "Image"
-msgstr "Podoba"
+msgstr "Imatge"
 
 msgctxt "field:product.image,image_id:"
 msgid "Image ID"
-msgstr "ID podobe"
+msgstr "ID de la imatge"
 
 msgctxt "field:product.image,product:"
 msgid "Variant"
-msgstr "Različica"
+msgstr "Variant"
 
 msgctxt "field:product.image,template:"
 msgid "Product"
-msgstr "Izdelek"
+msgstr "Producte"
+
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
 
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
-msgstr "Podoba"
+msgstr "Imatge"
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
-msgstr "ID podobe"
+msgstr "ID de la imatge"
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
-msgstr "Podoba produkta"
+msgstr "Imatge del producte"
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
-msgstr "Velikost"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
+msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
-msgstr "URL podobe"
+msgstr "URL de la imatge"
 
 msgctxt "field:product.product,images:"
 msgid "Images"
-msgstr "Podobe"
+msgstr "Imatges"
 
 msgctxt "field:product.template,image_url:"
 msgid "Image URL"
-msgstr "URL podobe"
+msgstr "URL de la imatge"
 
 msgctxt "field:product.template,images:"
 msgid "Images"
-msgstr "Podobe"
+msgstr "Imatges"
 
 msgctxt "model:ir.message,text:msg_product_image_size_unique"
 msgid "The size of a product image must be unique."
-msgstr "Velikost podobe izdelka mora biti edinstvena."
+msgstr "La mida d'una imatge de producte ha de ser única."
 
 msgctxt "model:product.image,name:"
 msgid "Product Image"
-msgstr "Podoba izdelka"
+msgstr "Imatge del producte"
 
 msgctxt "model:product.image.cache,name:"
 msgid "Product Image Cache"
-msgstr "Predpomnilnik podobe izdelka"
+msgstr "Memòria cau de la imatge del producte"
```

### Comparing `trytond_product_image-7.0.0/locale/tr.po` & `trytond_product_image-7.2.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/uk.po` & `trytond_product_image-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/locale/zh_CN.po` & `trytond_product_image-7.2.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:product.image,template:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product.image.cache,height:"
+msgid "Height"
+msgstr ""
+
 msgctxt "field:product.image.cache,image:"
 msgid "Image"
 msgstr ""
 
 msgctxt "field:product.image.cache,image_id:"
 msgid "Image ID"
 msgstr ""
 
 msgctxt "field:product.image.cache,product_image:"
 msgid "Product Image"
 msgstr ""
 
-msgctxt "field:product.image.cache,size:"
-msgid "Size"
+msgctxt "field:product.image.cache,width:"
+msgid "Width"
 msgstr ""
 
 msgctxt "field:product.product,image_url:"
 msgid "Image URL"
 msgstr ""
 
 msgctxt "field:product.product,images:"
```

### Comparing `trytond_product_image-7.0.0/product.py` & `trytond_product_image-7.2.0/product.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 from urllib.parse import quote, urlencode, urljoin
 
 import PIL.Image
 
 from trytond.config import config
 from trytond.model import (
     MatchMixin, ModelSQL, ModelView, Unique, fields, sequence_ordered)
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 from trytond.pyson import Bool, Eval, If
 from trytond.tools import slugify
 from trytond.transaction import Transaction
 from trytond.url import http_host
 from trytond.wsgi import Base64Converter
 
 if config.getboolean('product', 'image_filestore', default=False):
     file_id = 'image_id'
     store_prefix = config.get('product', 'image_prefix', default=None)
 else:
     file_id = None
     store_prefix = None
+SIZE_MAX = config.getint('product', 'image_size_max', default=2048)
 URL_BASE = config.get('product', 'image_base', default='')
 URL_EXTERNAL_BASE = config.get('product', 'image_base', default=http_host())
 
 
 class ImageURLMixin:
     __slots__ = ()
     __image_url__ = None
@@ -43,34 +44,39 @@
                         'database': Base64Converter(None).to_url(
                             Transaction().database.name),
                         'code': quote(self.code, ''),
                         'name': slugify(self.name),
                         }))
             if args:
                 size = args.pop('s', None)
+                width = args.pop('w', None)
+                height = args.pop('h', None)
                 index = args.pop('i', None)
                 args = {k: int(bool(v)) for k, v in args.items()}
                 if size:
                     args['s'] = size
+                if width:
+                    args['w'] = width
+                if height:
+                    args['h'] = height
                 if index is not None:
                     args['i'] = index
                 url += '?' + urlencode(args)
             return url
 
     def get_image_url(self, _external=False, **args):
         return self._image_url(
             URL_EXTERNAL_BASE if _external else URL_BASE, **args)
 
     @property
     def images_used(self):
         yield from self.images
 
     def get_images(self, pattern):
-        pool = Pool()
-        Image = pool.get('product.image')
+        Image = self.__class__.images.get_target()
         pattern = pattern.copy()
         for key in set(pattern.keys()) - Image.allowed_match_keys():
             del pattern[key]
         pattern = {k: bool(int(v)) for k, v in pattern.items()}
         for image in self.images_used:
             if image.match(pattern):
                 yield image
@@ -95,46 +101,24 @@
     def images_used(self):
         yield from super().images_used
         for image in self.template.images_used:
             if not image.product:
                 yield image
 
 
-class ImageMixin:
+class _ImageMixin:
     __slots__ = ()
     image = fields.Binary(
         "Image", file_id=file_id, store_prefix=store_prefix, required=True)
     image_id = fields.Char("Image ID", readonly=True)
 
 
-class Image(ImageMixin, sequence_ordered(), ModelSQL, ModelView, MatchMixin):
-    "Product Image"
-    __name__ = 'product.image'
-    template = fields.Many2One(
-        'product.template', "Product",
-        required=True, ondelete='CASCADE',
-        domain=[
-            If(Bool(Eval('product')),
-                ('products', '=', Eval('product')),
-                ()),
-            ])
-    product = fields.Many2One(
-        'product.product', "Variant",
-        domain=[
-            If(Bool(Eval('template')),
-                ('template', '=', Eval('template')),
-                ()),
-            ])
-    cache = fields.One2Many(
-        'product.image.cache', 'product_image', "Cache", readonly=True)
-
-    @classmethod
-    def __setup__(cls):
-        super().__setup__()
-        cls.__access__.update(['product', 'template'])
+class ImageMixin(_ImageMixin):
+    __slots__ = ()
+    cache = None
 
     @classmethod
     def allowed_match_keys(cls):
         return set()
 
     @classmethod
     def create(cls, vlist):
@@ -153,86 +137,195 @@
                 values = values.copy()
                 values['image'] = cls.convert(values['image'])
             args.append(images)
             args.append(values)
         super().write(*args)
         cls.clear_cache(sum(args[0:None:2], []))
 
-    def get(self, size=400):
-        size = min((
+    @classmethod
+    def _round_size(cls, size):
+        return min((
                 2 ** math.ceil(math.log2(size)),
                 10 * math.ceil(size / 10) if size <= 100
                 else 50 * math.ceil(size / 50)))
-        if not (0 < size <= 2048):
-            raise ValueError("Invalid size")
+
+    def get(self, size=400):
+        if isinstance(size, int):
+            size = (size, size)
+        size = tuple(map(self._round_size, size))
+        if not all(0 < s <= SIZE_MAX for s in size):
+            raise ValueError(f"Invalid size {size}")
         for cache in self.cache:
-            if cache.size == size:
+            if (cache.width, cache.height) == size:
                 return cache.image
         with Transaction().new_transaction():
             cache = self._store_cache(size, self._resize(size))
             # Save cache only if record is already committed
             if self.__class__.search([('id', '=', self.id)]):
                 cache.save()
             return cache.image
 
     @classmethod
     def convert(cls, image, **_params):
         data = io.BytesIO()
         img = PIL.Image.open(io.BytesIO(image))
-        width, height = img.size
-        size = min(width, height)
-        img = img.crop((
-                (width - size) // 2,
-                (height - size) // 2,
-                (width + size) // 2,
-                (height + size) // 2))
-        if size > 2048:
-            img = img.resize((2048, 2048))
+        img.thumbnail((SIZE_MAX, SIZE_MAX))
         if img.mode in {'RGBA', 'P'}:
-            img = img.convert('RGB')
+            img.convert('RGBA')
+            background = PIL.Image.new('RGBA', img.size, (255, 255, 255))
+            background.alpha_composite(img)
+            img = background.convert('RGB')
         img.save(data, format='jpeg', optimize=True, **_params)
         return data.getvalue()
 
     def _resize(self, size=64, **_params):
         data = io.BytesIO()
         img = PIL.Image.open(io.BytesIO(self.image))
-        img = img.resize((size, size))
+        if isinstance(size, int):
+            size = (size, size)
+        img.thumbnail(size)
         img.save(data, format='jpeg', optimize=True, **_params)
         return data.getvalue()
 
     def _store_cache(self, size, image):
-        pool = Pool()
-        Cache = pool.get('product.image.cache')
+        Cache = self.__class__.cache.get_target()
+        if isinstance(size, int):
+            width = height = size
+        else:
+            width, height = size
         return Cache(
-            product_image=self,
             image=image,
-            size=size)
+            width=width,
+            height=height)
 
     @classmethod
     def clear_cache(cls, images):
-        pool = Pool()
-        Cache = pool.get('product.image.cache')
+        Cache = cls.cache.get_target()
         caches = [c for i in images for c in i.cache]
         Cache.delete(caches)
 
 
-class ImageCache(ImageMixin, ModelSQL):
+class Image(ImageMixin, sequence_ordered(), ModelSQL, ModelView, MatchMixin):
+    "Product Image"
+    __name__ = 'product.image'
+    template = fields.Many2One(
+        'product.template', "Product",
+        required=True, ondelete='CASCADE',
+        domain=[
+            If(Bool(Eval('product')),
+                ('products', '=', Eval('product')),
+                ()),
+            ])
+    product = fields.Many2One(
+        'product.product', "Variant",
+        domain=[
+            If(Bool(Eval('template')),
+                ('template', '=', Eval('template')),
+                ()),
+            ])
+    cache = fields.One2Many(
+        'product.image.cache', 'product_image', "Cache", readonly=True)
+
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.__access__.update(['product', 'template'])
+
+    def _store_cache(self, size, image):
+        cache = super()._store_cache(size, image)
+        cache.product_image = self
+        return cache
+
+
+class ImageCacheMixin(_ImageMixin):
+    __slots__ = ()
+
+    width = fields.Integer(
+        "Width", required=True,
+        domain=[
+            ('width', '>', 0),
+            ('width', '<=', SIZE_MAX),
+            ])
+    height = fields.Integer(
+        "Height", required=True,
+        domain=[
+            ('height', '>', 0),
+            ('height', '<=', SIZE_MAX),
+            ])
+
+
+class ImageCache(ImageCacheMixin, ModelSQL):
     "Product Image Cache"
     __name__ = 'product.image.cache'
     product_image = fields.Many2One(
         'product.image', "Product Image", required=True, ondelete='CASCADE')
-    size = fields.Integer(
-        "Size", required=True,
-        domain=[
-            ('size', '>', 0),
-            ('size', '<=', 2048),
-            ])
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         t = cls.__table__()
-        cls._sql_constraints = [
-            ('size_unique', Unique(t, t.product_image, t.size),
-                'ir.msg_product_image_size_unique'),
+        cls._sql_constraints += [
+            ('dimension_unique', Unique(t, t.product_image, t.width, t.height),
+                'product_image.msg_image_cache_size_unique'),
+            ]
+
+    @classmethod
+    def __register__(cls, module):
+        cursor = Transaction().connection.cursor()
+        table = cls.__table__()
+        table_h = cls.__table_handler__(module)
+
+        super().__register__(module)
+
+        # Migration from 7.0: split size into width and height
+        table_h.drop_constraint('size_unique')
+        if table_h.column_exist('size'):
+            cursor.execute(*table.update(
+                    [table.width, table.height],
+                    [table.size, table.size]))
+            table_h.drop_column('size')
+
+
+class Category(ImageURLMixin, metaclass=PoolMeta):
+    __name__ = 'product.category'
+    __image_url__ = '/product-category/image'
+    images = fields.One2Many('product.category.image', 'category', "Images")
+
+
+class CategoryImage(
+        ImageMixin, sequence_ordered(), ModelSQL, ModelView, MatchMixin):
+    "Category Image"
+    __name__ = 'product.category.image'
+    category = fields.Many2One(
+        'product.category', "Category",
+        required=True, ondelete='CASCADE')
+    cache = fields.One2Many(
+        'product.category.image.cache', 'category_image', "Cache",
+        readonly=True)
+
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.__access__.add('category')
+
+    def _store_cache(self, size, image):
+        cache = super()._store_cache(size, image)
+        cache.category_image = self
+        return cache
+
+
+class CategoryImageCache(ImageCacheMixin, ModelSQL):
+    "Category Image Cache"
+    __name__ = 'product.category.image.cache'
+    category_image = fields.Many2One(
+        'product.category.image', "Category Image", required=True,
+        ondelete='CASCADE')
+
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        t = cls.__table__()
+        cls._sql_constraints += [
+            ('dimension_unique',
+                Unique(t, t.category_image, t.width, t.height),
+                'product_image.msg_image_cache_size_unique'),
             ]
-        cls._order.append(('size', 'ASC'))
```

### Comparing `trytond_product_image-7.0.0/routes.py` & `trytond_product_image-7.2.0/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,26 +44,54 @@
                 ('code', '=', unquote(code)),
                 ])
     except ValueError:
         abort(HTTPStatus.NOT_FOUND)
     return _image(request, pool, product)
 
 
+@app.route(
+    '/product-category/image/<code>/<base64:database_name>',
+    methods={'GET'})
+@app.route(
+    '/product-category/image/<code>/<base64:database_name>/<name>',
+    methods={'GET'})
+@with_pool
+@with_transaction()
+def category_image(request, pool, code, name=None):
+    Category = pool.get('product.category')
+    try:
+        category, = Category.search([
+                ('code', '=', unquote(code)),
+                ])
+    except ValueError:
+        abort(HTTPStatus.NOT_FOUND)
+    return _image(request, pool, category)
+
+
 def _image(request, pool, record):
     images = record.get_images(request.args)
     if not images:
         abort(HTTPStatus.NOT_FOUND)
     try:
         image = list(images)[int(request.args.get('i', 0))]
     except IndexError:
         abort(HTTPStatus.NOT_FOUND)
     except ValueError:
         abort(HTTPStatus.BAD_REQUEST)
     try:
         size = int(request.args.get('s', 400))
     except ValueError:
         abort(HTTPStatus.BAD_REQUEST)
-    response = Response(image.get(size), mimetype='image/jpeg')
+    try:
+        width = int(request.args.get('w', size))
+    except ValueError:
+        abort(HTTPStatus.BAD_REQUEST)
+    try:
+        height = int(request.args.get('h', size))
+    except ValueError:
+        abort(HTTPStatus.BAD_REQUEST)
+
+    response = Response(image.get((width, height)), mimetype='image/jpeg')
     response.headers['Cache-Control'] = (
         'max-age=%s, public' % TIMEOUT)
     response.add_etag()
     return response
```

### Comparing `trytond_product_image-7.0.0/setup.py` & `trytond_product_image-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-product-image'),
+            'https://docs.tryton.org/modules-product-image'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product image thumbnail',
     package_dir={'trytond.modules.product_image': '.'},
     packages=(
         ['trytond.modules.product_image']
```

### Comparing `trytond_product_image-7.0.0/tox.ini` & `trytond_product_image-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_image-7.0.0/trytond_product_image.egg-info/PKG-INFO` & `trytond_product_image-7.2.0/trytond_product_image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-product-image
-Version: 7.0.0
+Name: trytond_product_image
+Version: 7.2.0
 Summary: Tryton module that adds images to products
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-image
+Project-URL: Documentation, https://docs.tryton.org/modules-product-image
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product image thumbnail
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pillow
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 ####################
 Product Image Module
 ####################
 
 The *Product Image Module* adds images to each product and variant.
```

### Comparing `trytond_product_image-7.0.0/trytond_product_image.egg-info/SOURCES.txt` & `trytond_product_image-7.2.0/trytond_product_image.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

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
@@ -40,14 +39,18 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
+./view/category_form.xml
+./view/category_image_form.xml
+./view/category_image_list.xml
+./view/category_list.xml
 ./view/image_form.xml
 ./view/image_list.xml
 ./view/template_form.xml
 ./view/template_list.xml
 doc/conf.py
 doc/configuration.rst
 doc/design.rst
@@ -83,11 +86,15 @@
 trytond_product_image.egg-info/PKG-INFO
 trytond_product_image.egg-info/SOURCES.txt
 trytond_product_image.egg-info/dependency_links.txt
 trytond_product_image.egg-info/entry_points.txt
 trytond_product_image.egg-info/not-zip-safe
 trytond_product_image.egg-info/requires.txt
 trytond_product_image.egg-info/top_level.txt
+view/category_form.xml
+view/category_image_form.xml
+view/category_image_list.xml
+view/category_list.xml
 view/image_form.xml
 view/image_list.xml
 view/template_form.xml
 view/template_list.xml
```

### Comparing `trytond_product_image-7.0.0/view/image_form.xml` & `trytond_product_image-7.2.0/view/image_form.xml`

 * *Files identical despite different names*

