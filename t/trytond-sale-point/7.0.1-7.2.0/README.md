# Comparing `tmp/trytond_sale_point-7.0.1.tar.gz` & `tmp/trytond_sale_point-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_point-7.0.1.tar", last modified: Fri Dec  1 23:18:30 2023, max compression
+gzip compressed data, was "trytond_sale_point-7.2.0.tar", last modified: Mon Apr 29 15:48:34 2024, max compression
```

## Comparing `trytond_sale_point-7.0.1.tar` & `trytond_sale_point-7.2.0.tar`

### file list

```diff
@@ -1,90 +1,89 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-01 23:18:30.835889 trytond_sale_point-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-12-01 23:18:28.000000 trytond_sale_point-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-12-01 23:18:28.000000 trytond_sale_point-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-12-01 23:18:30.835889 trytond_sale_point-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-01 23:18:30.832555 trytond_sale_point-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-01 23:18:30.825888 trytond_sale_point-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17180 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17599 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17213 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17447 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14481 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14156 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17048 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14071 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14063 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45545 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24915 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-11-27 22:53:13.000000 trytond_sale_point-7.0.1/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-12-01 23:18:30.835889 trytond_sale_point-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4584 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-01 23:18:30.829222 trytond_sale_point-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5832 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/scenario_sale_point.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3674 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/scenario_sale_point_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4456 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/scenario_sale_point_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5000 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/scenario_sale_point_session.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3928 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/scenario_sale_point_tax_excluded.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-10-30 17:55:12.000000 trytond_sale_point-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-01 23:18:30.832555 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-12-01 23:18:30.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2023-12-01 23:18:30.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-12-01 23:18:30.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-12-01 23:18:30.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:08.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-12-01 23:18:30.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-12-01 23:18:30.000000 trytond_sale_point-7.0.1/trytond_sale_point.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-01 23:18:30.832555 trytond_sale_point-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/cash_session_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/cash_session_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/cash_transfer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/cash_transfer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/cash_transfer_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/cash_transfer_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/payment_form_wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/payment_method_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      799 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/point_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/sale_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/sale_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_sale_point-7.0.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-29 15:25:42.000000 trytond_sale_point-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:25:42.000000 trytond_sale_point-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.273331 trytond_sale_point-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_sale_point-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:26.000000 trytond_sale_point-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-09-24 17:12:47.000000 trytond_sale_point-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.276664 trytond_sale_point-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17180 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17599 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17213 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17447 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14481 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14168 2024-04-29 13:17:17.000000 trytond_sale_point-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17048 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14071 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14063 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2024-02-04 18:51:26.000000 trytond_sale_point-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45634 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24271 2024-04-27 16:30:39.000000 trytond_sale_point-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2024-03-17 11:01:36.000000 trytond_sale_point-7.2.0/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:30:39.000000 trytond_sale_point-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.276664 trytond_sale_point-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5830 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3643 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4447 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4928 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_session.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3900 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_tax_excluded.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:26.000000 trytond_sale_point-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-29 15:25:38.000000 trytond_sale_point-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2919 2024-04-29 15:48:34.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_session_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_session_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_transfer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_transfer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-02-04 18:51:26.000000 trytond_sale_point-7.2.0/view/cash_transfer_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_transfer_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_form_wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_method_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      799 2024-02-04 18:51:26.000000 trytond_sale_point-7.2.0/view/point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/point_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-09-24 17:12:47.000000 trytond_sale_point-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/sale_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/sale_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/template_tree.xml
```

### Comparing `trytond_sale_point-7.0.1/CHANGELOG` & `trytond_sale_point-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2023-12-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_point-7.0.1/LICENSE` & `trytond_sale_point-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/PKG-INFO` & `trytond_sale_point-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale_point
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-point/
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-point/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton POS sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,24 +49,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #################
 Sale Point Module
 #################
 
 The *Sale Point Module* allows retail sales to be handled and recorded.
