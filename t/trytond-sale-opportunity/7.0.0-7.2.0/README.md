# Comparing `tmp/trytond_sale_opportunity-7.0.0.tar.gz` & `tmp/trytond_sale_opportunity-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_opportunity-7.0.0.tar", last modified: Mon Oct 30 17:38:28 2023, max compression
+gzip compressed data, was "trytond_sale_opportunity-7.2.0.tar", last modified: Mon Apr 29 15:48:21 2024, max compression
```

## Comparing `trytond_sale_opportunity-7.0.0.tar` & `trytond_sale_opportunity-7.2.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.131236 trytond_sale_opportunity-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:23:18.000000 trytond_sale_opportunity-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3203 2023-10-30 17:12:18.000000 trytond_sale_opportunity-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-10-30 17:12:18.000000 trytond_sale_opportunity-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5441 2023-10-30 17:38:28.127903 trytond_sale_opportunity-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2619 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1904 2023-08-13 15:26:13.000000 trytond_sale_opportunity-7.0.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.0.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.127903 trytond_sale_opportunity-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:23:18.000000 trytond_sale_opportunity-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2619 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:18.000000 trytond_sale_opportunity-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.127903 trytond_sale_opportunity-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/icons/tryton-sale-opportunity.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.121236 trytond_sale_opportunity-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    12735 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12072 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11345 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12218 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12124 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11290 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12041 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12359 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11336 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12295 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11711 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10970 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12112 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12442 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11492 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11973 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11700 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12122 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10524 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12652 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12151 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11327 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10295 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11444 2023-10-30 16:47:45.000000 trytond_sale_opportunity-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2938 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20871 2023-10-26 14:42:39.000000 trytond_sale_opportunity-7.0.0/opportunity.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10375 2023-10-27 17:38:49.000000 trytond_sale_opportunity-7.0.0/opportunity.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15493 2023-10-27 17:38:49.000000 trytond_sale_opportunity-7.0.0/opportunity_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25576 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/opportunity_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2236 2023-08-13 15:26:13.000000 trytond_sale_opportunity-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:38:28.131236 trytond_sale_opportunity-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4473 2023-10-27 17:38:49.000000 trytond_sale_opportunity-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.124569 trytond_sale_opportunity-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5463 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/tests/scenario_sale_opportunity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4099 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/tests/scenario_sale_opportunity_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_opportunity-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-10-30 17:12:14.000000 trytond_sale_opportunity-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.127903 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5441 2023-10-30 17:38:27.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4147 2023-10-30 17:38:28.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:38:27.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:38:27.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:38:27.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:38:27.000000 trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:28.124569 trytond_sale_opportunity-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2303 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.0.0/view/opportunity_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_employee_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_employee_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_employee_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-08-21 07:34:17.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-08-21 07:34:17.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2023-08-21 07:34:17.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-08-21 07:34:17.000000 trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      781 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/opportunity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.816990 trytond_sale_opportunity-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4109 2024-04-29 15:25:32.000000 trytond_sale_opportunity-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2024-04-29 15:25:32.000000 trytond_sale_opportunity-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-04-29 15:48:21.816990 trytond_sale_opportunity-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1904 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.810324 trytond_sale_opportunity-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3610 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:26.000000 trytond_sale_opportunity-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.810324 trytond_sale_opportunity-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/icons/tryton-sale-opportunity.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.810324 trytond_sale_opportunity-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    12891 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12228 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11501 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12374 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12280 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11446 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12197 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12515 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11492 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12565 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11867 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12268 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12598 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11648 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12136 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11856 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12278 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12548 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12808 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12307 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11483 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10451 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11600 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2938 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22612 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10404 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15523 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25162 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2236 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:21.816990 trytond_sale_opportunity-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4640 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.813657 trytond_sale_opportunity-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5386 2024-04-22 12:14:36.000000 trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3919 2024-04-22 12:14:36.000000 trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:26.000000 trytond_sale_opportunity-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-29 15:25:28.000000 trytond_sale_opportunity-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.813657 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4161 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.813657 trytond_sale_opportunity-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2303 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      908 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/view/opportunity_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/view/opportunity_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_employee_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_employee_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_employee_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      781 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/party_form.xml
```

### Comparing `trytond_sale_opportunity-7.0.0/CHANGELOG` & `trytond_sale_opportunity-7.2.0/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Add description and note to opportunity line
+* Make product optional on opportunity line
+* Restrict convert button to sale group
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
@@ -15,104 +22,129 @@
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Refactor reporting
 * Use default customer payment term
 * Allow to store currency on opportunity
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use Date field for monthly report
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
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add employee on opportunities for some states
 * Add contact on opportunity
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Use ir.calendar.month in report
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Make description on sale opportunity optional
 
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
 * Compute rates as ratio
 * Make Opportunity employee not required on leads
 
 Version 4.2.0 - 2016-11-28
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Change probability into conversion probability
 * Manage readonly state on Opportunity Line
 
 Version 4.0.0 - 2016-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Rename Opportunity reference into number and add reference
 * Add Python3 support
 * Replace history by revision on client
 
 Version 3.8.0 - 2015-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Fix origin migration from 3.4
 
 Version 3.6.0 - 2015-04-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for PyPy
 * Allow to set manually end date
 * Update of opportunity amount based on linked sales
 * Add a state 'won'
 * Allow to edit the probability after conversion
 
 Version 3.4.0 - 2014-10-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.2.0 - 2014-04-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.0.0 - 2013-10-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Make party optional in leads
 
 Version 2.8.0 - 2013-04-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.6.0 - 2012-10-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.4.0 - 2012-04-24
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove warehouse
 
 Version 2.2.0 - 2011-10-25
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.0.0 - 2011-04-27
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.8.0 - 2010-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 1.6.0 - 2010-09-07
+--------------------------
 * Initial release
