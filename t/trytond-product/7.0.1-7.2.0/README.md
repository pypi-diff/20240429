# Comparing `tmp/trytond_product-7.0.1.tar.gz` & `tmp/trytond_product-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product-7.0.1.tar", last modified: Sat Dec 16 10:04:42 2023, max compression
+gzip compressed data, was "trytond_product-7.2.0.tar", last modified: Mon Apr 29 15:42:21 2024, max compression
```

## Comparing `trytond_product-7.0.1.tar` & `trytond_product-7.2.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.786575 trytond_product-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-30 17:06:38.000000 trytond_product-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     5376 2023-12-16 10:04:40.000000 trytond_product-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-12-16 10:04:40.000000 trytond_product-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_product-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_product-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2831 2023-12-16 10:04:42.786575 trytond_product-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_product-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-10-30 17:06:38.000000 trytond_product-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-10-30 17:06:38.000000 trytond_product-7.0.1/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-10-30 17:06:38.000000 trytond_product-7.0.1/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2064 2023-10-30 17:06:38.000000 trytond_product-7.0.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2558 2023-10-30 17:06:38.000000 trytond_product-7.0.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.779908 trytond_product-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5486 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-10-30 17:06:38.000000 trytond_product-7.0.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_product-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.779908 trytond_product-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_product-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-10-30 17:06:38.000000 trytond_product-7.0.1/icons/tryton-product.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-10-30 17:06:38.000000 trytond_product-7.0.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.783241 trytond_product-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    24996 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26388 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22448 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26809 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26635 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22475 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23000 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24422 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22383 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26611 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25122 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22098 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23216 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25465 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24117 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26440 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26272 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23582 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26050 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25236 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23581 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23677 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21311 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24924 2023-10-30 17:06:38.000000 trytond_product-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1904 2023-10-30 17:06:38.000000 trytond_product-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28292 2023-12-10 21:35:03.000000 trytond_product-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10515 2023-10-30 17:06:38.000000 trytond_product-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-12-16 10:04:42.786575 trytond_product-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4584 2023-10-30 17:06:38.000000 trytond_product-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.783241 trytond_product-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_product-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1262 2023-10-30 17:06:38.000000 trytond_product-7.0.1/tests/scenario_product_identifier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2123 2023-12-10 21:35:03.000000 trytond_product-7.0.1/tests/scenario_product_variant.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    22022 2023-10-30 17:06:38.000000 trytond_product-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_product-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_product-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-10-30 17:55:12.000000 trytond_product-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.786575 trytond_product-7.0.1/trytond_product.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2831 2023-12-16 10:04:42.000000 trytond_product-7.0.1/trytond_product.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2778 2023-12-16 10:04:42.000000 trytond_product-7.0.1/trytond_product.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-12-16 10:04:42.000000 trytond_product-7.0.1/trytond_product.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-12-16 10:04:42.000000 trytond_product-7.0.1/trytond_product.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:53.000000 trytond_product-7.0.1/trytond_product.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      122 2023-12-16 10:04:42.000000 trytond_product-7.0.1/trytond_product.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-12-16 10:04:42.000000 trytond_product-7.0.1/trytond_product.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    10730 2023-10-30 17:06:38.000000 trytond_product-7.0.1/uom.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17035 2023-10-30 17:06:38.000000 trytond_product-7.0.1/uom.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:04:42.786575 trytond_product-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/category_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1133 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/product_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/product_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/product_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/uom_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/uom_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/uom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_product-7.0.1/view/uom_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.546413 trytond_product-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5565 2024-04-29 15:21:14.000000 trytond_product-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:21:13.000000 trytond_product-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2822 2024-04-29 15:42:21.546413 trytond_product-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-27 16:30:39.000000 trytond_product-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1087 2024-04-27 16:30:39.000000 trytond_product-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3875 2024-04-27 16:30:39.000000 trytond_product-7.2.0/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5393 2024-04-27 16:30:39.000000 trytond_product-7.2.0/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2310 2024-04-27 16:30:39.000000 trytond_product-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-27 16:30:39.000000 trytond_product-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.539746 trytond_product-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_product-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-15 07:12:15.000000 trytond_product-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5486 2024-01-27 09:58:52.000000 trytond_product-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-27 16:30:39.000000 trytond_product-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1011 2024-04-27 16:30:39.000000 trytond_product-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:14.000000 trytond_product-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-04-15 07:12:15.000000 trytond_product-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_product-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.543079 trytond_product-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_product-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_product-7.2.0/icons/tryton-product.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_product-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.543079 trytond_product-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    24996 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26388 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22448 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26809 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26635 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22475 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23000 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24422 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22383 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26611 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25122 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22098 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23216 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25465 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24117 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26440 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26272 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23582 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25936 2024-04-29 13:17:17.000000 trytond_product-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25236 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23581 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23677 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21311 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24924 2024-04-27 16:43:24.000000 trytond_product-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2072 2024-04-27 16:30:39.000000 trytond_product-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    30204 2024-04-27 16:30:39.000000 trytond_product-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10469 2024-04-27 16:30:39.000000 trytond_product-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:21.546413 trytond_product-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:30:39.000000 trytond_product-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.543079 trytond_product-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1182 2024-04-22 12:14:36.000000 trytond_product-7.2.0/tests/scenario_product_identifier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-04-22 12:14:36.000000 trytond_product-7.2.0/tests/scenario_product_variant.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    22022 2024-01-27 09:58:52.000000 trytond_product-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:14.000000 trytond_product-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-29 15:21:09.000000 trytond_product-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.546413 trytond_product-7.2.0/trytond_product.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2822 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_product-7.2.0/trytond_product.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      122 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:21.000000 trytond_product-7.2.0/trytond_product.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    10730 2024-02-04 18:51:26.000000 trytond_product-7.2.0/uom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16944 2024-04-27 16:30:39.000000 trytond_product-7.2.0/uom.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:21.546413 trytond_product-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      661 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1133 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/product_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1416 2024-04-27 16:30:39.000000 trytond_product-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_product-7.2.0/view/uom_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/uom_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-01-16 14:00:20.000000 trytond_product-7.2.0/view/uom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product-7.2.0/view/uom_tree.xml
```

### Comparing `trytond_product-7.0.1/CHANGELOG` & `trytond_product-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 
-Version 7.0.1 - 2023-12-16
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
+* Add Manufacturer Part Number product identifier
+* Add brand product identifier
+* Support generate barcode of different type
+* Add code on product category
+* Add product deactivable mixins
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_product-7.0.1/COPYRIGHT` & `trytond_product-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 Copyright (C) 2004-2008 Tiny SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_product-7.0.1/LICENSE` & `trytond_product-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/PKG-INFO` & `trytond_product-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_product
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module with products
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product/
+Project-URL: Documentation, https://docs.tryton.org/modules-product/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -50,19 +50,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
 Requires-Dist: python-stdnum
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond[barcode]<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond[barcode]<7.3,>=7.2; extra == "test"
 
 ##############
 Product Module
 ##############
 
 The *Product Module* defines the essential concepts needed to describe
 products in Tryton.