```

### Comparing `trytond_sale_point-7.0.1/__init__.py` & `trytond_sale_point-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/account.py` & `trytond_sale_point-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/doc/conf.py` & `trytond_sale_point-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_point-7.0.1/doc/design.rst` & `trytond_sale_point-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/bg.po` & `trytond_sale_point-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/ca.po` & `trytond_sale_point-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/cs.po` & `trytond_sale_point-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/de.po` & `trytond_sale_point-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/es.po` & `trytond_sale_point-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/es_419.po` & `trytond_sale_point-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/et.po` & `trytond_sale_point-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/fa.po` & `trytond_sale_point-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/fi.po` & `trytond_sale_point-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/fr.po` & `trytond_sale_point-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/hu.po` & `trytond_sale_point-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/id.po` & `trytond_sale_point-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/it.po` & `trytond_sale_point-7.2.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 msgctxt "field:sale.point.cash.transfer,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.point.cash.transfer,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
 msgctxt "field:sale.point.cash.transfer,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:sale.point.cash.transfer,move:"
 msgid "Move"
@@ -280,15 +280,15 @@
 
 msgctxt "field:sale.point.sale.line,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:sale.point.sale.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
 msgctxt "field:sale.point.sale.line,moves:"
 msgid "Moves"
 msgstr "Movimenti"
 
 msgctxt "field:sale.point.sale.line,product:"
 msgid "Product"
```

### Comparing `trytond_sale_point-7.0.1/locale/lo.po` & `trytond_sale_point-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/lt.po` & `trytond_sale_point-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/nl.po` & `trytond_sale_point-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/pl.po` & `trytond_sale_point-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/pt.po` & `trytond_sale_point-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/ro.po` & `trytond_sale_point-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/ru.po` & `trytond_sale_point-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/sl.po` & `trytond_sale_point-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/tr.po` & `trytond_sale_point-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/uk.po` & `trytond_sale_point-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/locale/zh_CN.po` & `trytond_sale_point-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/message.xml` & `trytond_sale_point-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/product.py` & `trytond_sale_point-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/product.xml` & `trytond_sale_point-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/sale.py` & `trytond_sale_point-7.2.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from collections import defaultdict
 from decimal import Decimal
 
-from sql import Literal, Union
+from sql import Literal, Null, Union
 from sql.aggregate import Sum
 from sql.conditionals import Coalesce
 from sql.functions import CharLength
 from sql.operators import Equal
 
 from trytond.i18n import gettext
 from trytond.model import (
@@ -204,15 +204,17 @@
                 'depends': ['state'],
                 },
             )
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def default_employee(cls):
```

### Comparing `trytond_sale_point-7.0.1/sale.xml` & `trytond_sale_point-7.2.0/sale.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_sale_point-7.0.1/sale.xml` & `trytond_sale_point-7.2.0/sale.xml`

```diff
@@ -50,39 +50,39 @@
     <record model="ir.action.act_window.view" id="act_point_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="point_view_form"/>
       <field name="act_window" ref="act_point_form"/>
     </record>
     <menuitem parent="sale.menu_configuration" action="act_point_form" sequence="10" id="menu_point_form"/>
     <record model="ir.model.access" id="access_point">
-      <field name="model" search="[('model', '=', 'sale.point')]"/>
+      <field name="model">sale.point</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_point_sale_point">
-      <field name="model" search="[('model', '=', 'sale.point')]"/>
+      <field name="model">sale.point</field>
       <field name="group" ref="group_sale_point"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_point_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.point')]"/>
+      <field name="model">sale.point</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_point_sale_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.point')]"/>
+      <field name="model">sale.point</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_point_sale_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_point_sale_companies"/>
     </record>
     <record model="ir.ui.view" id="sale_view_form">