```

### Comparing `trytond_sale_opportunity-7.0.0/COPYRIGHT` & `trytond_sale_opportunity-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2010-2011 Open Labs Business Solutions.
-Copyright (C) 2010-2023 Cédric Krier.
-Copyright (C) 2010-2023 B2CK SPRL.
+Copyright (C) 2010-2024 Cédric Krier.
+Copyright (C) 2010-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_opportunity-7.0.0/LICENSE` & `trytond_sale_opportunity-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/__init__.py` & `trytond_sale_opportunity-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/configuration.py` & `trytond_sale_opportunity-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/configuration.xml` & `trytond_sale_opportunity-7.2.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/doc/conf.py` & `trytond_sale_opportunity-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_opportunity-7.0.0/icons/LICENSE` & `trytond_sale_opportunity-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/locale/bg.po` & `trytond_sale_opportunity-7.2.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Служител"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Очаквани приходи"
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/ca.po` & `trytond_sale_opportunity-7.2.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,20 @@
 msgstr "Empleat"
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Empleat"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Import estimat d'ingressos."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr "Percentatge entre 0 i 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/cs.po` & `trytond_sale_opportunity-7.2.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,20 @@
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr ""
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/de.po` & `trytond_sale_opportunity-7.2.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,20 @@
 msgstr "Mitarbeiter"
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Geschätzter Ertrag."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr "Prozentsatz zwischen 0 und 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/es.po` & `trytond_sale_opportunity-7.2.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,20 @@
 msgstr "Empleado"
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Empleado"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Importe estimado de ingresos."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr "Porcentaje entre 0 y 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/es_419.po` & `trytond_sale_opportunity-7.2.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,20 @@
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr ""
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/et.po` & `trytond_sale_opportunity-7.2.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Töötaja"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/fa.po` & `trytond_sale_opportunity-7.2.0/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "کارمند"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "مقدار درآمد تخمینی"
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/fi.po` & `trytond_sale_opportunity-7.2.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,20 @@
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr ""
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/fr.po` & `trytond_sale_opportunity-7.2.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,22 @@
 msgstr "Employé"
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Employé"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+"L'adresse par défaut pour la facture et l'expédition.\n"
+"Laissez vide pour utiliser les valeurs par défaut."
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Revenu estimé."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr "Pourcentage entre 0 et 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/hu.po` & `trytond_sale_opportunity-7.2.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Alkalmazott"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/id.po` & `trytond_sale_opportunity-7.2.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Karyawan"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/it.po` & `trytond_sale_opportunity-7.2.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Dipendente"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Importo reddito stimato"
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/lo.po` & `trytond_sale_opportunity-7.2.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "ພະນັກງານ"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/lt.po` & `trytond_sale_opportunity-7.2.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,20 @@
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr ""
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/nl.po` & `trytond_sale_opportunity-7.2.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,20 @@
 msgstr "Werknemer"
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Werknemer"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Geschat omzetbedrag."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr "Percentage tussen 0 en 100."
@@ -235,15 +241,15 @@
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_conversion_rate"
 msgid "Conversion Rate"
 msgstr "Conversie percentage"
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_conversion_trend"
 msgid "Conversion Trend"
-msgstr "Conversie trend"
+msgstr "Ontwikkeling conversie"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_converted"
 msgid "Converted"
 msgstr "Geconverteerd"
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount"
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/pl.po` & `trytond_sale_opportunity-7.2.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Pracownik"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/pt.po` & `trytond_sale_opportunity-7.2.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Empregado"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Monante estimado de receitas"
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/ro.po` & `trytond_sale_opportunity-7.2.0/locale/uk.po`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 msgctxt "field:sale.configuration.sequence,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
 msgstr ""
 
 msgctxt "field:sale.opportunity,address:"
 msgid "Address"
-msgstr "Adresa"
+msgstr ""
 
 msgctxt "field:sale.opportunity,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:sale.opportunity,comment:"
 msgid "Comment"
-msgstr "Cometariu"
+msgstr ""
 
 msgctxt "field:sale.opportunity,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.opportunity,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
@@ -36,55 +36,55 @@
 
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
 msgstr ""
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:sale.opportunity,lines:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "field:sale.opportunity,lost_reason:"
 msgid "Reason for loss"
 msgstr ""
 
 msgctxt "field:sale.opportunity,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:sale.opportunity,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:sale.opportunity,payment_term:"
 msgid "Payment Term"
-msgstr "Termen de plata"
+msgstr ""
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
-msgstr "Referinţă"
+msgstr ""
 
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
-msgstr "Vânzări"
+msgstr ""
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
@@ -96,51 +96,54 @@
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.conversion.employee,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr ""
 
-#, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr ""
+
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
 
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
@@ -221,23 +224,21 @@
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount_trend"
 msgid "Amount Trend"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_conversion_rate"
 msgid "Conversion Rate"
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_conversion_trend"
@@ -254,44 +255,41 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount_trend"
 msgid "Converted Amount Trend"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_lost"
 msgid "Lost"
-msgstr "Pierdut"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_help"
 msgid "Number of opportunities"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_trend"
 msgid "Number Trend"
-msgstr "Număr"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_rate"
 msgid "Winning Rate"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
 msgid "Won Amount Trend"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:opportunity_cancel_button"
@@ -427,18 +425,17 @@
 msgid "Won"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
-msgstr "Lună"
+msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/ru.po` & `trytond_sale_opportunity-7.2.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Сотрудник"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Оценочная прибыль"
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/sl.po` & `trytond_sale_opportunity-7.2.0/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,20 @@
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr "Zaposlenec"
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Ocenjen znesek prihodkov"
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/tr.po` & `trytond_sale_opportunity-7.2.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,20 @@
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr ""
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/uk.po` & `trytond_sale_opportunity-7.2.0/locale/zh_CN.po`

 * *Files 9% similar despite different names*

