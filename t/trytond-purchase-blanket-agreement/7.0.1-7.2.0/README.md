# Comparing `tmp/trytond_purchase_blanket_agreement-7.0.1.tar.gz` & `tmp/trytond_purchase_blanket_agreement-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_blanket_agreement-7.0.1.tar", last modified: Sat Feb  3 11:25:26 2024, max compression
+gzip compressed data, was "trytond_purchase_blanket_agreement-7.2.0.tar", last modified: Mon Apr 29 15:45:40 2024, max compression
```

## Comparing `trytond_purchase_blanket_agreement-7.0.1.tar` & `trytond_purchase_blanket_agreement-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:25:26.206912 trytond_purchase_blanket_agreement-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-02-03 11:25:23.000000 trytond_purchase_blanket_agreement-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-02-03 11:25:23.000000 trytond_purchase_blanket_agreement-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2764 2024-02-03 11:25:26.206912 trytond_purchase_blanket_agreement-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:25:26.200245 trytond_purchase_blanket_agreement-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1686 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:25:26.203578 trytond_purchase_blanket_agreement-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7774 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7827 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7838 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7784 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6718 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7900 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    32146 2024-01-26 18:05:24.000000 trytond_purchase_blanket_agreement-7.0.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12122 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:25:26.206912 trytond_purchase_blanket_agreement-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4833 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:25:26.203578 trytond_purchase_blanket_agreement-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5671 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/tests/scenario_purchase_blanket_agreement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-10-30 17:55:12.000000 trytond_purchase_blanket_agreement-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:25:26.206912 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2764 2024-02-03 11:25:25.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2423 2024-02-03 11:25:26.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:25:25.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-03 11:25:25.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:01.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-02-03 11:25:25.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:25:25.000000 trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:25:26.206912 trytond_purchase_blanket_agreement-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/product_list_agreement_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_create_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-10-30 17:06:38.000000 trytond_purchase_blanket_agreement-7.0.1/view/purchase_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:23:34.000000 trytond_purchase_blanket_agreement-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-29 15:23:34.000000 trytond_purchase_blanket_agreement-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.261215 trytond_purchase_blanket_agreement-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_purchase_blanket_agreement-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1686 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:20.000000 trytond_purchase_blanket_agreement-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.261215 trytond_purchase_blanket_agreement-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7774 2024-04-27 16:43:26.000000 trytond_purchase_blanket_agreement-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7827 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7838 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7784 2024-04-27 16:43:26.000000 trytond_purchase_blanket_agreement-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6718 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7900 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32617 2024-04-22 12:14:36.000000 trytond_purchase_blanket_agreement-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11915 2024-04-27 16:30:39.000000 trytond_purchase_blanket_agreement-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4824 2024-04-27 16:30:39.000000 trytond_purchase_blanket_agreement-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5537 2024-04-22 12:14:36.000000 trytond_purchase_blanket_agreement-7.2.0/tests/scenario_purchase_blanket_agreement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-22 12:14:36.000000 trytond_purchase_blanket_agreement-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:20.000000 trytond_purchase_blanket_agreement-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-04-29 15:23:30.000000 trytond_purchase_blanket_agreement-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2405 2024-04-29 15:45:40.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/product_list_agreement_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_create_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_line_list.xml
```

### Comparing `trytond_purchase_blanket_agreement-7.0.1/COPYRIGHT` & `trytond_purchase_blanket_agreement-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/LICENSE` & `trytond_purchase_blanket_agreement-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/PKG-INFO` & `trytond_purchase_blanket_agreement-7.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_blanket_agreement
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for purchase blanket agreement
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase-blanket-agreement
+Project-URL: Documentation, https://docs.tryton.org/modules-purchase-blanket-agreement
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://hg.tryton.org/modules/purchase_blanket_agreement
 Keywords: tryton,blanket agreement,purchase
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
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_purchase_blanket_agreement-7.0.1/__init__.py` & `trytond_purchase_blanket_agreement-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/doc/conf.py` & `trytond_purchase_blanket_agreement-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase_blanket_agreement-7.0.1/doc/design.rst` & `trytond_purchase_blanket_agreement-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/bg.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/ca.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/cs.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/de.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/es.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/es_419.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/et.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/fa.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/fi.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/fr.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/hu.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/id.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/it.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/lo.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/lt.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/nl.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/pl.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/pt.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/ro.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/ru.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/sl.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/tr.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/uk.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/locale/zh_CN.po` & `trytond_purchase_blanket_agreement-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/message.xml` & `trytond_purchase_blanket_agreement-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/product.xml` & `trytond_purchase_blanket_agreement-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/purchase.py` & `trytond_purchase_blanket_agreement-7.2.0/purchase.py`

 * *Files 2% similar despite different names*

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
@@ -246,15 +247,17 @@
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.state == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_currency(cls, **pattern):
         pool = Pool()
         Company = pool.get('company.company')
         company = pattern.get('company')
         if not company:
@@ -279,14 +282,28 @@
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

### Comparing `trytond_purchase_blanket_agreement-7.0.1/purchase.xml` & `trytond_purchase_blanket_agreement-7.2.0/purchase.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_purchase_blanket_agreement-7.0.1/purchase.xml` & `trytond_purchase_blanket_agreement-7.2.0/purchase.xml`

```diff
@@ -73,64 +73,64 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_purchase_blanket_agreement"/>
     </record>
     <menuitem parent="purchase.menu_purchase" action="act_purchase_blanket_agreement" sequence="20" id="menu_purchase_blanket_agreement"/>
     <record model="ir.model.button" id="purchase_blanket_agreement_cancel_button">
