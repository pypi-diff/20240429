# Comparing `tmp/trytond_sale_blanket_agreement-7.0.0.tar.gz` & `tmp/trytond_sale_blanket_agreement-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_blanket_agreement-7.0.0.tar", last modified: Mon Oct 30 17:37:11 2023, max compression
+gzip compressed data, was "trytond_sale_blanket_agreement-7.2.0.tar", last modified: Mon Apr 29 15:47:24 2024, max compression
```

## Comparing `trytond_sale_blanket_agreement-7.0.0.tar` & `trytond_sale_blanket_agreement-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:11.620871 trytond_sale_blanket_agreement-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:23:16.000000 trytond_sale_blanket_agreement-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:11:37.000000 trytond_sale_blanket_agreement-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 17:11:36.000000 trytond_sale_blanket_agreement-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2718 2023-10-30 17:37:11.620871 trytond_sale_blanket_agreement-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:11.617538 trytond_sale_blanket_agreement-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:23:16.000000 trytond_sale_blanket_agreement-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:16.000000 trytond_sale_blanket_agreement-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:11.614204 trytond_sale_blanket_agreement-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7252 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7340 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7328 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7290 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6180 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7397 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2023-10-30 16:47:45.000000 trytond_sale_blanket_agreement-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      929 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28848 2023-10-24 07:56:52.000000 trytond_sale_blanket_agreement-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11626 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:37:11.620871 trytond_sale_blanket_agreement-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4741 2023-10-27 17:38:49.000000 trytond_sale_blanket_agreement-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:11.614204 trytond_sale_blanket_agreement-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5317 2023-08-13 15:26:13.000000 trytond_sale_blanket_agreement-7.0.0/tests/scenario_sale_blanket_agreement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_blanket_agreement-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-10-30 17:11:32.000000 trytond_sale_blanket_agreement-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:11.620871 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2718 2023-10-30 17:37:11.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2299 2023-10-30 17:37:11.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:37:11.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:37:11.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      181 2023-10-30 17:37:11.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:37:11.000000 trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:11.617538 trytond_sale_blanket_agreement-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/product_list_agreement_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_create_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.0.0/view/sale_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.518489 trytond_sale_blanket_agreement-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:24:47.000000 trytond_sale_blanket_agreement-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-29 15:24:46.000000 trytond_sale_blanket_agreement-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2709 2024-04-29 15:47:24.518489 trytond_sale_blanket_agreement-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.511822 trytond_sale_blanket_agreement-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_sale_blanket_agreement-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:24.000000 trytond_sale_blanket_agreement-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7252 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7340 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7328 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7290 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6186 2024-04-29 13:17:17.000000 trytond_sale_blanket_agreement-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7397 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      929 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    29320 2024-04-22 12:14:36.000000 trytond_sale_blanket_agreement-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11419 2024-04-27 16:30:39.000000 trytond_sale_blanket_agreement-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:24.518489 trytond_sale_blanket_agreement-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4732 2024-04-27 16:30:39.000000 trytond_sale_blanket_agreement-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5183 2024-04-22 12:14:36.000000 trytond_sale_blanket_agreement-7.2.0/tests/scenario_sale_blanket_agreement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-22 12:14:36.000000 trytond_sale_blanket_agreement-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:24.000000 trytond_sale_blanket_agreement-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-29 15:24:42.000000 trytond_sale_blanket_agreement-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2709 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2281 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/product_list_agreement_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_create_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_line_list.xml
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/COPYRIGHT` & `trytond_sale_blanket_agreement-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Copyright (C) 2021 Hashbang
 Copyright (C) 2021 Maxime Richez
 Copyright (C) 2021 SALUC SA
 Copyright (C) 2021 Thierry Bruyere