```

### Comparing `trytond_product-7.0.1/category.xml` & `trytond_product-7.2.0/category.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_product-7.0.1/category.xml` & `trytond_product-7.2.0/category.xml`

```diff
@@ -65,28 +65,39 @@
     </record>
     <record model="ir.action.act_window.view" id="act_category_product_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="category_view_form_product"/>
       <field name="act_window" ref="act_category_product"/>
     </record>
     <record model="ir.model.button" id="category_add_products_button">
+      <field name="model">product.category</field>
       <field name="name">add_products</field>
       <field name="string">Add products</field>
-      <field name="model" search="[('model', '=', 'product.category')]"/>
     </record>
     <record model="ir.model.access" id="access_product_category">
-      <field name="model" search="[('model', '=', 'product.category')]"/>
+      <field name="model">product.category</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_product_category_admin">
-      <field name="model" search="[('model', '=', 'product.category')]"/>
+      <field name="model">product.category</field>
       <field name="group" ref="group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
+    <record model="ir.sequence.type" id="sequence_type_category">
+      <field name="name">Category</field>
+    </record>
+    <record model="ir.sequence.type-res.group" id="sequence_type_category_group_admin">
+      <field name="sequence_type" ref="sequence_type_category"/>
+      <field name="group" ref="res.group_admin"/>
+    </record>
+    <record model="ir.sequence.type-res.group" id="sequence_type_category_group_product_admin">
+      <field name="sequence_type" ref="sequence_type_category"/>
+      <field name="group" ref="group_product_admin"/>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_product-7.0.1/configuration.py` & `trytond_product-7.2.0/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,20 @@
             ],
         help="Used to generate the last part of the product code.")
     template_sequence = fields.Many2One('ir.sequence', "Product Sequence",
         domain=[
             ('sequence_type', '=', Id('product', 'sequence_type_template')),
             ],
         help="Used to generate the first part of the product code.")