@@ -129,61 +129,61 @@
     </record>
     <menuitem parent="sale.menu_sale" action="act_sale_form" sequence="10" id="menu_sale_form"/>
     <record model="ir.ui.menu-res.group" id="menu_sale_form_group_sale_point">
       <field name="menu" ref="menu_sale_form"/>
       <field name="group" ref="group_sale_point"/>
     </record>
     <record model="ir.model.access" id="access_sale">
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
+      <field name="model">sale.point.sale</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_sale_sale_point">
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
+      <field name="model">sale.point.sale</field>
       <field name="group" ref="group_sale_point"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="sale_pay_button">
+      <field name="model">sale.point.sale</field>
       <field name="name">pay</field>
       <field name="string">Pay</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_cancel_button">
+      <field name="model">sale.point.sale</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_open_button">
+      <field name="model">sale.point.sale</field>
       <field name="name">open</field>
       <field name="string">Re-Open</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_process_button">
+      <field name="model">sale.point.sale</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_post_button">
+      <field name="model">sale.point.sale</field>
       <field name="name">post</field>
       <field name="string">Post</field>
       <field name="confirm">Are you sure you want to post the sales?</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_post_button_group_sale_point_posting">
       <field name="button" ref="sale_post_button"/>
       <field name="group" ref="group_sale_point_posting"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sale_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
+      <field name="model">sale.point.sale</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sale_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sale_companies"/>
     </record>
     <record model="ir.ui.view" id="sale_line_view_form">
@@ -236,51 +236,51 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_cash_session_form"/>
     </record>
     <menuitem parent="sale.menu_sale" action="act_cash_session_form" sequence="20" id="menu_cash_session_form"/>
     <record model="ir.model.access" id="access_cash_session">
-      <field name="model" search="[('model', '=', 'sale.point.cash.session')]"/>
+      <field name="model">sale.point.cash.session</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_cash_session_sale_point">
-      <field name="model" search="[('model', '=', 'sale.point.cash.session')]"/>
+      <field name="model">sale.point.cash.session</field>
       <field name="group" ref="group_sale_point"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="cash_session_open_button">
+      <field name="model">sale.point.cash.session</field>
       <field name="name">open</field>
       <field name="string">Re-Open</field>
-      <field name="model" search="[('model', '=', 'sale.point.cash.session')]"/>
     </record>
     <record model="ir.model.button" id="cash_session_close_button">
+      <field name="model">sale.point.cash.session</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'sale.point.cash.session')]"/>
     </record>
     <record model="ir.model.button" id="cash_session_post_button">
+      <field name="model">sale.point.cash.session</field>
       <field name="name">post</field>
       <field name="string">Post</field>
       <field name="confirm">Are you sure you want to post the sessions?</field>
-      <field name="model" search="[('model', '=', 'sale.point.cash.session')]"/>
     </record>
     <record model="ir.model.button-res.group" id="cash_session_post_button_group_sale_point_posting">
       <field name="button" ref="cash_session_post_button"/>
       <field name="group" ref="group_sale_point_posting"/>
     </record>
     <record model="ir.rule.group" id="rule_group_cash_session_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.point.sale')]"/>
+      <field name="model">sale.point.sale</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_cash_session_companies">
       <field name="domain" eval="[('point.company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_cash_session_companies"/>
     </record>
     <record model="ir.ui.view" id="payment_method_view_form">
@@ -305,31 +305,31 @@
     <record model="ir.action.act_window.view" id="act_payment_method_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="payment_method_view_form"/>
       <field name="act_window" ref="act_payment_method_form"/>
     </record>
     <menuitem parent="sale.menu_configuration" action="act_payment_method_form" sequence="50" id="menu_payment_method_form"/>
     <record model="ir.model.access" id="access_payment_method">
-      <field name="model" search="[('model', '=', 'sale.point.payment.method')]"/>
+      <field name="model">sale.point.payment.method</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_method_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.point.payment.method')]"/>
+      <field name="model">sale.point.payment.method</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_payment_method_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.point.payment.method')]"/>
+      <field name="model">sale.point.payment.method</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_method_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_payment_method_companies"/>
     </record>
     <record model="ir.ui.view" id="payment_view_form">