```diff
@@ -30,25 +30,27 @@
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
-msgstr ""
+msgstr "Converted"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr ""
+msgstr "描述"
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
@@ -74,29 +76,32 @@
 msgid "Payment Term"
 msgstr ""
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
-msgstr ""
+msgstr "Sales"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
+#, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
-msgstr ""
+msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
@@ -110,17 +115,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "写入日期"
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
@@ -131,92 +137,106 @@
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
 msgstr ""
 
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
+msgstr ""
+
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr ""
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_sale_form"
 msgid "Sales"
-msgstr ""
+msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_opportunity_form"
 msgid "Leads and Opportunities"
-msgstr ""
+msgstr "Leads and Opportunities"
 
 msgctxt "model:ir.action,name:act_opportunity_form2"
 msgid "Sales Leads/Opportunities"
-msgstr ""
+msgstr "Sales Leads/Opportunities"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion"
 msgid "Opportunity Conversions"
-msgstr ""
+msgstr "Opportunities"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion_employee"
 msgid "Opportunity Conversions per Employee"
-msgstr ""
+msgstr "Opportunities per Employee"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion_employee_time_series"
 msgid "Opportunity Conversions per Employee"
-msgstr ""
+msgstr "Opportunities per Employee"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion_time_series"
 msgid "Opportunity Conversions"
-msgstr ""
+msgstr "Opportunities"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Opportunities"
-msgstr ""
+msgstr "Opportunities"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Opportunities"
-msgstr ""
+msgstr "Opportunities"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "全部"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancelled"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_converted"
 msgid "Converted"
-msgstr ""
+msgstr "Converted"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_leads"
 msgid "Leads"
-msgstr ""
+msgstr "Leads"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_lost"
 msgid "Lost"
-msgstr ""
+msgstr "Lost"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_opportunities"
 msgid "Opportunities"
-msgstr ""
+msgstr "Opportunities"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_won"
 msgid "Won"
-msgstr ""
+msgstr "圆"
 
 msgctxt "model:ir.message,text:msg_modify_origin_opportunity"
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
@@ -226,89 +246,96 @@
 msgid "Amount"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount_trend"
 msgid "Amount Trend"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_conversion_rate"
 msgid "Conversion Rate"
-msgstr ""
+msgstr "Converted"
 
+#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_conversion_trend"
 msgid "Conversion Trend"
-msgstr ""
+msgstr "Converted"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_converted"
 msgid "Converted"
-msgstr ""
+msgstr "Converted"
 
+#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount"
 msgid "Converted Amount"
-msgstr ""
+msgstr "Converted"
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount_trend"
 msgid "Converted Amount Trend"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_lost"
 msgid "Lost"
-msgstr ""
+msgstr "Lost"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_help"
 msgid "Number of opportunities"
-msgstr ""
+msgstr "Opportunities"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_trend"
 msgid "Number Trend"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_rate"
 msgid "Winning Rate"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr ""
+msgstr "圆"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
 msgid "Won Amount Trend"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:opportunity_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:opportunity_convert_button"
 msgid "Convert to Sale"
-msgstr ""
+msgstr "Convert to Sale"
 
 msgctxt "model:ir.model.button,string:opportunity_lead_button"
 msgid "Set as Lead"
-msgstr ""
+msgstr "Set as Lead"
 
 msgctxt "model:ir.model.button,string:opportunity_lost_button"
 msgid "Mark as Lost"
-msgstr ""
+msgstr "Mark as Lost"
 
 msgctxt "model:ir.model.button,string:opportunity_opportunity_button"
 msgid "Convert to Opportunity"
-msgstr ""
+msgstr "Convert to Opportunity"
 
 msgctxt "model:ir.rule.group,name:rule_group_opportunity_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_conversion_companies"
 msgid "User in companies"
@@ -327,122 +354,141 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
-msgstr ""
+msgstr "Sale Opportunity"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale_opportunity"
 msgid "Sale Opportunity"
-msgstr ""
+msgstr "Sale Opportunity"
 
 msgctxt "model:ir.ui.menu,name:menu_opportunity_form"
 msgid "Leads and Opportunities"
-msgstr ""
+msgstr "Leads and Opportunities"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_opportunity"
 msgid "Opportunities"
-msgstr ""
+msgstr "Opportunities"
 
 msgctxt "model:res.group,name:group_opportunity"
 msgid "Sale Opportunity"
-msgstr ""
+msgstr "Sale Opportunity"
 
+#, fuzzy
 msgctxt "model:sale.opportunity,name:"
 msgid "Sale Opportunity"
-msgstr ""
+msgstr "Sale Opportunity"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.line,name:"
 msgid "Sale Opportunity Line"
-msgstr ""
+msgstr "Sale Opportunity"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.reporting.context,name:"
 msgid "Sale Opportunity Reporting Context"
-msgstr ""
+msgstr "Opportunities per Employee per Month"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr ""
+msgstr "Opportunities per Employee per Month"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.employee,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr ""
+msgstr "Opportunities per Employee per Month"
 
+#, fuzzy
 msgctxt ""
 "model:sale.opportunity.reporting.conversion.employee.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr ""
+msgstr "Opportunities per Employee per Month"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr ""
+msgstr "Opportunities per Employee per Month"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.reporting.main,name:"
 msgid "Sale Opportunity Reporting"
-msgstr ""
+msgstr "Sale Opportunity"
 
+#, fuzzy
 msgctxt "model:sale.opportunity.reporting.main.time_series,name:"
 msgid "Sale Opportunity Reporting"
-msgstr ""
+msgstr "Sale Opportunity"
 
+#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancelled"
 
+#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Converted"
-msgstr ""
+msgstr "Converted"
 
+#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lead"
-msgstr ""
+msgstr "Leads"
 
+#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lost"
-msgstr ""
+msgstr "Lost"
 
+#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
-msgstr ""
+msgstr "Opportunities"
 
+#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr ""
+msgstr "圆"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
+#, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
+#, fuzzy
 msgctxt "view:sale.opportunity:"
 msgid "%"
-msgstr ""
+msgstr "%"
 
 msgctxt "view:sale.opportunity:"
 msgid "Lead/Opportunity"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_opportunity-7.0.0/locale/zh_CN.po` & `trytond_sale_opportunity-7.2.0/locale/ro.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,488 +1,481 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:sale.configuration,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
-msgstr ""
+msgstr "Secvență de oportunitate"
 
+#, fuzzy
 msgctxt "field:sale.configuration.sequence,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
-msgstr ""
+msgstr "Secvență de oportunitate"
 
 msgctxt "field:sale.opportunity,address:"
 msgid "Address"
-msgstr ""
+msgstr "Adresa"
 
 msgctxt "field:sale.opportunity,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:sale.opportunity,comment:"
 msgid "Comment"
-msgstr ""
+msgstr "Cometariu"
 
 msgctxt "field:sale.opportunity,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:sale.opportunity,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
-msgstr ""
+msgstr "Probabilitate de conversie"
 
-#, fuzzy
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
-msgstr "Converted"
+msgstr "Convertit de"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descriere"
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Angajat"
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data Încheiere"
 
 msgctxt "field:sale.opportunity,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
 msgctxt "field:sale.opportunity,lost_reason:"
 msgid "Reason for loss"
-msgstr ""
+msgstr "Motivul pierderii"
 
 msgctxt "field:sale.opportunity,number:"
 msgid "Number"
-msgstr ""
+msgstr "Număr"
 
 msgctxt "field:sale.opportunity,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:sale.opportunity,payment_term:"
 msgid "Payment Term"
-msgstr ""
+msgstr "Termen de plata"
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
-msgstr ""
+msgstr "Referinţă"
 
-#, fuzzy
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Vânzări"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data de Început"
 
-#, fuzzy
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
-#, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
-msgstr "Opportunities"
+msgstr "Oportunitate"
 
+#, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
-msgstr ""
+msgstr "Starea oportunității"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Unitate"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr "写入日期"
+msgstr "De la Data"
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Perioadă"
 
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Până la Data"
 
 msgctxt "field:sale.opportunity.reporting.conversion.employee,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Angajat"
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
+msgstr "Angajat"
+
+msgctxt "help:sale.opportunity,address:"
+msgid ""
+"The default address for the invoice and shipment.\n"
+"Leave empty to use the default values."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
-msgstr ""
+msgstr "Suma estimată a veniturilor."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
-msgstr ""
+msgstr "Procent între 0 și 100."
 
 msgctxt "model:ir.action,name:act_open_sale_form"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Vânzări"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_opportunity_form"
 msgid "Leads and Opportunities"
-msgstr "Leads and Opportunities"
+msgstr "Piste și Oportunități"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_opportunity_form2"
 msgid "Sales Leads/Opportunities"
-msgstr "Sales Leads/Opportunities"
+msgstr "Piste/Oportunități de vânzări"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion"
 msgid "Opportunity Conversions"
-msgstr "Opportunities"
+msgstr "Conversii de oportunitate"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion_employee"
 msgid "Opportunity Conversions per Employee"
-msgstr "Opportunities per Employee"
+msgstr "Conversii de oportunitate per angajat"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion_employee_time_series"
 msgid "Opportunity Conversions per Employee"
-msgstr "Opportunities per Employee"
+msgstr "Conversii de oportunitate per angajat"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_conversion_time_series"
 msgid "Opportunity Conversions"
-msgstr "Opportunities"
+msgstr "Conversii de oportunitate"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Opportunities"
-msgstr "Opportunities"
+msgstr "Oportunități"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Opportunities"
-msgstr "Opportunities"
+msgstr "Oportunități"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Cancelled"
+msgstr "Anulat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_converted"
 msgid "Converted"
-msgstr "Converted"
+msgstr "Convertit"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_leads"
 msgid "Leads"
-msgstr "Leads"
+msgstr "Piste"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_lost"
 msgid "Lost"
-msgstr "Lost"
+msgstr "Pierdut"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_opportunities"
 msgid "Opportunities"
-msgstr "Opportunities"
+msgstr "Oportunități"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_won"
 msgid "Won"
-msgstr "圆"
+msgstr "Câștigat"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_modify_origin_opportunity"
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
-msgstr ""
+msgstr "Nu puteți modifica originea oportunității vânzării \"%(sale)s\"."
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
 msgstr ""
+"Pentru a șterge oportunitatea \"%(opportunity)s\", aceasta trebuie să fie "
+"anulată."
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount_trend"
 msgid "Amount Trend"
-msgstr ""
+msgstr "Suma"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_conversion_rate"
 msgid "Conversion Rate"
-msgstr "Converted"
+msgstr "Rata de conversie"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_conversion_trend"
 msgid "Conversion Trend"
-msgstr "Converted"
+msgstr "Tendința de conversie"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_converted"
 msgid "Converted"
-msgstr "Converted"
+msgstr "Convertit"
 
-#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount"
 msgid "Converted Amount"
-msgstr "Converted"
+msgstr "Suma convertită"
 
+#, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount_trend"
 msgid "Converted Amount Trend"
-msgstr ""
+msgstr "Tendința sumei convertite"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_lost"
 msgid "Lost"
-msgstr "Lost"
+msgstr "Pierdut"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_help"
 msgid "Number of opportunities"
-msgstr "Opportunities"
+msgstr "Numărul de oportunități"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_trend"
 msgid "Number Trend"
-msgstr ""
+msgstr "Tendința numărului"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_rate"
 msgid "Winning Rate"
-msgstr ""
+msgstr "Rata de câștig"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "圆"
+msgstr "Câștigat"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
-msgstr ""
+msgstr "Suma câștigată"
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
 msgid "Won Amount Trend"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:opportunity_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anulare"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:opportunity_convert_button"
 msgid "Convert to Sale"
-msgstr "Convert to Sale"
+msgstr "Convertire în vânzare"
 
 msgctxt "model:ir.model.button,string:opportunity_lead_button"
 msgid "Set as Lead"
-msgstr "Set as Lead"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:opportunity_lost_button"
 msgid "Mark as Lost"
-msgstr "Mark as Lost"
+msgstr "Marcați ca Pierdut"
 
 msgctxt "model:ir.model.button,string:opportunity_opportunity_button"
 msgid "Convert to Opportunity"
-msgstr "Convert to Opportunity"
+msgstr "Convertiți în oportunitate"
 
 msgctxt "model:ir.rule.group,name:rule_group_opportunity_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_conversion_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_employee_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_employee_time_series_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
-msgstr "Sale Opportunity"
+msgstr "Oportunitate de vânzare"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale_opportunity"
 msgid "Sale Opportunity"
-msgstr "Sale Opportunity"
+msgstr "Oportunitate de vânzare"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_opportunity_form"
 msgid "Leads and Opportunities"
-msgstr "Leads and Opportunities"
+msgstr "Piste și oportunități"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_opportunity"
 msgid "Opportunities"
-msgstr "Opportunities"
+msgstr "Oportunități"
 
 msgctxt "model:res.group,name:group_opportunity"
 msgid "Sale Opportunity"
-msgstr "Sale Opportunity"
+msgstr "Oportunitate de vânzare"
 
-#, fuzzy
 msgctxt "model:sale.opportunity,name:"
 msgid "Sale Opportunity"
-msgstr "Sale Opportunity"
+msgstr "Oportunitate de vânzare"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.line,name:"
 msgid "Sale Opportunity Line"
-msgstr "Sale Opportunity"
+msgstr "Rând de oportunități de vânzare"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.context,name:"
 msgid "Sale Opportunity Reporting Context"
-msgstr "Opportunities per Employee per Month"
+msgstr "Context de raportare a oportunităților de vânzare"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr "Opportunities per Employee per Month"
+msgstr "Conversie de raportare a oportunităților de vânzare"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.employee,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr "Opportunities per Employee per Month"
+msgstr "Conversie de raportare a oportunităților de vânzare per angajat"
 
 #, fuzzy
 msgctxt ""
 "model:sale.opportunity.reporting.conversion.employee.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr "Opportunities per Employee per Month"
+msgstr "Conversie de raportare a oportunităților de vânzare per angajat"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr "Opportunities per Employee per Month"
+msgstr "Conversie de raportare a oportunităților de vânzare"
 
-#, fuzzy
 msgctxt "model:sale.opportunity.reporting.main,name:"
 msgid "Sale Opportunity Reporting"
-msgstr "Sale Opportunity"
+msgstr "Raportarea oportunităților de vânzare"
 
-#, fuzzy
 msgctxt "model:sale.opportunity.reporting.main.time_series,name:"
 msgid "Sale Opportunity Reporting"
-msgstr "Sale Opportunity"
+msgstr "Raportarea oportunităților de vânzare"
 
-#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Cancelled"
-msgstr "Cancelled"
+msgstr "Anulat"
 
-#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Converted"
-msgstr "Converted"
+msgstr "Convertit"
 
-#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lead"
-msgstr "Leads"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lost"
-msgstr "Lost"
+msgstr "Pierdut"
 
-#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
-msgstr "Opportunities"
+msgstr "Oportunitate"
 
-#, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "圆"
+msgstr "Câștigat"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
-msgstr ""
+msgstr "Zi"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
-msgstr ""
+msgstr "Lună"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
-msgstr ""
+msgstr "An"
 
-#, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
-#, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
 
-#, fuzzy
 msgctxt "view:sale.opportunity:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity:"
 msgid "Lead/Opportunity"
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.0.0/message.xml` & `trytond_sale_opportunity-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/opportunity.py` & `trytond_sale_opportunity-7.2.0/opportunity.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from trytond.model import (
     Index, ModelSQL, ModelView, Workflow, fields, sequence_ordered)
 from trytond.model.exceptions import AccessError
 from trytond.modules.company.model import employee_field, set_employee
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, Get, If, In
+from trytond.tools import firstline
 from trytond.transaction import Transaction
 
 
 class SaleOpportunity(
         Workflow, ModelSQL, ModelView,
         AttachmentCopyMixin, NoteCopyMixin):
     'Sale Opportunity'
@@ -54,15 +55,17 @@
             },
         search_context={
             'related_party': Eval('party'),
             },
         depends=['party', 'company'])
     address = fields.Many2One(
         'party.address', "Address", states=_states_stop,
-        domain=[('party', '=', Eval('party'))])
+        domain=[('party', '=', Eval('party'))],
+        help="The default address for the invoice and shipment.\n"
+        "Leave empty to use the default values.")
     company = fields.Many2One(
         'company.company', "Company", required=True,
         states={
             'readonly': _states_stop['readonly'] | Eval('party', True),
             },
         domain=[
             ('id', If(In('company', Eval('context', {})), '=', '!='),
@@ -337,29 +340,33 @@
                 if self.party.customer_currency:
                     self.currency = self.party.customer_currency
 
     def _get_sale_opportunity(self):
         '''
         Return sale for an opportunity
         '''
-        Sale = Pool().get('sale.sale')
-        return Sale(
+        pool = Pool()
+        Sale = pool.get('sale.sale')
+        sale = Sale(
             description=self.description,
             party=self.party,
             contact=self.contact,
-            payment_term=self.payment_term,
             company=self.company,
-            invoice_address=self.address,
-            shipment_address=self.address,
-            currency=self.currency,
             comment=self.comment,
             sale_date=None,
             origin=self,
             warehouse=Sale.default_warehouse(),
             )
+        sale.on_change_party()
+        if self.address:
+            sale.invoice_address = sale.shipment_address = self.address
+        if self.payment_term:
+            sale.payment_term = self.payment_term
+        sale.currency = self.currency
+        return sale
 
     def create_sale(self):
         '''
         Create a sale for the opportunity and return the sale
         '''
         sale = self._get_sale_opportunity()
         sale_lines = []
@@ -388,24 +395,27 @@
     @classmethod
     @ModelView.button
     @Workflow.transition('opportunity')
     def opportunity(cls, opportunities):
         pass
 
     @classmethod
-    @ModelView.button
+    @ModelView.button_action('sale.act_sale_form')
     @Workflow.transition('converted')
     @set_employee('converted_by')
     def convert(cls, opportunities):
         pool = Pool()
         Sale = pool.get('sale.sale')
         sales = [o.create_sale() for o in opportunities if not o.sales]
         Sale.save(sales)
         for sale in sales:
             sale.origin.copy_resources_to(sale)
+        return {
+            'res_id': [s.id for s in sales],
+            }
 
     @property
     def is_forecast(self):
         pool = Pool()
         Date = pool.get('ir.date')
         with Transaction().set_context(company=self.company.id):
             today = Date.today()
@@ -530,35 +540,60 @@
         'sale.opportunity', "Opportunity", ondelete='CASCADE', required=True,
         states={
             'readonly': _states['readonly'] & Bool(Eval('opportunity')),
             })
     opportunity_state = fields.Function(
         fields.Selection('get_opportunity_states', "Opportunity State"),
         'on_change_with_opportunity_state')
-    product = fields.Many2One('product.product', 'Product', required=True,
+    product = fields.Many2One(
+        'product.product', "Product",
         domain=[
             If(Eval('opportunity_state').in_(['lead', 'opportunity'])
                 & ~(Eval('quantity', 0) < 0),
                 ('salable', '=', True),
                 ()),
             ],
         states=_states)
+    product_uom_category = fields.Function(
+        fields.Many2One(
+            'product.uom.category', "Product UoM Category"),
+        'on_change_with_product_uom_category')
     quantity = fields.Float(
         "Quantity", digits='unit', required=True, states=_states)
-    unit = fields.Many2One('product.uom', 'Unit', required=True,
-        states=_states)
+    unit = fields.Many2One(
+        'product.uom', "Unit",
+        domain=[
+            If(Eval('product_uom_category'),
+                ('category', '=', Eval('product_uom_category', -1)),
+                ('category', '=', -1)),
+            ],
+        states={
+            'required': Bool(Eval('product')),
+            'readonly': _states['readonly'],
+            })
+    description = fields.Text("Description", states=_states)
+    summary = fields.Function(fields.Char("Summary"), 'on_change_with_summary')
+    note = fields.Text("Note")
 
     del _states
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('opportunity')
 
     @classmethod
+    def __register__(cls, module):
+        table_h = cls.__table_handler__(module)
+        super().__register__(module)
+        # Migration from 7.0: remove required on product and unit
+        table_h.not_null_action('product', 'remove')
+        table_h.not_null_action('unit', 'remove')
+
+    @classmethod
     def get_opportunity_states(cls):
         pool = Pool()
         Opportunity = pool.get('sale.opportunity')
         return Opportunity.fields_get(['state'])['state']['selection']
 
     @fields.depends('opportunity', '_parent_opportunity.state')
     def on_change_with_opportunity_state(self, name=None):
@@ -570,38 +605,50 @@
         if not self.product:
             return
 
         category = self.product.sale_uom.category
         if not self.unit or self.unit.category != category:
             self.unit = self.product.sale_uom
 
+    @fields.depends('product')
+    def on_change_with_product_uom_category(self, name=None):
+        return self.product.default_uom_category if self.product else None
+
+    @fields.depends('description')
+    def on_change_with_summary(self, name=None):
+        return firstline(self.description or '')
+
     def get_sale_line(self, sale):
         '''
         Return sale line for opportunity line
         '''
         SaleLine = Pool().get('sale.line')
         sale_line = SaleLine(
             type='line',
             product=self.product,
             sale=sale,
-            description=None,
+            description=self.description,
             )
         sale_line.on_change_product()
         self._set_sale_line_quantity(sale_line)
         sale_line.on_change_quantity()
         return sale_line
 
     def _set_sale_line_quantity(self, sale_line):
         sale_line.quantity = self.quantity
         sale_line.unit = self.unit
 
     def get_rec_name(self, name):
         pool = Pool()
         Lang = pool.get('ir.lang')
         lang = Lang.get()
-        return (lang.format_number_symbol(
-                self.quantity or 0, self.unit, digits=self.unit.digits)
-            + ' %s @ %s' % (self.product.rec_name, self.opportunity.rec_name))
+        if self.product:
+            return (lang.format_number_symbol(
+                    self.quantity or 0, self.unit, digits=self.unit.digits)
+                + ' %s @ %s' % (
+                    self.product.rec_name, self.opportunity.rec_name))
+        else:
+            return self.opportunity.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('product.rec_name',) + tuple(clause[1:])]
```