+    category_sequence = fields.Many2One(
+        'ir.sequence', "Category Sequence",
+        domain=[
+            ('sequence_type', '=', Id('product', 'sequence_type_category')),
+            ],
+        help="Used to generate the category code.")
 
     @classmethod
     def default_default_cost_price_method(cls, **pattern):
         return cls.multivalue_model(
             'default_cost_price_method').default_default_cost_price_method()
```

### Comparing `trytond_product-7.0.1/configuration.xml` & `trytond_product-7.2.0/configuration.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_product-7.0.1/configuration.xml` & `trytond_product-7.2.0/configuration.xml`

```diff
@@ -19,22 +19,22 @@
     </record>
     <menuitem parent="menu_configuration" action="act_product_configuration_form" sequence="10" id="menu_product_configuration" icon="tryton-list"/>
     <record model="ir.ui.menu-res.group" id="menu_product_configuration_group_product_admin">
       <field name="menu" ref="menu_product_configuration"/>
       <field name="group" ref="group_product_admin"/>
     </record>
     <record model="ir.model.access" id="access_product_configuration">
-      <field name="model" search="[('model', '=', 'product.configuration')]"/>
+      <field name="model">product.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_product_configuration_product_admin">
-      <field name="model" search="[('model', '=', 'product.configuration')]"/>
+      <field name="model">product.configuration</field>
       <field name="group" ref="group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_product-7.0.1/doc/conf.py` & `trytond_product-7.2.0/doc/conf.py`

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

### Comparing `trytond_product-7.0.1/doc/configuration.rst` & `trytond_product-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/doc/design.rst` & `trytond_product-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/doc/usage.rst` & `trytond_product-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/icons/LICENSE` & `trytond_product-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/ir.py` & `trytond_product-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/bg.po` & `trytond_product-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/ca.po` & `trytond_product-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/cs.po` & `trytond_product-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/de.po` & `trytond_product-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/es.po` & `trytond_product-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/es_419.po` & `trytond_product-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/et.po` & `trytond_product-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/fa.po` & `trytond_product-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/fi.po` & `trytond_product-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/fr.po` & `trytond_product-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/hu.po` & `trytond_product-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/id.po` & `trytond_product-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/it.po` & `trytond_product-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/lo.po` & `trytond_product-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/lt.po` & `trytond_product-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/nl.po` & `trytond_product-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/pl.po` & `trytond_product-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/pt.po` & `trytond_product-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/ro.po` & `trytond_product-7.2.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -123,23 +123,21 @@
 msgid "Cost Price"
 msgstr "Cost"
 
 msgctxt "field:product.product,cost_prices:"
 msgid "Cost Prices"
 msgstr "Costuri"
 
-#, fuzzy
 msgctxt "field:product.product,default_uom:"
 msgid "Default UoM"
 msgstr "UM Implicita"
 
-#, fuzzy
 msgctxt "field:product.product,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Categorie implicita al UM"
+msgstr "Categorie Implicita UM"
 
 msgctxt "field:product.product,description:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:product.product,identifiers:"
 msgid "Identifiers"