-Copyright (C) 2022-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2022-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/LICENSE` & `trytond_sale_blanket_agreement-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/PKG-INFO` & `trytond_sale_blanket_agreement-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale_blanket_agreement
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for sale blanket agreement
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-blanket-agreement
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-blanket-agreement
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton,blanket agreement,sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,17 +49,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/__init__.py` & `trytond_sale_blanket_agreement-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/doc/conf.py` & `trytond_sale_blanket_agreement-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_blanket_agreement-7.0.0/doc/design.rst` & `trytond_sale_blanket_agreement-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/bg.po` & `trytond_sale_blanket_agreement-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/ca.po` & `trytond_sale_blanket_agreement-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/cs.po` & `trytond_sale_blanket_agreement-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/de.po` & `trytond_sale_blanket_agreement-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/es.po` & `trytond_sale_blanket_agreement-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/es_419.po` & `trytond_sale_blanket_agreement-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/et.po` & `trytond_sale_blanket_agreement-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/fa.po` & `trytond_sale_blanket_agreement-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/fi.po` & `trytond_sale_blanket_agreement-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/fr.po` & `trytond_sale_blanket_agreement-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/hu.po` & `trytond_sale_blanket_agreement-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/id.po` & `trytond_sale_blanket_agreement-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/it.po` & `trytond_sale_blanket_agreement-7.2.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 msgctxt "field:sale.blanket_agreement.line,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.blanket_agreement.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
 msgctxt "field:sale.blanket_agreement.line,processed_quantity:"
 msgid "Processed quantity"
 msgstr ""
 
 msgctxt "field:sale.blanket_agreement.line,product:"
 msgid "Product"
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/lo.po` & `trytond_sale_blanket_agreement-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/lt.po` & `trytond_sale_blanket_agreement-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/nl.po` & `trytond_sale_blanket_agreement-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/pl.po` & `trytond_sale_blanket_agreement-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/pt.po` & `trytond_sale_blanket_agreement-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/ro.po` & `trytond_sale_blanket_agreement-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/ru.po` & `trytond_sale_blanket_agreement-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/sl.po` & `trytond_sale_blanket_agreement-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/tr.po` & `trytond_sale_blanket_agreement-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/uk.po` & `trytond_sale_blanket_agreement-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/locale/zh_CN.po` & `trytond_sale_blanket_agreement-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/message.xml` & `trytond_sale_blanket_agreement-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/product.xml` & `trytond_sale_blanket_agreement-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/sale.py` & `trytond_sale_blanket_agreement-7.2.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import functools
 from decimal import Decimal
 from itertools import groupby
 
+from sql import Null
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Workflow, fields
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits, round_price
 from trytond.modules.product.exceptions import UOMValidationError
@@ -247,15 +248,17 @@
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_currency(cls, **pattern):
         pool = Pool()
         Company = pool.get('company.company')
         company = pattern.get('company')
         if not company:
@@ -280,14 +283,28 @@
             amount = self.currency.round(amount)
         return amount
 
     @classmethod
     def default_state(cls):
         return 'draft'
 
+    @property
+    def full_number(self):
+        return self.number
+
+    def get_rec_name(self, name):
+        items = []
+        if self.full_number:
+            items.append(self.full_number)
+        if self.reference:
+            items.append('[%s]' % self.reference)
+        if not items:
+            items.append('(%s)' % self.id)
+        return ' '.join(items)
+
     @classmethod
     def search_rec_name(cls, name, clause):
         _, operator, value = clause
         if operator.startswith('!') or operator.startswith('not '):
             bool_op = 'AND'
         else:
             bool_op = 'OR'
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/sale.xml` & `trytond_sale_blanket_agreement-7.2.0/sale.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_sale_blanket_agreement-7.0.0/sale.xml` & `trytond_sale_blanket_agreement-7.2.0/sale.xml`

```diff
@@ -73,64 +73,64 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_sale_blanket_agreement"/>
     </record>
     <menuitem parent="sale.menu_sale" action="act_sale_blanket_agreement" sequence="20" id="menu_sale_blanket_agreement"/>
     <record model="ir.model.button" id="sale_blanket_agreement_cancel_button">