### Comparing `trytond_sale_opportunity-7.0.0/opportunity.xml` & `trytond_sale_opportunity-7.2.0/opportunity.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_sale_opportunity-7.0.0/opportunity.xml` & `trytond_sale_opportunity-7.2.0/opportunity.xml`

```diff
@@ -99,64 +99,68 @@
     </record>
     <menuitem parent="sale.menu_sale" action="act_opportunity_form" sequence="5" id="menu_opportunity_form"/>
     <record model="ir.ui.menu-res.group" id="menu_sale_opportunity_group_opportunity">
       <field name="menu" ref="sale.menu_sale"/>
       <field name="group" ref="group_opportunity"/>
     </record>
     <record model="ir.model.access" id="access_opportunity">
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
+      <field name="model">sale.opportunity</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_opportunity_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
+      <field name="model">sale.opportunity</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_opportunity_oppotunity">
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
+      <field name="model">sale.opportunity</field>
       <field name="group" ref="group_opportunity"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="opportunity_lead_button">
+      <field name="model">sale.opportunity</field>
       <field name="name">lead</field>
       <field name="string">Set as Lead</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
     </record>
     <record model="ir.model.button" id="opportunity_opportunity_button">
+      <field name="model">sale.opportunity</field>
       <field name="name">opportunity</field>
       <field name="string">Convert to Opportunity</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
     </record>
     <record model="ir.model.button" id="opportunity_convert_button">
+      <field name="model">sale.opportunity</field>
       <field name="name">convert</field>
       <field name="string">Convert to Sale</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
+    </record>
+    <record model="ir.model.button-res.group" id="opportunity_convert_button_group_sale">
+      <field name="button" ref="opportunity_convert_button"/>
+      <field name="group" ref="sale.group_sale"/>
     </record>
     <record model="ir.model.button" id="opportunity_lost_button">
+      <field name="model">sale.opportunity</field>
       <field name="name">lost</field>
       <field name="string">Mark as Lost</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
     </record>
     <record model="ir.model.button" id="opportunity_cancel_button">
+      <field name="model">sale.opportunity</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
     </record>
     <record model="ir.rule.group" id="rule_group_opportunity_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity')]"/>
+      <field name="model">sale.opportunity</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_opportunity_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_opportunity_companies"/>
     </record>
     <record model="ir.action.act_window" id="act_open_sale_form">
```