@@ -205,23 +203,21 @@
 msgid "Cost Price Method"
 msgstr "Metoda a pretului de cost"
 
 msgctxt "field:product.template,cost_price_methods:"
 msgid "Cost Price Methods"
 msgstr "Metode Pret cost"
 
-#, fuzzy
 msgctxt "field:product.template,default_uom:"
 msgid "Default UoM"
 msgstr "UM Implicita"
 
-#, fuzzy
 msgctxt "field:product.template,default_uom_category:"
 msgid "Default UoM Category"
-msgstr "Categorie implicita al UM"
+msgstr "Categorie Implicita UM"
 
 msgctxt "field:product.template,list_price:"
 msgid "List Price"
 msgstr "Lista de preturi"
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
@@ -345,27 +341,25 @@
 "Suma de cost pentru a achiziționa sau a produce varianta, sau a efectua "
 "serviciul."
 
 msgctxt "help:product.product,cost_price_method:"
 msgid "The method used to calculate the cost price."
 msgstr "Metoda utilizată pentru calcularea a costului."
 
-#, fuzzy
 msgctxt "help:product.product,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
-"Unitatea standard de măsură pentru produs.\n"
-"Folosit intern la calcularea nivelului stocului de bunuri și active."
+"Unitatea standard de măsură pentru produsul.\n"
+"Folosit intern la calcularea nivelului stocului de marfă și active."
 
-#, fuzzy
 msgctxt "help:product.product,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Categorii de unități de măsură"
+msgstr "Categoria Unităţii de Măsura implicite."
 
 msgctxt "help:product.product,identifiers:"
 msgid "Other identifiers associated with the variant."
 msgstr "Alți identificatori asociați cu varianta."
 
 msgctxt "help:product.product,list_price:"
 msgid "The standard price the product is sold at."
@@ -403,27 +397,25 @@
 "Sumă care costă achiziţia sau producţia produsului, sau pentru a executa "
 "serviciul."
 
 msgctxt "help:product.template,cost_price_method:"
 msgid "The method used to calculate the cost price."
 msgstr "Metoda utilizată pentru calcularea a costului."
 
-#, fuzzy
 msgctxt "help:product.template,default_uom:"
 msgid ""
 "The standard Unit of Measure for the product.\n"
 "Used internally when calculating the stock levels of goods and assets."
 msgstr ""
 "Unitatea standard de măsură pentru produs.\n"
-"Folosit intern la calcularea nivelului stocului de bunuri și active."
+"Folosit intern la calcularea nivelului stocului de marfuri și active."
 
-#, fuzzy
 msgctxt "help:product.template,default_uom_category:"
 msgid "The category of the default Unit of Measure."
-msgstr "Categorii de unități de măsură"
+msgstr "Categora Unităţii de Măsura implicite."
 
 msgctxt "help:product.template,list_price:"
 msgid "The standard price the product is sold at."
 msgstr "Prețul standard la care se vinde produsul."
 
 msgctxt "help:product.template,products:"
 msgid "The different variants the product comes in."
@@ -509,47 +501,41 @@
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "%(type)s \"%(code)s\" nu este valabil pentru produsul \"%(product)s\"."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "Codul al unui produs activ trebuie să fie unic."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_decrease_digits"
 msgid "You cannot decrease the digits of the unit of measure \"%(uom)s\"."
 msgstr "Nu se pot reduce zecimalele al UM \"%(uom)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_incompatible_factor_rate"
 msgid "Incompatible factor and rate values on unit of measure\"%(uom)s\"."
 msgstr "Factor şi rata incompatibil pentru UM \"%(uom)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_category"
 msgid "You cannot modify the category of the unit of measure \"%(uom)s\"."
 msgstr "Categoria de UM nu se poate modifica \"%(uom)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_factor"
 msgid "You cannot modify the factor of the unit of measure \"%(uom)s\"."
 msgstr "Nu se poate modifica factorul Unităţii de Masură \"%(uom)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_options"
 msgid ""
 "If the unit of measure is still not used, you can delete it otherwise you "
 "can deactivate it and create a new one."
 msgstr ""
 "Dacă UM nu este utilizată se poate şterge, altfel se poate dezactiva în "
 "vedere creării unei noi UM."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_modify_rate"
 msgid "You cannot modify the rate of the unit of measure\"%(uom)s\"."