@@ -360,41 +360,41 @@
     </record>
     <record model="ir.ui.view" id="cash_transfer_view_list">
       <field name="model">sale.point.cash.transfer</field>
       <field name="type">tree</field>
       <field name="name">cash_transfer_list</field>
     </record>
     <record model="ir.model.access" id="access_cash_transfer">
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer')]"/>
+      <field name="model">sale.point.cash.transfer</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_cash_transfer_sale_point">
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer')]"/>
+      <field name="model">sale.point.cash.transfer</field>
       <field name="group" ref="group_sale_point"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="cash_transfer_post_button">
+      <field name="model">sale.point.cash.transfer</field>
       <field name="name">post</field>
       <field name="string">Post</field>
       <field name="confirm">Are you sure you want to post the transfer?</field>
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer')]"/>
     </record>
     <record model="ir.model.button-res.group" id="cash_transfer_post_button_group_sale_point_posting">
       <field name="button" ref="cash_transfer_post_button"/>
       <field name="group" ref="group_sale_point_posting"/>
     </record>
     <record model="ir.rule.group" id="rule_group_cash_transfer_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer')]"/>
+      <field name="model">sale.point.cash.transfer</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_cash_transfer_companies">
       <field name="domain" eval="[('point.company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_cash_transfer_companies"/>
     </record>
     <record model="ir.ui.view" id="cash_transfer_type_view_form">
@@ -419,31 +419,31 @@
     <record model="ir.action.act_window.view" id="act_cash_transfer_type_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="cash_transfer_type_view_form"/>
       <field name="act_window" ref="act_cash_transfer_type_form"/>
     </record>
     <menuitem parent="sale.menu_configuration" action="act_cash_transfer_type_form" sequence="50" id="menu_cash_transfer_type_form"/>
     <record model="ir.model.access" id="access_cash_transfer_type">
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer.type')]"/>
+      <field name="model">sale.point.cash.transfer.type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_cash_transfer_type_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer.type')]"/>
+      <field name="model">sale.point.cash.transfer.type</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_cash_transfer_type_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.point.cash.transfer.type')]"/>
+      <field name="model">sale.point.cash.transfer.type</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_cash_transfer_type_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_cash_transfer_type_companies"/>
     </record>
   </data>
```

### Comparing `trytond_sale_point-7.0.1/sale_reporting.py` & `trytond_sale_point-7.2.0/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/setup.py` & `trytond_sale_point-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-sale-point/'),
+            'https://docs.tryton.org/modules-sale-point/'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton POS sale',
     package_dir={'trytond.modules.sale_point': '.'},
     packages=(
         ['trytond.modules.sale_point']
```

### Comparing `trytond_sale_point-7.0.1/tests/scenario_sale_point.rst` & `trytond_sale_point-7.2.0/tests/scenario_sale_point.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 POS Scenario
 ============
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax)
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_point')
 
     >>> Journal = Model.get('account.journal')
     >>> Location = Model.get('stock.location')
@@ -158,16 +157,15 @@
     >>> payment = sale.click('pay')
     >>> payment.form.method = terminal_method
     >>> payment.form.amount
     Decimal('6036.00')
     >>> payment.form.amount = Decimal('6100.00')
     >>> payment.execute('pay')
 
-    >>> payment.form.method == cash_method
-    True
+    >>> assertEqual(payment.form.method, cash_method)
     >>> payment.form.amount
     Decimal('-64.00')
     >>> payment.execute('pay')
 
     >>> sale.state
     'done'
 
@@ -178,22 +176,19 @@
     'posted'
 
 Check stock move::
 
     >>> move, = StockMove.find([
     ...     ('origin.sale', '=', sale.id, 'sale.point.sale.line')
     ...     ])
-    >>> move.product == goods
-    True
+    >>> assertEqual(move.product, goods)
     >>> move.quantity
     500.0
