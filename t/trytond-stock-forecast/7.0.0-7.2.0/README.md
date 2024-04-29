# Comparing `tmp/trytond_stock_forecast-7.0.0.tar.gz` & `tmp/trytond_stock_forecast-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_forecast-7.0.0.tar", last modified: Mon Oct 30 17:41:30 2023, max compression
+gzip compressed data, was "trytond_stock_forecast-7.2.0.tar", last modified: Mon Apr 29 15:50:56 2024, max compression
```

## Comparing `trytond_stock_forecast-7.0.0.tar` & `trytond_stock_forecast-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:30.058770 trytond_stock_forecast-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:23.000000 trytond_stock_forecast-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2919 2023-10-30 17:14:08.000000 trytond_stock_forecast-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:14:07.000000 trytond_stock_forecast-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_forecast-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2023-10-30 17:41:30.058770 trytond_stock_forecast-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-08-13 15:26:13.000000 trytond_stock_forecast-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:30.058770 trytond_stock_forecast-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:23.000000 trytond_stock_forecast-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:23.000000 trytond_stock_forecast-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21817 2023-10-24 07:56:52.000000 trytond_stock_forecast-7.0.0/forecast.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6362 2023-10-27 17:38:49.000000 trytond_stock_forecast-7.0.0/forecast.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:30.055437 trytond_stock_forecast-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5450 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5330 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5465 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5327 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4513 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4884 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5610 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5373 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4908 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4605 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4895 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5294 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4668 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5281 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4853 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5134 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4460 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5638 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5041 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4635 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4406 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4690 2023-10-30 16:47:45.000000 trytond_stock_forecast-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      777 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-08-13 15:26:13.000000 trytond_stock_forecast-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:41:30.058770 trytond_stock_forecast-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4303 2023-10-27 17:38:49.000000 trytond_stock_forecast-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:30.055437 trytond_stock_forecast-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14564 2023-10-24 07:56:52.000000 trytond_stock_forecast-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_forecast-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      135 2023-10-30 17:14:04.000000 trytond_stock_forecast-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:30.058770 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2023-10-30 17:41:29.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1763 2023-10-30 17:41:30.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:41:29.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:41:29.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2023-10-30 17:41:29.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:41:29.000000 trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:30.058770 trytond_stock_forecast-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-08-13 15:26:13.000000 trytond_stock_forecast-7.0.0/view/forecast_complete_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      915 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.0.0/view/forecast_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-24 07:56:52.000000 trytond_stock_forecast-7.0.0/view/forecast_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-24 07:56:52.000000 trytond_stock_forecast-7.0.0/view/forecast_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-08-13 15:26:13.000000 trytond_stock_forecast-7.0.0/view/forecast_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-08-13 15:26:13.000000 trytond_stock_forecast-7.0.0/view/product_list_forecast.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.839602 trytond_stock_forecast-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3749 2024-04-29 15:27:34.000000 trytond_stock_forecast-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:27:33.000000 trytond_stock_forecast-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_forecast-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.832936 trytond_stock_forecast-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:32.000000 trytond_stock_forecast-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22210 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/forecast.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6201 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/forecast.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5450 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5330 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5465 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5327 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4513 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4884 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5610 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5373 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4908 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4895 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5294 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4668 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5281 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4853 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5134 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4460 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5638 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5041 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4406 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4690 2024-04-27 16:43:27.000000 trytond_stock_forecast-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      777 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:56.839602 trytond_stock_forecast-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4462 2024-04-27 16:30:39.000000 trytond_stock_forecast-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14575 2024-04-22 12:14:37.000000 trytond_stock_forecast-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:32.000000 trytond_stock_forecast-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-04-29 15:27:29.000000 trytond_stock_forecast-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1777 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      126 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:56.000000 trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:56.836269 trytond_stock_forecast-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/view/forecast_complete_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      915 2023-04-15 07:12:15.000000 trytond_stock_forecast-7.2.0/view/forecast_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-02-04 18:51:26.000000 trytond_stock_forecast-7.2.0/view/forecast_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-02-04 18:51:26.000000 trytond_stock_forecast-7.2.0/view/forecast_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/view/forecast_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-01-27 09:58:52.000000 trytond_stock_forecast-7.2.0/view/product_list_forecast.xml
```

### Comparing `trytond_stock_forecast-7.0.0/CHANGELOG` & `trytond_stock_forecast-7.2.0/CHANGELOG`

 * *Files 22% similar despite different names*

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
 * Rename UOM to Unit for forecast line
 
 Version 6.8.0 - 2023-05-01
@@ -13,100 +18,127 @@
 * Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
 * Remove support for Python 3.6
 
 Version 6.2.0 - 2021-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.0.0 - 2021-05-03
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 * Rename forecast state from cancel to cancelled
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.0.0 - 2018-10-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 2.7
 
 Version 4.8.0 - 2018-04-23
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.6.0 - 2017-10-30
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.4.0 - 2017-05-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.2.0 - 2016-11-28
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Manage readonly state on Forecast Line
 
 Version 4.0.0 - 2016-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add Python3 support
 
 Version 3.8.0 - 2015-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.6.0 - 2015-04-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for PyPy
 * Deactivate forecast with passed period
 
 Version 3.4.0 - 2014-10-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.2.0 - 2014-04-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.0.0 - 2013-10-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.8.0 - 2013-04-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.6.0 - 2012-10-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.4.0 - 2012-04-24
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.2.0 - 2011-10-25
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Forecast creates draft moves only on demand
 * Forecast works at warehouse level
 * Allow 'production' as destination
 
 Version 2.0.0 - 2011-04-27
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.8.0 - 2010-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.6.0 - 2010-05-12
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add default search value on forecast
 * Remove egenix-mx-base and replace it by python-dateutil
 
 Version 1.4.0 - 2009-10-19
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.2.0 - 2009-08-10
+--------------------------
 * Initial release
```