### Comparing `trytond_sale_opportunity-7.0.0/opportunity_reporting.py` & `trytond_sale_opportunity-7.2.0/opportunity_reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,16 @@
     @classmethod
     def _group_by(cls, tables, withs):
         opportunity = tables['opportunity']
         return super()._group_by(tables, withs) + [
             opportunity.employee]
 
     def get_rec_name(self, name):
-        return self.employee.rec_name
+        if self.employee:
+            return self.employee.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('employee.rec_name', *clause[1:])]
 
 
 class ConversionEmployee(EmployeeMixin, AbstractConversion, ModelView):
```

### Comparing `trytond_sale_opportunity-7.0.0/opportunity_reporting.xml` & `trytond_sale_opportunity-7.2.0/opportunity_reporting.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale_opportunity-7.0.0/opportunity_reporting.xml` & `trytond_sale_opportunity-7.2.0/opportunity_reporting.xml`

```diff
@@ -38,30 +38,30 @@
     <record model="ir.action.keyword" id="act_reporting_main_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model" ref="menu_reporting_opportunity"/>
       <field name="action" ref="act_reporting_main"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_main_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.main')]"/>
+      <field name="model">sale.opportunity.reporting.main</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_main_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_main_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.main')]"/>
+      <field name="model">sale.opportunity.reporting.main</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.main')]"/>
+      <field name="model">sale.opportunity.reporting.main</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_main_time_series_view_list">
@@ -105,30 +105,30 @@
     <record model="ir.action.keyword" id="act_reporting_main_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.opportunity.reporting.main,-1</field>
       <field name="action" ref="act_reporting_main_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_main_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.main.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.main.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_main_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_main_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_time_series">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.main.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.main.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.main.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.main.time_series</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Conversion -->