-msgstr "Nu se poate modifică rate al UM \"%(uom)s\"."
+msgstr "Nu se poate modifică rata al UM \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_no_zero_factor_rate"
 msgid "Rate and factor can not be both equal to zero."
 msgstr "Rata şi factor nu pot ambele sa fii egale cu zero."
 
 msgctxt "model:ir.model.button,string:category_add_products_button"
 msgid "Add products"
```

### Comparing `trytond_product-7.0.1/locale/ru.po` & `trytond_product-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/sl.po` & `trytond_product-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/tr.po` & `trytond_product-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/uk.po` & `trytond_product-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/locale/zh_CN.po` & `trytond_product-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/message.xml` & `trytond_product-7.2.0/message.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_product-7.0.1/message.xml` & `trytond_product-7.2.0/message.xml`

```diff
@@ -26,9 +26,12 @@
     </record>
     <record model="ir.message" id="msg_invalid_code">
       <field name="text">The %(type)s &quot;%(code)s&quot; for product &quot;%(product)s&quot; is not valid.</field>
     </record>
     <record model="ir.message" id="msg_product_code_unique">
       <field name="text">Code of active product must be unique.</field>
     </record>
+    <record model="ir.message" id="msg_category_code_unique">
+      <field name="text">The code on product category must be unique.</field>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_product-7.0.1/product.py` & `trytond_product-7.2.0/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import logging
 from decimal import Decimal
 from importlib import import_module
 
 import stdnum
 import stdnum.exceptions
 from sql import Literal
+from sql.conditionals import Coalesce
 from sql.functions import CharLength
 from sql.operators import Equal
 
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Exclude, Index, Model, ModelSQL, ModelView, UnionMixin,
     fields, sequence_ordered)
 from trytond.modules.company.model import (
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.pool import Pool
-from trytond.pyson import Eval, Get, If
+from trytond.pyson import Eval, Get
 from trytond.tools import is_full_text, lstrip_wildcard
 from trytond.transaction import Transaction
 
 try:
     from trytond.tools import barcode
 except ImportError:
     barcode = None
@@ -110,17 +111,14 @@
         help="The categories that the product is in.\n"
         "Used to group similar products together.")
     categories_all = fields.Many2Many(
         'product.template-product.category.all',
         'template', 'category', "Categories", readonly=True)
     products = fields.One2Many(
         'product.product', 'template', "Variants",
-        domain=[
-            If(~Eval('active'), ('active', '=', False), ()),
-            ],
         help="The different variants the product comes in.")
 
     @classmethod
     def __setup__(cls):
         cls.code.search_unaccented = False
         super().__setup__()
         t = cls.__table__()
@@ -318,26 +316,79 @@
         Template = pool.get('product.template')
         definition = super().definition(model, language)
         definition['searchable'] = self._field.definition(
             Template, language)['searchable']
         return definition
 
 
