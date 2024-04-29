# Comparing `tmp/trytond_product_price_list_dates-7.0.0.tar.gz` & `tmp/trytond_product_price_list_dates-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_price_list_dates-7.0.0.tar", last modified: Mon Oct 30 17:33:27 2023, max compression
+gzip compressed data, was "trytond_product_price_list_dates-7.2.0.tar", last modified: Mon Apr 29 15:43:46 2024, max compression
```

## Comparing `trytond_product_price_list_dates-7.0.0.tar` & `trytond_product_price_list_dates-7.2.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:27.206467 trytond_product_price_list_dates-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-10-22 17:23:10.000000 trytond_product_price_list_dates-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1591 2023-10-30 17:09:23.000000 trytond_product_price_list_dates-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:09:23.000000 trytond_product_price_list_dates-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2727 2023-10-30 17:33:27.206467 trytond_product_price_list_dates-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:27.203134 trytond_product_price_list_dates-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-10-22 17:23:10.000000 trytond_product_price_list_dates-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:10.000000 trytond_product_price_list_dates-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:27.203134 trytond_product_price_list_dates-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      696 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      838 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      746 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      748 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-28 12:11:23.000000 trytond_product_price_list_dates-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3498 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3729 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      743 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:33:27.206467 trytond_product_price_list_dates-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4729 2023-10-27 17:38:49.000000 trytond_product_price_list_dates-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:27.203134 trytond_product_price_list_dates-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5239 2023-10-07 15:40:36.000000 trytond_product_price_list_dates-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_price_list_dates-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-10-30 17:09:20.000000 trytond_product_price_list_dates-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:27.206467 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2727 2023-10-30 17:33:26.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1901 2023-10-30 17:33:27.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:26.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2023-10-30 17:33:26.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      178 2023-10-30 17:33:26.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:33:26.000000 trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:27.203134 trytond_product_price_list_dates-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:21.000000 trytond_product_price_list_dates-7.0.0/view/price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.0.0/view/price_list_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.0.0/view/price_list_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.0.0/view/price_list_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.0.0/view/price_list_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.0.0/view/product_sale_context_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1692 2024-04-29 15:22:20.000000 trytond_product_price_list_dates-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:22:19.000000 trytond_product_price_list_dates-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2727 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:46.830849 trytond_product_price_list_dates-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3087 2024-04-27 16:30:39.000000 trytond_product_price_list_dates-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:17.000000 trytond_product_price_list_dates-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      696 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      838 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      746 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      748 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2024-04-27 16:43:25.000000 trytond_product_price_list_dates-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3498 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2024-04-27 16:30:39.000000 trytond_product_price_list_dates-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      743 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4729 2024-03-17 11:01:36.000000 trytond_product_price_list_dates-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5239 2024-02-04 18:51:26.000000 trytond_product_price_list_dates-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:17.000000 trytond_product_price_list_dates-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-29 15:22:15.000000 trytond_product_price_list_dates-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2727 2024-04-29 15:43:46.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1883 2024-04-29 15:43:46.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:46.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-04-29 15:43:46.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      178 2024-04-29 15:43:46.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:46.000000 trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:46.834182 trytond_product_price_list_dates-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:21.000000 trytond_product_price_list_dates-7.2.0/view/price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.2.0/view/price_list_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.2.0/view/price_list_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.2.0/view/price_list_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-7.2.0/view/price_list_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-7.2.0/view/product_sale_context_form.xml
```

### Comparing `trytond_product_price_list_dates-7.0.0/CHANGELOG` & `trytond_product_price_list_dates-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_product_price_list_dates-7.0.0/COPYRIGHT` & `trytond_product_price_list_dates-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2023 Cédric Krier
-Copyright (C) 2017-2023 B2CK
+Copyright (C) 2017-2024 Cédric Krier
+Copyright (C) 2017-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_price_list_dates-7.0.0/LICENSE` & `trytond_product_price_list_dates-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/PKG-INFO` & `trytond_product_price_list_dates-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list_dates
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add dates on price list
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
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_product_price_list_cache<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_price_list<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_price_list<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_product_price_list_cache<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_price_list<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2; extra == "test"
 
 Product Price List Dates Module
 ###############################
 
 The *Product Price List Dates Module* adds date range condition to the price
 list lines.