@@ -160,30 +160,30 @@
     <record model="ir.action.keyword" id="act_reporting_conversion_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model" ref="menu_reporting_opportunity"/>
       <field name="action" ref="act_reporting_conversion"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_conversion_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion')]"/>
+      <field name="model">sale.opportunity.reporting.conversion</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_conversion_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_conversion_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion')]"/>
+      <field name="model">sale.opportunity.reporting.conversion</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion')]"/>
+      <field name="model">sale.opportunity.reporting.conversion</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_conversion_time_series_view_list">
@@ -227,30 +227,30 @@
     <record model="ir.action.keyword" id="act_reporting_conversion_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.opportunity.reporting.conversion,-1</field>
       <field name="action" ref="act_reporting_conversion_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_conversion_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_conversion_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_conversion_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_time_series">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.time_series</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Conversion Employee -->
@@ -300,30 +300,30 @@
     <record model="ir.action.keyword" id="act_reporting_conversion_employee_keyword2">
       <field name="keyword">tree_open</field>
       <field name="model">sale.opportunity.reporting.conversion,-1</field>
       <field name="action" ref="act_reporting_conversion_employee"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_conversion_employee_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.employee')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.employee</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_conversion_employee_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_conversion_employee_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_employee">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.employee')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.employee</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_employee_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.employee')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.employee</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_conversion_employee_time_series_view_list">