+      <field name="model">purchase.blanket_agreement</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="purchase_blanket_agreement_draft_button">
+      <field name="model">purchase.blanket_agreement</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="purchase_blanket_agreement_run_button">
+      <field name="model">purchase.blanket_agreement</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="purchase_blanket_agreement_create_purchase_button">
+      <field name="model">purchase.blanket_agreement</field>
       <field name="name">create_purchase</field>
       <field name="string">Create a Purchase</field>
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
     </record>
     <record model="ir.model.button" id="purchase_blanket_agreement_close_button">
+      <field name="model">purchase.blanket_agreement</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
     </record>
     <record model="ir.model.access" id="access_purchase_blanket_agreement">
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
+      <field name="model">purchase.blanket_agreement</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_blanket_agreement_group_purchase">
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
+      <field name="model">purchase.blanket_agreement</field>
       <field name="group" ref="purchase.group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_blanket_agreement_group_purchase_blanket_agreement">
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
+      <field name="model">purchase.blanket_agreement</field>
       <field name="group" ref="group_purchase_blanket_agreement"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_purchase_blanket_agreement_companies">
       <field name="name">Purchases Blanket Agreement</field>
-      <field name="model" search="[('model', '=', 'purchase.blanket_agreement')]"/>
+      <field name="model">purchase.blanket_agreement</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_purchase_blanket_agreement_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_purchase_blanket_agreement_companies"/>
     </record>
     <record model="ir.ui.view" id="purchase_blanket_agreement_line_view_form">
```

### Comparing `trytond_purchase_blanket_agreement-7.0.1/setup.py` & `trytond_purchase_blanket_agreement-7.2.0/setup.py`

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
-            'https://docs.tryton.org/projects/modules-purchase-blanket-agreement',  # noqa: E501
+            'https://docs.tryton.org/modules-purchase-blanket-agreement',  # noqa: E501
         "Forum": 'https://www.tryton.org/forum',
         "Source Code":
             'https://hg.tryton.org/modules/purchase_blanket_agreement',
         },
     keywords='tryton, blanket agreement, purchase',
     package_dir={'trytond.modules.purchase_blanket_agreement': '.'},
     packages=(
```

### Comparing `trytond_purchase_blanket_agreement-7.0.1/tests/scenario_purchase_blanket_agreement.rst` & `trytond_purchase_blanket_agreement-7.2.0/tests/scenario_purchase_blanket_agreement.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 ===================================
 
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
 
@@ -105,16 +103,15 @@
     1
     >>> create_purchase.form.lines[0].remaining_quantity
     20.0
     >>> create_purchase.execute('create_purchase')
     >>> purchase, = create_purchase.actions[0]
 
     >>> line, = purchase.lines
-    >>> line.product == product1
-    True
+    >>> assertEqual(line.product, product1)
     >>> line.quantity
     20.0
     >>> line.unit_price
     Decimal('7.0000')
     >>> line.quantity = 5.0
     >>> line.save()
 
@@ -135,25 +132,25 @@
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
 
 Try to purchase more than remaining::
 
     >>> purchase = Purchase(party=supplier)
@@ -163,15 +160,15 @@
     Decimal('8.0000')
     >>> purchase_line.blanket_agreement_line = blanket_agreement_line
     >>> purchase_line.quantity
     15.0
     >>> purchase_line.unit_price
     Decimal('7.0000')
     >>> purchase_line.quantity = 20
-    >>> purchase.click('quote')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> purchase.click('quote')
     Traceback (most recent call last):
         ...
     BlanketAgreementQuantityWarning: ...
 
 Purchase remaining quantity::
 
     >>> purchase_line, = purchase.lines
```

### Comparing `trytond_purchase_blanket_agreement-7.0.1/tox.ini` & `trytond_purchase_blanket_agreement-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/PKG-INFO` & `trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_blanket_agreement
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for purchase blanket agreement
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase-blanket-agreement
+Project-URL: Documentation, https://docs.tryton.org/modules-purchase-blanket-agreement
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://hg.tryton.org/modules/purchase_blanket_agreement
 Keywords: tryton,blanket agreement,purchase
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
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_purchase_blanket_agreement-7.0.1/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt` & `trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_form.xml` & `trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_line_form.xml` & `trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.0.1/view/purchase_blanket_agreement_line_list.xml` & `trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_list.xml`

 * *Files identical despite different names*