```

### Comparing `trytond_product_price_list_dates-7.0.0/__init__.py` & `trytond_product_price_list_dates-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/doc/conf.py` & `trytond_product_price_list_dates-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_price_list_dates-7.0.0/doc/design.rst` & `trytond_product_price_list_dates-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/bg.po` & `trytond_product_price_list_dates-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/ca.po` & `trytond_product_price_list_dates-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/cs.po` & `trytond_product_price_list_dates-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/de.po` & `trytond_product_price_list_dates-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/es.po` & `trytond_product_price_list_dates-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/es_419.po` & `trytond_product_price_list_dates-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/et.po` & `trytond_product_price_list_dates-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/fa.po` & `trytond_product_price_list_dates-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/fi.po` & `trytond_product_price_list_dates-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/fr.po` & `trytond_product_price_list_dates-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/hu.po` & `trytond_product_price_list_dates-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/id.po` & `trytond_product_price_list_dates-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/it.po` & `trytond_product_price_list_dates-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/lo.po` & `trytond_product_price_list_dates-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/lt.po` & `trytond_product_price_list_dates-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/nl.po` & `trytond_product_price_list_dates-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/pl.po` & `trytond_product_price_list_dates-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/pt.po` & `trytond_product_price_list_dates-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/ro.po` & `trytond_product_price_list_dates-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/ru.po` & `trytond_product_price_list_dates-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/sl.po` & `trytond_product_price_list_dates-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/tr.po` & `trytond_product_price_list_dates-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/uk.po` & `trytond_product_price_list_dates-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/locale/zh_CN.po` & `trytond_product_price_list_dates-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/product.py` & `trytond_product_price_list_dates-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/product.xml` & `trytond_product_price_list_dates-7.2.0/product.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_product_price_list_dates-7.0.0/product.xml` & `trytond_product_price_list_dates-7.2.0/product.xml`

```diff
@@ -5,17 +5,17 @@
   <data>
     <record model="ir.ui.view" id="price_list_view_form">
       <field name="model">product.price_list</field>
       <field name="inherit" ref="product_price_list.price_list_view_form"/>
       <field name="name">price_list_form</field>
     </record>
     <record model="ir.model.button" id="price_list_open_lines_button">
+      <field name="model">product.price_list</field>
       <field name="name">open_lines</field>
       <field name="string">Open Lines</field>
-      <field name="model" search="[('model', '=', 'product.price_list')]"/>
     </record>
     <record model="ir.ui.view" id="price_list_line_view_form">
       <field name="model">product.price_list.line</field>
       <field name="inherit" ref="product_price_list.price_list_line_view_form"/>
       <field name="name">price_list_line_form</field>
     </record>
     <record model="ir.ui.view" id="price_list_line_view_tree">
```

### Comparing `trytond_product_price_list_dates-7.0.0/purchase.py` & `trytond_product_price_list_dates-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/sale.py` & `trytond_product_price_list_dates-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/setup.py` & `trytond_product_price_list_dates-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/tests/test_module.py` & `trytond_product_price_list_dates-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/tox.ini` & `trytond_product_price_list_dates-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/PKG-INFO` & `trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-price-list-dates
-Version: 7.0.0
+Name: trytond_product_price_list_dates
+Version: 7.2.0
 Summary: Tryton module to add dates on price list
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
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_product_price_list_cache<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_price_list<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_price_list<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_product_price_list_cache<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_price_list<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2; extra == "test"
 
 Product Price List Dates Module
 ###############################
 
 The *Product Price List Dates Module* adds date range condition to the price
 list lines.
```

### Comparing `trytond_product_price_list_dates-7.0.0/trytond_product_price_list_dates.egg-info/SOURCES.txt` & `trytond_product_price_list_dates-7.2.0/trytond_product_price_list_dates.egg-info/SOURCES.txt`

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
 product.py
```