+class TemplateDeactivatableMixin(DeactivableMixin):
+    __slots__ = ()
+
+    @classmethod
+    def _active_expression(cls, tables):
+        pool = Pool()
+        Template = pool.get('product.template')
+        table, _ = tables[None]
+        if 'template' not in tables:
+            template = Template.__table__()
+            tables['template'] = {
+                None: (template, table.template == template.id),
+                }
+        else:
+            template, _ = tables['template'][None]
+        return table.active & template.active
+
+    @classmethod
+    def domain_active(cls, domain, tables):
+        expression = cls._active_expression(tables)
+        _, operator, value = domain
+        if operator in {'=', '!='}:
+            if (operator == '=') != value:
+                expression = ~expression
+        elif operator in {'in', 'not in'}:
+            if True in value and False not in value:
+                pass
+            elif False in value and True not in value:
+                expression = ~expression
+            else:
+                expression = Literal(True)
+        else:
+            expression = Literal(True)
+        return expression
+
+
+class ProductDeactivatableMixin(TemplateDeactivatableMixin):
+    __slots__ = ()
+
+    @classmethod
+    def _active_expression(cls, tables):
+        pool = Pool()
+        Product = pool.get('product.product')
+        table, _ = tables[None]
+        if 'product' not in tables:
+            product = Product.__table__()
+            tables['product'] = {
+                None: (product, table.product == product.id),
+                }
+        else:
+            product, _ = tables['product'][None]
+        expression = super()._active_expression(tables)
+        return expression & Coalesce(product.active, expression)
+
+
 class Product(
-        DeactivableMixin, ModelSQL, ModelView, CompanyMultiValueMixin):
+        TemplateDeactivatableMixin, ModelSQL, ModelView,
+        CompanyMultiValueMixin):
     "Product Variant"
     __name__ = "product.product"
     _order_name = 'rec_name'
     template = fields.Many2One(
         'product.template', "Product Template",
         required=True, ondelete='CASCADE',
         search_context={'default_products': False},
-        domain=[
-            If(Eval('active'), ('active', '=', True), ()),
-            ],
         help="The product that defines the common properties "
         "inherited by the variant.")
     code_readonly = fields.Function(fields.Boolean('Code Readonly'),
         'get_code_readonly')
     prefix_code = fields.Function(fields.Char(
             "Prefix Code",
             states={
@@ -528,16 +579,14 @@
         Template = pool.get('product.template')
         product, _ = tables[None]
         if 'template' not in tables:
             template = Template.__table__()
             tables['template'] = {
                 None: (template, product.template == template.id),
                 }
-        else:
-            template = tables['template']
         return cls.order_code(tables) + Template.name.convert_order('name',
             tables['template'], Template)
 
     def get_rec_name(self, name):
         if self.code:
             return '[' + self.code + '] ' + self.name
         else:
@@ -751,14 +800,16 @@
             (None, ''),
             ('ean', "International Article Number"),
             ('isan', "International Standard Audiovisual Number"),
             ('isbn', "International Standard Book Number"),
             ('isil', "International Standard Identifier for Libraries"),
             ('isin', "International Securities Identification Number"),
             ('ismn', "International Standard Music Number"),
+            ('brand', "Brand"),
+            ('mpn', "Manufacturer Part Number"),
             ], "Type")
     type_string = type.translated('type')
     code = fields.Char("Code", required=True)
 
     @classmethod
     def __setup__(cls):
         cls.code.search_unaccented = False
@@ -768,33 +819,38 @@
         cls._sql_indexes.update({
                 Index(
                     t,
                     (t.product, Index.Equality()),
                     (t.code, Index.Similarity())),
                 })
 
-    @fields.depends('type', 'code')
+    @property
+    @fields.depends('type')
+    def _is_stdnum(self):
+        return self.type in {'ean', 'isan', 'isbn', 'isil', 'isin', 'ismn'}
+
+    @fields.depends('type', 'code', methods=['_is_stdnum'])
     def on_change_with_code(self):
-        if self.type and self.type != 'other':
+        if self._is_stdnum:
             try:
                 module = import_module('stdnum.%s' % self.type)
                 return module.compact(self.code)
             except ImportError:
                 pass
             except stdnum.exceptions.ValidationError:
                 pass
         return self.code
 
     def pre_validate(self):
         super().pre_validate()
         self.check_code()
 
-    @fields.depends('type', 'product', 'code')
+    @fields.depends('type', 'product', 'code', methods=['_is_stdnum'])
     def check_code(self):
-        if self.type:
+        if self._is_stdnum:
             try:
                 module = import_module('stdnum.%s' % self.type)
             except ModuleNotFoundError:
                 return
             if not module.is_valid(self.code):
                 if self.product and self.product.id > 0:
                     product = self.product.rec_name
@@ -802,11 +858,13 @@
                     product = ''
                 raise InvalidIdentifierCode(
                     gettext('product.msg_invalid_code',
                         type=self.type_string,
                         code=self.code,
                         product=product))
 
-    def barcode(self, format='svg', **options):
-        if barcode and self.type in barcode.BARCODES:
+    def barcode(self, format='svg', type=None, **options):
+        if type is None:
+            type = self.type
+        if barcode and type in barcode.BARCODES:
             generator = getattr(barcode, 'generate_%s' % format)
-            return generator(self.type, self.on_change_with_code(), **options)
+            return generator(type, self.on_change_with_code(), **options)
```

### Comparing `trytond_product-7.0.1/product.xml` & `trytond_product-7.2.0/product.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_product-7.0.1/product.xml` & `trytond_product-7.2.0/product.xml`

```diff
@@ -105,22 +105,22 @@
     <record model="ir.action.act_window.view" id="act_product_form_view">
       <field name="sequence" eval="20"/>
       <field name="view" ref="product_view_form"/>
       <field name="act_window" ref="act_product_form"/>
     </record>
     <menuitem parent="menu_template" action="act_product_form" sequence="10" id="menu_product" icon="tryton-list"/>
     <record model="ir.model.access" id="access_product_template">
-      <field name="model" search="[('model', '=', 'product.template')]"/>
+      <field name="model">product.template</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_product_template_admin">
-      <field name="model" search="[('model', '=', 'product.template')]"/>
+      <field name="model">product.template</field>
       <field name="group" ref="group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.act_window" id="act_product_from_template">
```

### Comparing `trytond_product-7.0.1/setup.py` & `trytond_product-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-product/',
+        "Documentation": 'https://docs.tryton.org/modules-product/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product',
     package_dir={'trytond.modules.product': '.'},
     packages=(
         ['trytond.modules.product']
```

### Comparing `trytond_product-7.0.1/tests/scenario_product_identifier.rst` & `trytond_product-7.2.0/tests/scenario_product_identifier.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 ===========================
 Product Identifier Scenario
 ===========================
 
 Imports::
 
-    >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('product')
 
 Create product::
@@ -30,15 +29,15 @@
     >>> identifier.type = 'ean'
     >>> identifier.code = '123 456 7890 123'
     >>> identifier.code
     '1234567890123'
 
 An Error is raised for invalid code::
 
-    >>> product.save() # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> product.save()
     Traceback (most recent call last):
         ...
     InvalidIdentifierCode: ...
 
 Valid codes are saved correctly::
 
     >>> identifier.code = '978-0-471-11709-4'
```

### Comparing `trytond_product-7.0.1/tests/scenario_product_variant.rst` & `trytond_product-7.2.0/tests/scenario_product_variant.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ========================
 Product Variant Scenario
 ========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('product')
 
 Create company::
```

### Comparing `trytond_product-7.0.1/tests/test_module.py` & `trytond_product-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/tox.ini` & `trytond_product-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/trytond_product.egg-info/PKG-INFO` & `trytond_product-7.2.0/trytond_product.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-product
-Version: 7.0.1
+Name: trytond_product
+Version: 7.2.0
 Summary: Tryton module with products
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product/
+Project-URL: Documentation, https://docs.tryton.org/modules-product/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -50,19 +50,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
 Requires-Dist: python-stdnum
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond[barcode]<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond[barcode]<7.3,>=7.2; extra == "test"
 
 ##############
 Product Module
 ##############
 
 The *Product Module* defines the essential concepts needed to describe
 products in Tryton.
```

### Comparing `trytond_product-7.0.1/trytond_product.egg-info/SOURCES.txt` & `trytond_product-7.2.0/trytond_product.egg-info/SOURCES.txt`

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
 category.py
@@ -80,14 +79,15 @@
 ./view/uom_category_tree.xml
 ./view/uom_form.xml
 ./view/uom_tree.xml
 doc/conf.py
 doc/configuration.rst
 doc/design.rst
 doc/index.rst
+doc/reference.rst
 doc/releases.rst
 doc/requirements-doc.txt
 doc/usage.rst
 icons/LICENSE
 icons/tryton-product.svg
 locale/bg.po
 locale/ca.po
```

### Comparing `trytond_product-7.0.1/uom.py` & `trytond_product-7.2.0/uom.py`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/uom.xml` & `trytond_product-7.2.0/uom.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_product-7.0.1/uom.xml` & `trytond_product-7.2.0/uom.xml`

```diff
@@ -49,14 +49,44 @@
     </record>
     <record model="ir.action.act_window.view" id="act_uom_category_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="uom_category_view_form"/>
       <field name="act_window" ref="act_uom_category_form"/>
     </record>
     <menuitem parent="menu_uom_form" action="act_uom_category_form" sequence="20" id="menu_uom_category_form"/>
+    <record model="ir.model.access" id="access_uom">
+      <field name="model">product.uom</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
+    <record model="ir.model.access" id="access_uom_admin">
+      <field name="model">product.uom</field>
+      <field name="group" ref="group_product_admin"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="True"/>
+      <field name="perm_create" eval="True"/>
+      <field name="perm_delete" eval="True"/>
+    </record>
+    <record model="ir.model.access" id="access_uom_category">
+      <field name="model">product.uom.category</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+      <field name="perm_create" eval="False"/>
+      <field name="perm_delete" eval="False"/>
+    </record>
+    <record model="ir.model.access" id="access_uom_category_admin">
+      <field name="model">product.uom.category</field>
+      <field name="group" ref="group_product_admin"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="True"/>
+      <field name="perm_create" eval="True"/>
+      <field name="perm_delete" eval="True"/>
+    </record>
   </data>
   <data noupdate="1">
     <record model="product.uom.category" id="uom_cat_unit">
       <field name="name">Units</field>
     </record>
     <record model="product.uom" id="uom_unit">
       <field name="name">Unit</field>
@@ -319,39 +349,9 @@
     <record model="product.uom" id="uom_energy_mwh">
       <field name="name">Megawatt-hour</field>
       <field name="symbol">MW⋅h</field>
       <field name="category" ref="uom_cat_energy"/>
       <field name="factor" eval="3_600_000_000"/>
       <field name="rate" eval="round(1.0 / 3_600_000_000, 12)"/>
     </record>
-    <record model="ir.model.access" id="access_uom">
-      <field name="model" search="[('model', '=', 'product.uom')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_uom_admin">
-      <field name="model" search="[('model', '=', 'product.uom')]"/>
-      <field name="group" ref="group_product_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
-    <record model="ir.model.access" id="access_uom_category">
-      <field name="model" search="[('model', '=', 'product.uom.category')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_uom_category_admin">
-      <field name="model" search="[('model', '=', 'product.uom.category')]"/>
-      <field name="group" ref="group_product_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
   </data>
 </tryton>
```

### Comparing `trytond_product-7.0.1/view/category_form.xml` & `trytond_product-7.2.0/view/category_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_product-7.0.1/view/category_form.xml` & `trytond_product-7.2.0/view/category_form.xml`

```diff
@@ -1,18 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form>
+<form col="6">
   <label name="name"/>
   <field name="name"/>
-  <label name="parent"/>
-  <field name="parent"/>
+  <label name="code"/>
+  <field name="code"/>
   <group colspan="2" col="-1" id="checkboxes">
     <!-- Add here some checkboxes ! -->
   </group>
-  <button name="add_products" colspan="2"/>
-  <notebook colspan="4">
+  <label name="parent"/>
+  <field name="parent" colspan="3"/>
+  <button name="add_products" colspan="6"/>
+  <notebook colspan="6">
     <page string="Children" col="1" id="childs">
       <field name="childs"/>
     </page>
   </notebook>
 </form>
```

### Comparing `trytond_product-7.0.1/view/product_form.xml` & `trytond_product-7.2.0/view/product_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/view/product_form_simple.xml` & `trytond_product-7.2.0/view/product_form_simple.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-7.0.1/view/uom_form.xml` & `trytond_product-7.2.0/view/uom_form.xml`

 * *Files identical despite different names*