@@ -366,30 +366,30 @@
     <record model="ir.action.keyword" id="act_reporting_conversion_employee_time_series_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.opportunity.reporting.conversion.employee,-1</field>
       <field name="action" ref="act_reporting_conversion_employee_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_conversion_employee_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.employee.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.employee.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_conversion_employee_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_conversion_employee_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_employee_time_series">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.employee.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.employee.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_conversion_employee_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.opportunity.reporting.conversion.employee.time_series')]"/>
+      <field name="model">sale.opportunity.reporting.conversion.employee.time_series</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_sale_opportunity-7.0.0/party.py` & `trytond_sale_opportunity-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/party.xml` & `trytond_sale_opportunity-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/sale.py` & `trytond_sale_opportunity-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/setup.py` & `trytond_sale_opportunity-7.2.0/setup.py`

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
@@ -55,15 +58,17 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": (
+            'https://docs.tryton.org/'
+            'modules-sale-opportunity'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale opportunity',
     package_dir={'trytond.modules.sale_opportunity': '.'},
     packages=(
         ['trytond.modules.sale_opportunity']
```

### Comparing `trytond_sale_opportunity-7.0.0/tests/scenario_sale_opportunity.rst` & `trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 =========================
 Sale Opportunity Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     create_payment_term
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
 Activate modules::
 
     >>> config = activate_modules('sale_opportunity')
 