### Comparing `trytond_stock_forecast-7.0.0/LICENSE` & `trytond_stock_forecast-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/__init__.py` & `trytond_stock_forecast-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/doc/conf.py` & `trytond_stock_forecast-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_forecast-7.0.0/forecast.py` & `trytond_stock_forecast-7.2.0/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import itertools
 
 from dateutil.relativedelta import relativedelta
 from sql import Null
 from sql.aggregate import Sum
 from sql.conditionals import Coalesce
 
+from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Unique, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.pyson import Bool, Equal, Eval, If, Not, Or
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.transaction import Transaction
@@ -119,14 +120,20 @@
                 where=sql_table.state == 'cancel'))
 
     @staticmethod
     def default_state():
         return 'draft'
 
     @classmethod
+    def default_warehouse(cls):
+        pool = Pool()
+        Location = pool.get('stock.location')
+        return Location.get_default_warehouse()
+
+    @classmethod
     def default_destination(cls):
         Location = Pool().get('stock.location')
         locations = Location.search(cls.destination.domain)
         if len(locations) == 1:
             return locations[0].id
 
     @staticmethod
@@ -520,21 +527,27 @@
                 qty = 0
         return a
 
 
 class ForecastLineMove(ModelSQL):
     'ForecastLine - Move'
     __name__ = 'stock.forecast.line-stock.move'