+      <field name="model">sale.blanket_agreement</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="sale_blanket_agreement_draft_button">
+      <field name="model">sale.blanket_agreement</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="sale_blanket_agreement_run_button">
+      <field name="model">sale.blanket_agreement</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="sale_blanket_agreement_create_sale_button">
+      <field name="model">sale.blanket_agreement</field>
       <field name="name">create_sale</field>
       <field name="string">Create a sale</field>
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="sale_blanket_agreement_close_button">
+      <field name="model">sale.blanket_agreement</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
     </record>
     <record model="ir.model.access" id="access_sale_blanket_agreement">
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
+      <field name="model">sale.blanket_agreement</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_sale_blanket_agreement_for_group_sale">
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
+      <field name="model">sale.blanket_agreement</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_sale_blanket_agreement_for_group_sale_blanket_agreement">
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
+      <field name="model">sale.blanket_agreement</field>
       <field name="group" ref="group_sale_blanket_agreement"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sale_blanket_agreement_companies">
       <field name="name">Sales Blanket Agreement</field>
-      <field name="model" search="[('model', '=', 'sale.blanket_agreement')]"/>
+      <field name="model">sale.blanket_agreement</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sale_blanket_agreement_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sale_blanket_agreement_companies"/>
     </record>
     <record model="ir.ui.view" id="sale_blanket_agreement_line_view_form">
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/setup.py` & `trytond_sale_blanket_agreement-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
-            'https://docs.tryton.org/projects/modules-sale-blanket-agreement',
+            'https://docs.tryton.org/modules-sale-blanket-agreement',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton, blanket agreement, sale',
     package_dir={'trytond.modules.sale_blanket_agreement': '.'},
     packages=(
         ['trytond.modules.sale_blanket_agreement']
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/tests/scenario_sale_blanket_agreement.rst` & `trytond_sale_blanket_agreement-7.2.0/tests/scenario_sale_blanket_agreement.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 ===============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> later = today + dt.timedelta(days=30)
 
 Activate modules::
 
     >>> config = activate_modules('sale_blanket_agreement')
@@ -101,16 +99,15 @@
     1
     >>> create_sale.form.lines[0].remaining_quantity
     20.0
     >>> create_sale.execute('create_sale')
     >>> sale, = create_sale.actions[0]
 
     >>> line, = sale.lines
-    >>> line.product == product1
-    True
+    >>> assertEqual(line.product, product1)
     >>> line.quantity
     20.0
     >>> line.unit_price
     Decimal('9.0000')
     >>> line.quantity = 5.0
     >>> line.save()
 
@@ -131,25 +128,25 @@
     15.0
 
 Try to change product with incompatible unit::
 
     >>> blanket_agreement.click('draft')
     >>> line, = blanket_agreement.lines
     >>> line.product = product2
-    >>> blanket_agreement.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> blanket_agreement.save()
     Traceback (most recent call last):
         ...
     UOMValidationError: ...
 
     >>> blanket_agreement.reload()
     >>> blanket_agreement.click('run')
 
 Try to close blanket agreement with remaining quantity::
 
-    >>> blanket_agreement.click('close')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> blanket_agreement.click('close')
     Traceback (most recent call last):
         ...
     BlanketAgreementClosingWarning: ...
 
 Try to sale more than remaining::
 
 
@@ -160,15 +157,15 @@
     Decimal('10.0000')
     >>> sale_line.blanket_agreement_line = blanket_agreement_line
     >>> sale_line.quantity
     15.0
     >>> sale_line.unit_price
     Decimal('9.0000')
     >>> sale_line.quantity = 20
-    >>> sale.click('quote')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.click('quote')
     Traceback (most recent call last):
         ...
     BlanketAgreementQuantityWarning: ...
 
 Sale remaining quantity::
 
     >>> sale_line, = sale.lines
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/tox.ini` & `trytond_sale_blanket_agreement-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO` & `trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-sale-blanket-agreement
-Version: 7.0.0
+Name: trytond_sale_blanket_agreement
+Version: 7.2.0
 Summary: Tryton module for sale blanket agreement
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-blanket-agreement
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-blanket-agreement
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton,blanket agreement,sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,17 +49,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_sale_blanket_agreement-7.0.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt` & `trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt`

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

### Comparing `trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_form.xml` & `trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.0.0/view/sale_blanket_agreement_line_form.xml` & `trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_line_form.xml`

 * *Files identical despite different names*