+    >>> Sale = Model.get('sale.sale')
+
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create chart of accounts::
 
@@ -121,27 +121,24 @@
     >>> line = opportunity.lines.new()
     >>> line.product = product
     >>> line.quantity = 10
     >>> opportunity.save()
 
 Convert to sale::
 
-    >>> opportunity.click('convert')
+    >>> set_user(sale_user)
+    >>> sale, = opportunity.click('convert')
     >>> opportunity.state
     'converted'
+    >>> assertEqual(sale.origin, opportunity)
 
 Find the sale::
 
-    >>> set_user(sale_user)
-    >>> Sale = Model.get('sale.sale')
-    >>> sale, = Sale.find(
-    ...     [('origin', '=', 'sale.opportunity,%s' % opportunity.id)])
     >>> line, = sale.lines
-    >>> line.product == product
-    True
+    >>> assertEqual(line.product, product)
     >>> line.quantity
     10.0
 
 Quote different quantity::
 
     >>> line.quantity = 9
     >>> sale.click('quote')
```

### Comparing `trytond_sale_opportunity-7.0.0/tests/scenario_sale_opportunity_reporting.rst` & `trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity_reporting.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 ===================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('sale_opportunity')
 
@@ -61,22 +58,21 @@
     >>> opportunity.click('opportunity')
 
     >>> opportunity = Opportunity(party=customer2)
     >>> opportunity.amount = Decimal('500.00')
     >>> opportunity.employee = employee2
     >>> opportunity.end_date = today
     >>> opportunity.click('opportunity')
-    >>> opportunity.click('convert')
+    >>> sale, = opportunity.click('convert')
 
     >>> opportunity = Opportunity(party=customer1)
     >>> opportunity.amount = Decimal('700.00')
     >>> opportunity.employee = employee1
     >>> opportunity.click('opportunity')
-    >>> opportunity.click('convert')
-    >>> sale, = opportunity.sales
+    >>> sale, = opportunity.click('convert')
     >>> line = sale.lines.new()
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('800.00')
     >>> sale.invoice_address, = sale.party.addresses
     >>> sale.click('quote')
     >>> sale.click('confirm')
 
@@ -94,35 +90,34 @@
     ...     to_date=today,
     ...     period='month')
     >>> with config.set_context(context=context):
     ...     reports = Main.find([])
     >>> report, = reports
     >>> report.number
     5
-    >>> report.amount == Decimal('4500.00')
-    True
+    >>> report.amount
+    Decimal('4500.00')
     >>> report.converted
     2
     >>> report.conversion_rate
     0.4
-    >>> report.converted_amount == Decimal('1300.00')
-    True
+    >>> report.converted_amount
+    Decimal('1300.00')
 
     >>> report, = report.time_series
     >>> report.number
     5
-    >>> report.amount == Decimal('4500.00')
-    True
+    >>> report.amount
+    Decimal('4500.00')
     >>> report.converted
     2
     >>> report.conversion_rate
     0.4
-    >>> report.converted_amount == Decimal('1300.00')
-    True
-
+    >>> report.converted_amount
+    Decimal('1300.00')
 
 Check conversion reporting::
 
     >>> Conversion = Model.get('sale.opportunity.reporting.conversion')
     >>> with config.set_context(context=context):
     ...     reports = Conversion.find([])
     >>> report, = reports
@@ -130,16 +125,16 @@
     3
     >>> report.converted
     2
     >>> report.won
     1
     >>> report.winning_rate
     0.3333
-    >>> report.won_amount == Decimal('800.00')
-    True
+    >>> report.won_amount
+    Decimal('800.00')
     >>> report.lost
     1
     >>> len(report.time_series)
     1
 
     >>> ConversionEmployee = Model.get(
     ...     'sale.opportunity.reporting.conversion.employee')
```

### Comparing `trytond_sale_opportunity-7.0.0/tox.ini` & `trytond_sale_opportunity-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/trytond_sale_opportunity.egg-info/SOURCES.txt` & `trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/SOURCES.txt`

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
@@ -85,15 +84,17 @@
 ./view/opportunity_reporting_main_list.xml
 ./view/opportunity_reporting_main_time_series_graph_amount.xml
 ./view/opportunity_reporting_main_time_series_graph_number.xml
 ./view/opportunity_reporting_main_time_series_list.xml
 ./view/opportunity_tree.xml
 ./view/party_form.xml
 doc/conf.py
+doc/design.rst
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 icons/LICENSE
 icons/tryton-sale-opportunity.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

### Comparing `trytond_sale_opportunity-7.0.0/view/opportunity_form.xml` & `trytond_sale_opportunity-7.2.0/view/opportunity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/view/opportunity_reporting_conversion_list.xml` & `trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/view/opportunity_reporting_main_list.xml` & `trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.0.0/view/opportunity_tree.xml` & `trytond_sale_opportunity-7.2.0/view/opportunity_tree.xml`

 * *Files identical despite different names*