-    _table = 'forecast_line_stock_move_rel'
     line = fields.Many2One(
         'stock.forecast.line', "Forecast Line",
         ondelete='CASCADE', required=True)
     move = fields.Many2One(
         'stock.move', "Move", ondelete='CASCADE', required=True)
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'forecast_line_stock_move_rel', cls._table)
+        super().__register__(module)
+
 
 class ForecastCompleteAsk(ModelView):
     'Complete Forecast'
     __name__ = 'stock.forecast.complete.ask'
     company = fields.Many2One('company.company', "Company", readonly=True)
     warehouse = fields.Many2One('stock.location', "Warehouse", readonly=True)
     destination = fields.Many2One(
```

### Comparing `trytond_stock_forecast-7.0.0/forecast.xml` & `trytond_stock_forecast-7.2.0/forecast.xml`

 * *Files 20% similar despite different names*

#### Comparing `trytond_stock_forecast-7.0.0/forecast.xml` & `trytond_stock_forecast-7.2.0/forecast.xml`

```diff
@@ -72,50 +72,50 @@
     <record model="ir.ui.view" id="forecast_complete_ask_view_form">
       <field name="model">stock.forecast.complete.ask</field>
       <field name="type">form</field>
       <field name="name">forecast_complete_ask_form</field>
     </record>
     <record model="ir.rule.group" id="rule_group_forecast_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
+      <field name="model">stock.forecast</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_forecast_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_forecast_companies"/>
     </record>
     <record model="ir.model.access" id="access_forecast">
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
+      <field name="model">stock.forecast</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_forecast_group_stock">
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
+      <field name="model">stock.forecast</field>
       <field name="group" ref="group_stock_forecast"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="forecast_cancel_button">
+      <field name="model">stock.forecast</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
     </record>
     <record model="ir.model.button" id="forecast_draft_button">
+      <field name="model">stock.forecast</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
     </record>
     <record model="ir.model.button" id="forecast_confirm_button">
+      <field name="model">stock.forecast</field>
       <field name="name">confirm</field>
       <field name="string">Confirm</field>
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
     </record>
     <record model="ir.model.button" id="forecast_complete_button">
+      <field name="model">stock.forecast</field>
       <field name="name">complete</field>
-      <field name="model" search="[('model', '=', 'stock.forecast')]"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_stock_forecast-7.0.0/locale/bg.po` & `trytond_stock_forecast-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/ca.po` & `trytond_stock_forecast-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/cs.po` & `trytond_stock_forecast-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/de.po` & `trytond_stock_forecast-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/es.po` & `trytond_stock_forecast-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/es_419.po` & `trytond_stock_forecast-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/et.po` & `trytond_stock_forecast-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/fa.po` & `trytond_stock_forecast-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/fi.po` & `trytond_stock_forecast-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/fr.po` & `trytond_stock_forecast-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/hu.po` & `trytond_stock_forecast-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/id.po` & `trytond_stock_forecast-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/it.po` & `trytond_stock_forecast-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/lo.po` & `trytond_stock_forecast-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/lt.po` & `trytond_stock_forecast-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/nl.po` & `trytond_stock_forecast-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/pl.po` & `trytond_stock_forecast-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/pt.po` & `trytond_stock_forecast-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/ro.po` & `trytond_stock_forecast-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/ru.po` & `trytond_stock_forecast-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/sl.po` & `trytond_stock_forecast-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/tr.po` & `trytond_stock_forecast-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/uk.po` & `trytond_stock_forecast-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/locale/zh_CN.po` & `trytond_stock_forecast-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/message.xml` & `trytond_stock_forecast-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/setup.py` & `trytond_stock_forecast-7.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
 def get_require_version(name):
     require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
@@ -53,15 +56,16 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": (
+            'https://docs.tryton.org/projects/modules-stock-forecast'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock forecast',
     package_dir={'trytond.modules.stock_forecast': '.'},
     packages=(
         ['trytond.modules.stock_forecast']
```

### Comparing `trytond_stock_forecast-7.0.0/tests/test_module.py` & `trytond_stock_forecast-7.2.0/tests/test_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 )
             forecast.save()
             with inactive_records():
                 forecasts = Forecast.search([('rec_name', '=', "Warehouse")])
 
             self.assertEqual(
                 forecast.rec_name,
-                "Warehouse → Customer @ [01/01/2023 - 03/31/2023]")
+                "[WH] Warehouse → [CUS] Customer @ [01/01/2023 - 03/31/2023]")
             self.assertEqual(forecasts, [forecast])
 
     @with_transaction()
     def test_distribute(self):
         'Test distribute'
         pool = Pool()
         Line = pool.get('stock.forecast.line')
```

### Comparing `trytond_stock_forecast-7.0.0/tox.ini` & `trytond_stock_forecast-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/trytond_stock_forecast.egg-info/SOURCES.txt` & `trytond_stock_forecast-7.2.0/trytond_stock_forecast.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
@@ -49,15 +48,17 @@
 ./view/forecast_complete_ask_form.xml
 ./view/forecast_form.xml
 ./view/forecast_line_form.xml
 ./view/forecast_line_tree.xml
 ./view/forecast_tree.xml
 ./view/product_list_forecast.xml
 doc/conf.py
+doc/design.rst
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_stock_forecast-7.0.0/view/forecast_complete_ask_form.xml` & `trytond_stock_forecast-7.2.0/view/forecast_complete_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/view/forecast_form.xml` & `trytond_stock_forecast-7.2.0/view/forecast_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-7.0.0/view/forecast_line_form.xml` & `trytond_stock_forecast-7.2.0/view/forecast_line_form.xml`

 * *Files identical despite different names*