-    >>> move.from_location == storage_loc
-    True
-    >>> move.to_location == customer_loc
-    True
+    >>> assertEqual(move.from_location, storage_loc)
+    >>> assertEqual(move.to_location, customer_loc)
     >>> move.state
     'done'
 
 Check account move::
 
     >>> bool(sale.move)
     True
```

### Comparing `trytond_sale_point-7.0.1/tests/scenario_sale_point_reporting.rst` & `trytond_sale_point-7.2.0/tests/scenario_sale_point_reporting.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 POS Reporting Scenario
 ======================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale_point')
 
     >>> Journal = Model.get('account.journal')
     >>> Location = Model.get('stock.location')
@@ -118,9 +117,9 @@
     >>> with config.set_context(context=context):
     ...     reports = Reporting.find([])
     >>> len(reports)
     1
     >>> report, = reports
     >>> report.number
     1
-    >>> report.revenue == Decimal('12.00')
-    True
+    >>> report.revenue
+    Decimal('12.00')
```

### Comparing `trytond_sale_point-7.0.1/tests/scenario_sale_point_return.rst` & `trytond_sale_point-7.2.0/tests/scenario_sale_point_return.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 POS Scenario Return
 ===================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_point')
 
 Get models::
 
@@ -139,20 +138,17 @@
     >>> sale.state
     'posted'
 
 Check stock move::
 
     >>> line, = sale.lines
     >>> move, = line.moves
-    >>> move.product == goods
-    True
-    >>> move.from_location == customer_loc
-    True
-    >>> move.to_location == input_loc
-    True
+    >>> assertEqual(move.product, goods)
+    >>> assertEqual(move.from_location, customer_loc)
+    >>> assertEqual(move.to_location, input_loc)
     >>> move.state
     'done'
 
 Check account move::
 
     >>> bool(sale.move)
     True
```

### Comparing `trytond_sale_point-7.0.1/tests/scenario_sale_point_session.rst` & `trytond_sale_point-7.2.0/tests/scenario_sale_point_session.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 POS Session Scenario
 ====================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale_point')
 
     >>> Journal = Model.get('account.journal')
     >>> Location = Model.get('stock.location')
@@ -165,15 +164,15 @@
     >>> session.start_amount
     Decimal('100.00')
     >>> session.balance
     Decimal('20.00')
 
 Try to close::
 
-    >>> session.click('close')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> session.click('close')
     Traceback (most recent call last):
         ...
     SessionValidationError: ...
 
     >>> session.end_amount = Decimal('120.00')
     >>> session.click('close')
     >>> session.state
```

### Comparing `trytond_sale_point-7.0.1/tests/scenario_sale_point_tax_excluded.rst` & `trytond_sale_point-7.2.0/tests/scenario_sale_point_tax_excluded.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 POS Scenario
 ============
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard, Report
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('sale_point')
 
 Get models::
```

### Comparing `trytond_sale_point-7.0.1/tox.ini` & `trytond_sale_point-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/trytond_sale_point.egg-info/PKG-INFO` & `trytond_sale_point-7.2.0/trytond_sale_point.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-sale-point
-Version: 7.0.1
+Name: trytond_sale_point
+Version: 7.2.0
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-point/
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-point/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton POS sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,24 +49,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #################
 Sale Point Module
 #################
 
 The *Sale Point Module* allows retail sales to be handled and recorded.
```

### Comparing `trytond_sale_point-7.0.1/trytond_sale_point.egg-info/SOURCES.txt` & `trytond_sale_point-7.2.0/trytond_sale_point.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_sale_point-7.0.1/view/cash_session_form.xml` & `trytond_sale_point-7.2.0/view/cash_session_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/view/cash_transfer_form.xml` & `trytond_sale_point-7.2.0/view/cash_transfer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/view/point_form.xml` & `trytond_sale_point-7.2.0/view/point_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/view/sale_form.xml` & `trytond_sale_point-7.2.0/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.0.1/view/sale_line_form.xml` & `trytond_sale_point-7.2.0/view/sale_line_form.xml`

 * *Files identical despite different names*

