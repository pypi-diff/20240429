# Comparing `tmp/trytond_commission-7.0.0.tar.gz` & `tmp/trytond_commission-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_commission-7.0.0.tar", last modified: Mon Oct 30 17:28:31 2023, max compression
+gzip compressed data, was "trytond_commission-7.2.0.tar", last modified: Mon Apr 29 15:39:08 2024, max compression
```

## Comparing `trytond_commission-7.0.0.tar` & `trytond_commission-7.2.0.tar`

### file list

```diff
@@ -1,115 +1,114 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.351723 trytond_commission-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-22 17:23:01.000000 trytond_commission-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2599 2023-10-30 17:05:33.000000 trytond_commission-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:05:33.000000 trytond_commission-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3218 2023-10-30 17:28:31.351723 trytond_commission-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22626 2023-08-21 07:34:17.000000 trytond_commission-7.0.0/commission.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14458 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/commission.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7646 2023-10-27 17:38:49.000000 trytond_commission-7.0.0/commission_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8742 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/commission_reporting.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.348389 trytond_commission-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-22 17:23:01.000000 trytond_commission-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:01.000000 trytond_commission-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      872 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.351723 trytond_commission-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/icons/tryton-commission.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     9082 2023-08-13 15:26:13.000000 trytond_commission-7.0.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3713 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/invoice.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.345056 trytond_commission-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16314 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17192 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15228 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17627 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17297 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14178 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15826 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17040 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15215 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17532 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15741 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14712 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16162 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16499 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15442 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17601 2023-10-30 16:47:45.000000 trytond_commission-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15612 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14377 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16267 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16131 2023-10-30 16:47:45.000000 trytond_commission-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15215 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14133 2023-10-28 12:11:21.000000 trytond_commission-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15460 2023-10-30 16:47:45.000000 trytond_commission-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3639 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:28:31.351723 trytond_commission-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4746 2023-10-27 17:38:49.000000 trytond_commission-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2132 2023-10-07 17:14:58.000000 trytond_commission-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1154 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/stock_reporting_margin.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.345056 trytond_commission-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2741 2023-06-10 11:39:56.000000 trytond_commission-7.0.0/tests/scenario_agent_selection.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7332 2023-08-13 15:26:13.000000 trytond_commission-7.0.0/tests/scenario_commission.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3896 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/tests/scenario_commission_credit_posted_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5819 2023-06-10 11:39:56.000000 trytond_commission-7.0.0/tests/scenario_commission_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3670 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_commission-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:05:30.000000 trytond_commission-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.351723 trytond_commission-7.0.0/trytond_commission.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3218 2023-10-30 17:28:30.000000 trytond_commission-7.0.0/trytond_commission.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4163 2023-10-30 17:28:31.000000 trytond_commission-7.0.0/trytond_commission.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:28:30.000000 trytond_commission-7.0.0/trytond_commission.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-10-30 17:28:30.000000 trytond_commission-7.0.0/trytond_commission.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_commission-7.0.0/trytond_commission.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-30 17:28:30.000000 trytond_commission-7.0.0/trytond_commission.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:28:30.000000 trytond_commission-7.0.0/trytond_commission.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:31.348389 trytond_commission-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/account_invoice_credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/agent_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/agent_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/agent_selection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/agent_selection_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/agent_selection_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/commission_create_invoice_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/commission_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/commission_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/plan_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/plan_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/plan_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/plan_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/plan_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_agent_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_agent_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_agent_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_agent_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_agent_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_agent_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_commission-7.0.0/view/stock_reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_commission-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-29 15:18:45.000000 trytond_commission-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:18:45.000000 trytond_commission-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22626 2024-01-27 09:58:52.000000 trytond_commission-7.2.0/commission.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14258 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/commission.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8084 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/commission_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8572 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/commission_reporting.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.768121 trytond_commission-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:07.000000 trytond_commission-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      872 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.768121 trytond_commission-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/icons/tryton-commission.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     9082 2024-01-27 09:58:52.000000 trytond_commission-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3713 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/invoice.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.771454 trytond_commission-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16314 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17192 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15228 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17627 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17297 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14178 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15826 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17040 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15215 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17532 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15741 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14712 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16162 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16499 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15442 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17615 2024-04-29 13:17:17.000000 trytond_commission-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15612 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16639 2024-04-29 13:17:17.000000 trytond_commission-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16267 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16131 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15215 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14133 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15460 2024-04-27 16:43:22.000000 trytond_commission-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      682 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3639 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4746 2024-03-17 11:01:36.000000 trytond_commission-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2132 2024-02-04 18:51:26.000000 trytond_commission-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1154 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/stock_reporting_margin.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.771454 trytond_commission-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2688 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/tests/scenario_agent_selection.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7319 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/tests/scenario_commission.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3882 2024-04-22 12:14:36.000000 trytond_commission-7.2.0/tests/scenario_commission_credit_posted_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5752 2024-04-27 16:30:39.000000 trytond_commission-7.2.0/tests/scenario_commission_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3670 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:07.000000 trytond_commission-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-29 15:18:41.000000 trytond_commission-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/trytond_commission.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4145 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_commission-7.2.0/trytond_commission.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:08.000000 trytond_commission-7.2.0/trytond_commission.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:08.774788 trytond_commission-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/account_invoice_credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/agent_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_selection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_selection_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/agent_selection_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/commission_create_invoice_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/commission_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/commission_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/plan_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/plan_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/plan_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/plan_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/plan_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_agent_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_commission-7.2.0/view/stock_reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_commission-7.2.0/view/template_form.xml
```

### Comparing `trytond_commission-7.0.0/CHANGELOG` & `trytond_commission-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_commission-7.0.0/LICENSE` & `trytond_commission-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/PKG-INFO` & `trytond_commission-7.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_commission
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for commission
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
@@ -51,28 +51,28 @@
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
 Requires-Dist: python-sql
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: sparklines
 Requires-Dist: pygal; extra == "sparklines"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 #################
 Commission Module
 #################
 
 The *Commission Module* allows you to manage commission for sale's agent.
 A commission move is created when posting the invoice, following the agent's
```

### Comparing `trytond_commission-7.0.0/__init__.py` & `trytond_commission-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/commission.py` & `trytond_commission-7.2.0/commission.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/commission.xml` & `trytond_commission-7.2.0/commission.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_commission-7.0.0/commission.xml` & `trytond_commission-7.2.0/commission.xml`

```diff
@@ -55,30 +55,30 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="agent_view_form"/>
       <field name="act_window" ref="act_agent_form"/>
     </record>
     <menuitem parent="menu_commission" action="act_agent_form" sequence="20" id="menu_agent_form"/>
     <record model="ir.rule.group" id="rule_group_agent_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'commission.agent')]"/>
+      <field name="model">commission.agent</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_agent_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_agent_companies"/>
     </record>
     <record model="ir.model.access" id="access_agent">
-      <field name="model" search="[('model', '=', 'commission.agent')]"/>
+      <field name="model">commission.agent</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_agent_commission_admin">
-      <field name="model" search="[('model', '=', 'commission.agent')]"/>
+      <field name="model">commission.agent</field>
       <field name="group" ref="group_commission_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="agent_selection_view_form">
@@ -139,22 +139,22 @@
     <record model="ir.action.act_window.view" id="act_plan_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="plan_view_form"/>
       <field name="act_window" ref="act_plan_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_plan_form" sequence="10" id="menu_plan_form"/>
     <record model="ir.model.access" id="access_plan">
-      <field name="model" search="[('model', '=', 'commission.plan')]"/>
+      <field name="model">commission.plan</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_plan_commission_admin">
-      <field name="model" search="[('model', '=', 'commission.plan')]"/>
+      <field name="model">commission.plan</field>
       <field name="group" ref="group_commission_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="plan_line_view_form">
@@ -217,32 +217,32 @@
     </record>
     <record model="ir.action.keyword" id="act_commission_form2_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">commission.agent,-1</field>
       <field name="action" ref="act_commission_form2"/>
     </record>
     <record model="ir.model.access" id="access_commission">
-      <field name="model" search="[('model', '=', 'commission')]"/>
+      <field name="model">commission</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_commission_commission">
-      <field name="model" search="[('model', '=', 'commission')]"/>
+      <field name="model">commission</field>
       <field name="group" ref="group_commission"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="commission_invoice_button">
+      <field name="model">commission</field>
       <field name="name">invoice</field>
       <field name="string">Invoice</field>
-      <field name="model" search="[('model', '=', 'commission')]"/>
     </record>
     <record model="ir.action.wizard" id="act_commission_create_invoice">
       <field name="name">Create Commission Invoices</field>
       <field name="wiz_name">commission.create_invoice</field>
     </record>
     <record model="ir.action-res.group" id="act_commission_create_invoice-group_commission">
       <field name="action" ref="act_commission_create_invoice"/>
```

### Comparing `trytond_commission-7.0.0/commission_reporting.py` & `trytond_commission-7.2.0/commission_reporting.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 try:
     import pygal
 except ImportError:
     pygal = None
 from sql import Literal, Null
 from sql.aggregate import Count, Min, Sum
 from sql.conditionals import Coalesce
-from sql.functions import CurrentTimestamp, DateTrunc
+from sql.functions import CurrentTimestamp, DateTrunc, Round
 
 from trytond.model import ModelSQL, ModelView, fields
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits
 from trytond.pool import Pool
 from trytond.pyson import Eval, If
 from trytond.tools import pairwise_longest
@@ -33,16 +33,15 @@
     base_amount_trend = fields.Function(
         fields.Char("Base Amount Trend"), 'get_trend')
     amount = Monetary("Amount", currency='currency', digits=price_digits)
 
     time_series = fields.One2Many(
         'commission.reporting.agent.time_series', 'agent', "Time Series")
 
-    currency = fields.Function(fields.Many2One(
-            'currency.currency', "Currency"), 'get_currency')
+    currency = fields.Many2One('currency.currency', "Currency")
 
     @classmethod
     def table_query(cls):
         from_item, tables, withs = cls._joins()
         return from_item.select(
             *cls._columns(tables, withs),
             where=cls._where(tables, withs),
@@ -50,48 +49,58 @@
             with_=withs.values())
 
     @classmethod
     def _joins(cls):
         pool = Pool()
         Commission = pool.get('commission')
         Agent = pool.get('commission.agent')
+        Currency = pool.get('currency.currency')
 
         tables = {}
         tables['commission'] = commission = Commission.__table__()
         tables['commission.agent'] = agent = Agent.__table__()
+        tables['commission.agent.currency'] = currency = Currency.__table__()
         withs = {}
 
         from_item = (commission
-            .join(agent, condition=commission.agent == agent.id))
+            .join(agent, condition=commission.agent == agent.id)
+            .join(currency, condition=agent.currency == currency.id))
         return from_item, tables, withs
 
     @classmethod
     def _columns(cls, tables, withs):
         commission = tables['commission']
+        agent = tables['commission.agent']
+        currency = tables['commission.agent.currency']
         return [
             cls._column_id(tables, withs).as_('id'),
             Literal(0).as_('create_uid'),
             CurrentTimestamp().as_('create_date'),
             cls.write_uid.sql_cast(Literal(Null)).as_('write_uid'),
             cls.write_date.sql_cast(Literal(Null)).as_('write_date'),
             commission.agent.as_('agent'),
+            agent.currency.as_('currency'),
             Count(commission.id, distinct=True).as_('number'),
-            Sum(Coalesce(commission.base_amount, 0)).as_('base_amount'),
-            Sum(commission.amount).as_('amount'),
+            Round(
+                Sum(Coalesce(commission.base_amount, 0)),
+                currency.digits).as_('base_amount'),
+            Round(Sum(commission.amount), currency.digits).as_('amount'),
             ]
 
     @classmethod
     def _column_id(cls, tables, withs):
         commission = tables['commission']
         return commission.agent
 
     @classmethod
     def _group_by(cls, tables, withs):
         commission = tables['commission']
-        return [commission.agent]
+        agent = tables['commission.agent']
+        currency = tables['commission.agent.currency']
+        return [commission.agent, agent.currency, currency.digits]
 
     @classmethod
     def _where(cls, tables, withs):
         context = Transaction().context
         commission = tables['commission']
         agent = tables['commission.agent']
         where = agent.type_ == cls._get_agent_type(context.get('type', 'out'))
@@ -137,17 +146,14 @@
         if pygal:
             chart = pygal.Line()
             chart.add('', [
                     getattr(ts, name, 0) or 0
                     for ts in self.time_series_all])
             return chart.render_sparktext()
 
-    def get_currency(self, name):
-        return self.agent.currency.id
-
     def get_rec_name(self, name):
         return self.agent.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('agent.rec_name', *clause[1:])]
```

### Comparing `trytond_commission-7.0.0/commission_reporting.xml` & `trytond_commission-7.2.0/commission_reporting.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_commission-7.0.0/commission_reporting.xml` & `trytond_commission-7.2.0/commission_reporting.xml`

```diff
@@ -48,30 +48,30 @@
     <record model="ir.action.keyword" id="act_reporting_agent_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model" ref="menu_reporting_commission"/>
       <field name="action" ref="act_reporting_agent"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_agent_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'commission.reporting.agent')]"/>
+      <field name="model">commission.reporting.agent</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_agent_companies">
       <field name="domain" eval="[('agent.company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_agent_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_agent">
-      <field name="model" search="[('model', '=', 'commission.reporting.agent')]"/>
+      <field name="model">commission.reporting.agent</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_agent_commission">
-      <field name="model" search="[('model', '=', 'commission.reporting.agent')]"/>
+      <field name="model">commission.reporting.agent</field>
       <field name="group" ref="group_commission"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_agent_time_series_view_list">
@@ -114,30 +114,30 @@
     <record model="ir.action.keyword" id="act_reporting_agent_time_series_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">commission.reporting.agent,-1</field>
       <field name="action" ref="act_reporting_agent_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_agent_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'commission.reporting.agent.time_series')]"/>
+      <field name="model">commission.reporting.agent.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_agent_time_series_companies">
       <field name="domain" eval="[('agent.company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_agent_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_agent_time_series">
-      <field name="model" search="[('model', '=', 'commission.reporting.agent.time_series')]"/>
+      <field name="model">commission.reporting.agent.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_agent_time_series_commission">
-      <field name="model" search="[('model', '=', 'commission.reporting.agent.time_series')]"/>
+      <field name="model">commission.reporting.agent.time_series</field>
       <field name="group" ref="group_commission"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_commission-7.0.0/doc/conf.py` & `trytond_commission-7.2.0/doc/conf.py`

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

### Comparing `trytond_commission-7.0.0/doc/design.rst` & `trytond_commission-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/doc/usage.rst` & `trytond_commission-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/icons/LICENSE` & `trytond_commission-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/icons/tryton-commission.svg` & `trytond_commission-7.2.0/icons/tryton-commission.svg`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/invoice.py` & `trytond_commission-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/invoice.xml` & `trytond_commission-7.2.0/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/ir.py` & `trytond_commission-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/bg.po` & `trytond_commission-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/ca.po` & `trytond_commission-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/cs.po` & `trytond_commission-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/de.po` & `trytond_commission-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/es.po` & `trytond_commission-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/es_419.po` & `trytond_commission-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/et.po` & `trytond_commission-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/fa.po` & `trytond_commission-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/fi.po` & `trytond_commission-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/fr.po` & `trytond_commission-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/hu.po` & `trytond_commission-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/id.po` & `trytond_commission-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/it.po` & `trytond_commission-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/lo.po` & `trytond_commission-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/lt.po` & `trytond_commission-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/nl.po` & `trytond_commission-7.2.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
 msgctxt "field:commission.reporting.agent,base_amount:"
 msgid "Base Amount"
 msgstr "Basis bedrag"
 
 msgctxt "field:commission.reporting.agent,base_amount_trend:"
 msgid "Base Amount Trend"
-msgstr "Trend basisbedrag"
+msgstr "Ontwikkeling basisbedrag"
 
 msgctxt "field:commission.reporting.agent,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:commission.reporting.agent,number:"
 msgid "Number"
@@ -200,15 +200,15 @@
 
 msgctxt "field:commission.reporting.agent.time_series,base_amount:"
 msgid "Base Amount"
 msgstr "Basis bedrag"
 
 msgctxt "field:commission.reporting.agent.time_series,base_amount_trend:"
 msgid "Base Amount Trend"
-msgstr "Trend basisbedrag"
+msgstr "Ontwikkeling basisbedrag"
 
 msgctxt "field:commission.reporting.agent.time_series,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:commission.reporting.agent.time_series,date:"
 msgid "Date"
```

### Comparing `trytond_commission-7.0.0/locale/pl.po` & `trytond_commission-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/pt.po` & `trytond_commission-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/ro.po` & `trytond_commission-7.2.0/locale/uk.po`

 * *Files 9% similar despite different names*

```diff
@@ -24,60 +24,59 @@
 
 msgctxt "field:commission,agent:"
 msgid "Agent"
 msgstr ""
 
 msgctxt "field:commission,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:commission,base_amount:"
 msgid "Base Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:commission,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:commission,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:commission,invoice_line:"
 msgid "Invoice Line"
 msgstr ""
 
 msgctxt "field:commission,invoice_state:"
 msgid "Invoice State"
-msgstr "Stare Factura"
+msgstr ""
 
 msgctxt "field:commission,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:commission,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:commission,type_:"
 msgid "Type"
-msgstr "Tip"
+msgstr ""
 
 msgctxt "field:commission.agent,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:commission.agent,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:commission.agent,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:commission.agent,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
 msgctxt "field:commission.agent,plan:"
 msgid "Plan"
@@ -91,30 +90,29 @@
 msgid "Type"
 msgstr ""
 
 msgctxt "field:commission.agent.selection,agent:"
 msgid "Agent"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.agent.selection,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:commission.agent.selection,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:commission.agent.selection,end_date:"
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:commission.agent.selection,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:commission.agent.selection,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:commission.create_invoice.ask,agents:"
 msgid "Agents"
@@ -146,114 +144,103 @@
 
 msgctxt "field:commission.plan,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:commission.plan.line,category:"
 msgid "Category"
-msgstr "Categorie"
+msgstr ""
 
 msgctxt "field:commission.plan.line,formula:"
 msgid "Formula"
 msgstr ""
 
 msgctxt "field:commission.plan.line,plan:"
 msgid "Plan"
 msgstr ""
 
 msgctxt "field:commission.plan.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:commission.reporting.agent,agent:"
 msgid "Agent"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent,base_amount:"
 msgid "Base Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:commission.reporting.agent,base_amount_trend:"
 msgid "Base Amount Trend"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:commission.reporting.agent,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent,time_series:"
 msgid "Time Series"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent.time_series,agent:"
 msgid "Agent"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,base_amount:"
 msgid "Base Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:commission.reporting.agent.time_series,base_amount_trend:"
 msgid "Base Amount Trend"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:commission.reporting.agent.time_series,number:"
 msgid "Number"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Data"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,invoiced:"
 msgid "Invoiced"
-msgstr "Stare Factura"
+msgstr ""
 
 msgctxt "field:commission.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,to_date:"
 msgid "To Date"
-msgstr "Data"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,type:"
 msgid "Type"
-msgstr "Tip"
+msgstr ""
 
 msgctxt "field:party.party,agents:"
 msgid "Agents"
 msgstr ""
 
 msgctxt "field:product.product,principals:"
 msgid "Commission Principals"
@@ -265,15 +252,15 @@
 
 msgctxt "field:product.template-commission.agent,agent:"
 msgid "Agent"
 msgstr ""
 
 msgctxt "field:product.template-commission.agent,template:"
 msgid "Template"
-msgstr "Șablon"
+msgstr ""
 
 msgctxt "field:sale.line,principal:"
 msgid "Commission Principal"
 msgstr ""
 
 msgctxt "field:sale.sale,agent:"
 msgid "Commission Agent"
@@ -533,23 +520,23 @@
 
 msgctxt "model:ir.ui.menu,name:menu_commission_form"
 msgid "Commissions"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Налаштування"
 
 msgctxt "model:ir.ui.menu,name:menu_plan_form"
 msgid "Plans"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr ""
+msgstr "Звітність"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting_commission"
 msgid "Commissions"
 msgstr ""
 
 msgctxt "model:product.template-commission.agent,name:"
 msgid "Product Template - Commission Agent"
```

### Comparing `trytond_commission-7.0.0/locale/ru.po` & `trytond_commission-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/sl.po` & `trytond_commission-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/tr.po` & `trytond_commission-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/locale/uk.po` & `trytond_commission-7.2.0/locale/zh_CN.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.invoice,agent:"
 msgid "Commission Agent"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "field:account.invoice.credit.start,with_agent:"
 msgid "With Agent"
-msgstr ""
+msgstr "Agents"
 
+#, fuzzy
 msgctxt "field:account.invoice.line,commissions:"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
+#, fuzzy
 msgctxt "field:account.invoice.line,from_commissions:"
 msgid "From Commissions"
-msgstr ""
+msgstr "From Commissions"
 
 msgctxt "field:account.invoice.line,principal:"
 msgid "Commission Principal"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission,agent:"
 msgid "Agent"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:commission,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:commission,base_amount:"
 msgid "Base Amount"
 msgstr ""
 
 msgctxt "field:commission,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:commission,invoice_line:"
 msgid "Invoice Line"
 msgstr ""
 
 msgctxt "field:commission,invoice_state:"
 msgid "Invoice State"
@@ -54,17 +60,18 @@
 msgid "Origin"
 msgstr ""
 
 msgctxt "field:commission,product:"
 msgid "Product"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission,type_:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
 msgctxt "field:commission.agent,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:commission.agent,currency:"
 msgid "Currency"
@@ -82,73 +89,80 @@
 msgid "Plan"
 msgstr ""
 
 msgctxt "field:commission.agent,selections:"
 msgid "Selections"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.agent,type_:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "field:commission.agent.selection,agent:"
 msgid "Agent"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:commission.agent.selection,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:commission.agent.selection,employee:"
 msgid "Employee"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.agent.selection,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:commission.agent.selection,party:"
 msgid "Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.agent.selection,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "写入日期"
 
+#, fuzzy
 msgctxt "field:commission.create_invoice.ask,agents:"
 msgid "Agents"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:commission.create_invoice.ask,from_:"
 msgid "From"
 msgstr ""
 
 msgctxt "field:commission.create_invoice.ask,to:"
 msgid "To"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.create_invoice.ask,type_:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
 msgctxt "field:commission.plan,commission_method:"
 msgid "Commission Method"
 msgstr ""
 
 msgctxt "field:commission.plan,commission_product:"
 msgid "Commission Product"
 msgstr ""
 
 msgctxt "field:commission.plan,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.plan,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
 msgctxt "field:commission.plan.line,category:"
 msgid "Category"
 msgstr ""
 
 msgctxt "field:commission.plan.line,formula:"
 msgid "Formula"
@@ -158,17 +172,18 @@
 msgid "Plan"
 msgstr ""
 
 msgctxt "field:commission.plan.line,product:"
 msgid "Product"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.reporting.agent,agent:"
 msgid "Agent"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:commission.reporting.agent,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent,base_amount:"
 msgid "Base Amount"
@@ -186,17 +201,18 @@
 msgid "Number"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent,time_series:"
 msgid "Time Series"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,agent:"
 msgid "Agent"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:commission.reporting.agent.time_series,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent.time_series,base_amount:"
 msgid "Base Amount"
@@ -206,109 +222,122 @@
 msgid "Base Amount Trend"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent.time_series,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:commission.reporting.agent.time_series,number:"
 msgid "Number"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.reporting.context,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "写入日期"
 
+#, fuzzy
 msgctxt "field:commission.reporting.context,invoiced:"
 msgid "Invoiced"
-msgstr ""
+msgstr "Invoice"
 
 msgctxt "field:commission.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:commission.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:commission.reporting.context,type:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "field:party.party,agents:"
 msgid "Agents"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:product.product,principals:"
 msgid "Commission Principals"
 msgstr ""
 
 msgctxt "field:product.template,principals:"
 msgid "Commission Principals"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template-commission.agent,agent:"
 msgid "Agent"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "field:product.template-commission.agent,template:"
 msgid "Template"
 msgstr ""
 
 msgctxt "field:sale.line,principal:"
 msgid "Commission Principal"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.sale,agent:"
 msgid "Commission Agent"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "field:stock.move,commission_price:"
 msgid "Commission Price"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "field:stock.reporting.margin.context,include_commission:"
 msgid "Include Commission"
-msgstr ""
+msgstr "Commission"
 
 msgctxt "help:account.invoice,agent:"
 msgid "The agent who receives a commission for the invoice."
 msgstr ""
 
 msgctxt "help:account.invoice.credit.start,with_agent:"
 msgid "Check to keep the original invoice's agent."
 msgstr ""
 
 msgctxt "help:account.invoice.line,principal:"
 msgid "The principal who pays a commission for the invoice line."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:commission,date:"
 msgid "When the commission is due."
-msgstr ""
+msgstr "Create Commission Invoices"
 
 msgctxt "help:commission,invoice_state:"
 msgid "The current state of the invoice that the commission appears on."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:commission,origin:"
 msgid "The source of the commission."
-msgstr ""
+msgstr "Create Commission Invoices"
 
 msgctxt "help:commission,product:"
 msgid "The product that is used on the invoice line."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:commission.agent,party:"
 msgid "The party for whom the commission is calculated."
-msgstr ""
+msgstr "Create Commission Invoices"
 
 msgctxt "help:commission.agent,plan:"
 msgid "The plan used to calculate the commission."
 msgstr ""
 
 msgctxt "help:commission.agent.selection,end_date:"
 msgid "The last date that the agent will be considered for selection."
@@ -320,29 +349,33 @@
 
 msgctxt "help:commission.create_invoice.ask,agents:"
 msgid ""
 "Limit to commissions for these agents.\n"
 "If empty all agents of the selected type are used."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:commission.create_invoice.ask,from_:"
 msgid "Limit to commissions from this date."
-msgstr ""
+msgstr "Create Commission Invoices"
 
+#, fuzzy
 msgctxt "help:commission.create_invoice.ask,to:"
 msgid "Limit to commissions to this date."
-msgstr ""
+msgstr "Create Commission Invoices"
 
+#, fuzzy
 msgctxt "help:commission.create_invoice.ask,type_:"
 msgid "Limit to commissions of this type."
-msgstr ""
+msgstr "Create Commission Invoices"
 
+#, fuzzy
 msgctxt "help:commission.plan,commission_method:"
 msgid "When the commission is due."
-msgstr ""
+msgstr "Create Commission Invoices"
 
 msgctxt "help:commission.plan,commission_product:"
 msgid "The product that is used on the invoice lines."
 msgstr ""
 
 msgctxt "help:commission.plan,lines:"
 msgid "The formulas used to calculate the commission for different criteria."
@@ -385,101 +418,112 @@
 
 msgctxt "help:sale.sale,agent:"
 msgid "The agent who receives a commission for the sale."
 msgstr ""
 
 msgctxt "model:account.journal,name:journal_commission"
 msgid "Commission"
-msgstr ""
+msgstr "Commission"
 
+#, fuzzy
 msgctxt "model:commission,name:"
 msgid "Commission"
-msgstr ""
+msgstr "Commission"
 
+#, fuzzy
 msgctxt "model:commission.agent,name:"
 msgid "Commission Agent"
-msgstr ""
+msgstr "Commission Plans"
 
 msgctxt "model:commission.agent.selection,name:"
 msgid "Agent Selection"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:commission.create_invoice.ask,name:"
 msgid "Create Commission Invoice"
-msgstr ""
+msgstr "Create Commission Invoices"
 
+#, fuzzy
 msgctxt "model:commission.plan,name:"
 msgid "Commission Plan"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "model:commission.plan.line,name:"
 msgid "Commission Plan Line"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "model:commission.reporting.agent,name:"
 msgid "Commission Reporting per Agent"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "model:commission.reporting.agent.time_series,name:"
 msgid "Commission Reporting per Agent"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "model:commission.reporting.context,name:"
 msgid "Commission Reporting Context"
-msgstr ""
+msgstr "Commission Plans"
 
 msgctxt "model:ir.action,name:act_agent_form"
 msgid "Agents"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "model:ir.action,name:act_agent_selections"
 msgid "Selections"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_commission_create_invoice"
 msgid "Create Commission Invoices"
-msgstr ""
+msgstr "Create Commission Invoices"
 
 msgctxt "model:ir.action,name:act_commission_form"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
 msgctxt "model:ir.action,name:act_commission_form2"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
 msgctxt "model:ir.action,name:act_commission_from_relate"
 msgid "From Commissions"
-msgstr ""
+msgstr "From Commissions"
 
 msgctxt "model:ir.action,name:act_commission_relate"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
 msgctxt "model:ir.action,name:act_plan_form"
 msgid "Plans"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_agent"
 msgid "Commissions per Agent"
-msgstr ""
+msgstr "Commission Plans"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_agent_time_series"
 msgid "Commissions per Agent"
-msgstr ""
+msgstr "Commission Plans"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_commission_form_domain_all"
 msgid "All"
 msgstr ""
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_commission_form_domain_to_invoice"
 msgid "To Invoice"
-msgstr ""
+msgstr "Invoice"
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_commission"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending commissions "
 "with company \"%(company)s\"."
 msgstr ""
 
@@ -487,15 +531,15 @@
 msgid ""
 "Invalid formula \"%(formula)s\" in commission plan line \"%(line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:commission_invoice_button"
 msgid "Invoice"
-msgstr ""
+msgstr "Invoice"
 
 msgctxt "model:ir.rule.group,name:rule_group_agent_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_agent_companies"
 msgid "User in companies"
@@ -504,67 +548,71 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_agent_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_agent_form"
 msgid "Agents"
-msgstr ""
+msgstr "Agents"
 
 msgctxt "model:ir.ui.menu,name:menu_commission"
 msgid "Commission"
-msgstr ""
+msgstr "Commission"
 
 msgctxt "model:ir.ui.menu,name:menu_commission_create_invoice"
 msgid "Create Commission Invoices"
-msgstr ""
+msgstr "Create Commission Invoices"
 
 msgctxt "model:ir.ui.menu,name:menu_commission_form"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Налаштування"
+msgstr "设置"
 
 msgctxt "model:ir.ui.menu,name:menu_plan_form"
 msgid "Plans"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Звітність"
+msgstr "报告"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_commission"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
 msgctxt "model:product.template-commission.agent,name:"
 msgid "Product Template - Commission Agent"
 msgstr ""
 
 msgctxt "model:res.group,name:group_commission"
 msgid "Commission"
-msgstr ""
+msgstr "Commission"
 
 msgctxt "model:res.group,name:group_commission_admin"
 msgid "Commission Administration"
-msgstr ""
+msgstr "Commission Administration"
 
+#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Commission"
-msgstr ""
+msgstr "Commission"
 
+#, fuzzy
 msgctxt "selection:commission,invoice_state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "selection:commission,invoice_state:"
 msgid "Invoiced"
-msgstr ""
+msgstr "Invoice"
 
 msgctxt "selection:commission,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:commission,type_:"
 msgid "Incoming"
@@ -618,34 +666,40 @@
 msgid "Incoming"
 msgstr ""
 
 msgctxt "selection:commission.reporting.context,type:"
 msgid "Outgoing"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.invoice.line:"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
 msgctxt "view:commission.agent.selection:"
 msgid "Criteria"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:party.party:"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
+#, fuzzy
 msgctxt "view:sale.line:"
 msgid "Commissions"
-msgstr ""
+msgstr "Commissions"
 
+#, fuzzy
 msgctxt "wizard_button:commission.create_invoice,ask,create_:"
 msgid "OK"
-msgstr ""
+msgstr "确定"
 
+#, fuzzy
 msgctxt "wizard_button:commission.create_invoice,ask,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
```

### Comparing `trytond_commission-7.0.0/locale/zh_CN.po` & `trytond_commission-7.2.0/locale/ro.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,412 +1,395 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.invoice,agent:"
 msgid "Commission Agent"
-msgstr "Commission Plans"
+msgstr "Agent comisionar"
 
-#, fuzzy
 msgctxt "field:account.invoice.credit.start,with_agent:"
 msgid "With Agent"
-msgstr "Agents"
+msgstr "Cu agentul"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,commissions:"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr "Comisioane"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,from_commissions:"
 msgid "From Commissions"
-msgstr "From Commissions"
+msgstr "Din comisioane"
 
 msgctxt "field:account.invoice.line,principal:"
 msgid "Commission Principal"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:commission,agent:"
 msgid "Agent"
-msgstr "Agents"
+msgstr "Agent"
 
 msgctxt "field:commission,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
+#, fuzzy
 msgctxt "field:commission,base_amount:"
 msgid "Base Amount"
-msgstr ""
+msgstr "Suma de bază"
 
 msgctxt "field:commission,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valută"
 
-#, fuzzy
 msgctxt "field:commission,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:commission,invoice_line:"
 msgid "Invoice Line"
-msgstr ""
+msgstr "Rând Factură"
 
 msgctxt "field:commission,invoice_state:"
 msgid "Invoice State"
-msgstr ""
+msgstr "Stare Factura"
 
 msgctxt "field:commission,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:commission,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
-#, fuzzy
 msgctxt "field:commission,type_:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
 msgctxt "field:commission.agent,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:commission.agent,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:commission.agent,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:commission.agent,pending_amount:"
 msgid "Pending Amount"
-msgstr ""
+msgstr "Sumă în așteptare"
 
 msgctxt "field:commission.agent,plan:"
 msgid "Plan"
-msgstr ""
+msgstr "Plan"
 
 msgctxt "field:commission.agent,selections:"
 msgid "Selections"
-msgstr ""
+msgstr "Selecții"
 
-#, fuzzy
 msgctxt "field:commission.agent,type_:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
-#, fuzzy
 msgctxt "field:commission.agent.selection,agent:"
 msgid "Agent"
-msgstr "Agents"
+msgstr "Agent"
 
 msgctxt "field:commission.agent.selection,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:commission.agent.selection,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Angajat"
 
-#, fuzzy
 msgctxt "field:commission.agent.selection,end_date:"
 msgid "End Date"
-msgstr "日期格式"
+msgstr "Data de încheiere"
 
 msgctxt "field:commission.agent.selection,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
-#, fuzzy
 msgctxt "field:commission.agent.selection,start_date:"
 msgid "Start Date"
-msgstr "写入日期"
+msgstr "Data de Început"
 
-#, fuzzy
 msgctxt "field:commission.create_invoice.ask,agents:"
 msgid "Agents"
-msgstr "Agents"
+msgstr "Agenți"
 
 msgctxt "field:commission.create_invoice.ask,from_:"
 msgid "From"
-msgstr ""
+msgstr "De la"
 
 msgctxt "field:commission.create_invoice.ask,to:"
 msgid "To"
-msgstr ""
+msgstr "Către"
 
-#, fuzzy
 msgctxt "field:commission.create_invoice.ask,type_:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
+#, fuzzy
 msgctxt "field:commission.plan,commission_method:"
 msgid "Commission Method"
-msgstr ""
+msgstr "Metodă de Comision"
 
 msgctxt "field:commission.plan,commission_product:"
 msgid "Commission Product"
 msgstr ""
 
 msgctxt "field:commission.plan,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
-#, fuzzy
 msgctxt "field:commission.plan,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nume"
 
 msgctxt "field:commission.plan.line,category:"
 msgid "Category"
-msgstr ""
+msgstr "Categorie"
 
 msgctxt "field:commission.plan.line,formula:"
 msgid "Formula"
-msgstr ""
+msgstr "Formulă"
 
 msgctxt "field:commission.plan.line,plan:"
 msgid "Plan"
-msgstr ""
+msgstr "Plan"
 
 msgctxt "field:commission.plan.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent,agent:"
 msgid "Agent"
-msgstr "Agents"
+msgstr "Agent"
 
 msgctxt "field:commission.reporting.agent,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
+#, fuzzy
 msgctxt "field:commission.reporting.agent,base_amount:"
 msgid "Base Amount"
-msgstr ""
+msgstr "Suma de bază"
 
 msgctxt "field:commission.reporting.agent,base_amount_trend:"
 msgid "Base Amount Trend"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
 msgctxt "field:commission.reporting.agent,number:"
 msgid "Number"
-msgstr ""
+msgstr "Număr"
 
+#, fuzzy
 msgctxt "field:commission.reporting.agent,time_series:"
 msgid "Time Series"
-msgstr ""
+msgstr "Seria de timp"
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,agent:"
 msgid "Agent"
-msgstr "Agents"
+msgstr "Agent"
 
 msgctxt "field:commission.reporting.agent.time_series,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
+#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,base_amount:"
 msgid "Base Amount"
-msgstr ""
+msgstr "Suma de bază"
 
 msgctxt "field:commission.reporting.agent.time_series,base_amount_trend:"
 msgid "Base Amount Trend"
 msgstr ""
 
 msgctxt "field:commission.reporting.agent.time_series,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
-#, fuzzy
 msgctxt "field:commission.reporting.agent.time_series,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:commission.reporting.agent.time_series,number:"
 msgid "Number"
-msgstr ""
+msgstr "Număr"
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,from_date:"
 msgid "From Date"
-msgstr "写入日期"
+msgstr "De la Data"
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,invoiced:"
 msgid "Invoiced"
-msgstr "Invoice"
+msgstr "Facturat"
 
 msgctxt "field:commission.reporting.context,period:"
 msgid "Period"
-msgstr ""
+msgstr "Perioadă"
 
 #, fuzzy
 msgctxt "field:commission.reporting.context,to_date:"
 msgid "To Date"
-msgstr "日期格式"
+msgstr "Până la Data"
 
-#, fuzzy
 msgctxt "field:commission.reporting.context,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tip"
 
-#, fuzzy
 msgctxt "field:party.party,agents:"
 msgid "Agents"
-msgstr "Agents"
+msgstr "Agenți"
 
 msgctxt "field:product.product,principals:"
 msgid "Commission Principals"
 msgstr ""
 
 msgctxt "field:product.template,principals:"
 msgid "Commission Principals"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template-commission.agent,agent:"
 msgid "Agent"
-msgstr "Agents"
+msgstr "Agent"
 
 msgctxt "field:product.template-commission.agent,template:"
 msgid "Template"
-msgstr ""
+msgstr "Șablon"
 
 msgctxt "field:sale.line,principal:"
 msgid "Commission Principal"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.sale,agent:"
 msgid "Commission Agent"
-msgstr "Commission Plans"
+msgstr "Agent comisionar"
 
-#, fuzzy
 msgctxt "field:stock.move,commission_price:"
 msgid "Commission Price"
-msgstr "Commission Plans"
+msgstr "Preț comision"
 
-#, fuzzy
 msgctxt "field:stock.reporting.margin.context,include_commission:"
 msgid "Include Commission"
-msgstr "Commission"
+msgstr "Includere comision"
 
 msgctxt "help:account.invoice,agent:"
 msgid "The agent who receives a commission for the invoice."
-msgstr ""
+msgstr "Agentul care primește un comision pentru factură."
 
 msgctxt "help:account.invoice.credit.start,with_agent:"
 msgid "Check to keep the original invoice's agent."
-msgstr ""
+msgstr "Bifați pentru a păstra agentul facturii originale."
 
 msgctxt "help:account.invoice.line,principal:"
 msgid "The principal who pays a commission for the invoice line."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:commission,date:"
 msgid "When the commission is due."
-msgstr "Create Commission Invoices"
+msgstr "Când se datorează comisionul."
 
 msgctxt "help:commission,invoice_state:"
 msgid "The current state of the invoice that the commission appears on."
-msgstr ""
+msgstr "Starea actuală a facturii pe care apare comisionul."
 
-#, fuzzy
 msgctxt "help:commission,origin:"
 msgid "The source of the commission."
-msgstr "Create Commission Invoices"
+msgstr "Sursa comisionului."
 
 msgctxt "help:commission,product:"
 msgid "The product that is used on the invoice line."
-msgstr ""
+msgstr "Produsul care este utilizat pe rândul de factură."
 
-#, fuzzy
 msgctxt "help:commission.agent,party:"
 msgid "The party for whom the commission is calculated."
-msgstr "Create Commission Invoices"
+msgstr "Partea pentru care se calculează comisionul."
 
 msgctxt "help:commission.agent,plan:"
 msgid "The plan used to calculate the commission."
-msgstr ""
+msgstr "Planul folosit pentru calcularea comisionului."
 
 msgctxt "help:commission.agent.selection,end_date:"
 msgid "The last date that the agent will be considered for selection."
 msgstr ""
+"Ultima dată la care agentul va fi luat în considerare pentru selecție."
 
 msgctxt "help:commission.agent.selection,start_date:"
 msgid "The first date that the agent will be considered for selection."
-msgstr ""
+msgstr "Prima dată la care agentul va fi luat în considerare pentru selecție."
 
 msgctxt "help:commission.create_invoice.ask,agents:"
 msgid ""
 "Limit to commissions for these agents.\n"
 "If empty all agents of the selected type are used."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:commission.create_invoice.ask,from_:"
 msgid "Limit to commissions from this date."
-msgstr "Create Commission Invoices"
+msgstr "Limitare la comisioane de la această dată."
 
-#, fuzzy
 msgctxt "help:commission.create_invoice.ask,to:"
 msgid "Limit to commissions to this date."
-msgstr "Create Commission Invoices"
+msgstr "Limitare la comisioane până la această dată."
 
-#, fuzzy
 msgctxt "help:commission.create_invoice.ask,type_:"
 msgid "Limit to commissions of this type."
-msgstr "Create Commission Invoices"
+msgstr "Limitare la comisioane de acest tip."
 
-#, fuzzy
 msgctxt "help:commission.plan,commission_method:"
 msgid "When the commission is due."
-msgstr "Create Commission Invoices"
+msgstr "Când se datorează comisionul."
 
 msgctxt "help:commission.plan,commission_product:"
 msgid "The product that is used on the invoice lines."
-msgstr ""
+msgstr "Produsul care este utilizat pe rândurile de factură."
 
 msgctxt "help:commission.plan,lines:"
 msgid "The formulas used to calculate the commission for different criteria."
 msgstr ""
+"Formulele utilizate pentru calcularea comisionului pentru diferite criterii."
 
+#, fuzzy
 msgctxt "help:commission.plan.line,category:"
 msgid "Apply only to products in the category."
-msgstr ""
+msgstr "Aplicare numai produselor din categorie."
 
+#, fuzzy
 msgctxt "help:commission.plan.line,formula:"
 msgid ""
 "The python expression used to calculate the amount of commission for the line.\n"
 "It is evaluated with:\n"
 "- amount: the original amount"
 msgstr ""
+"Expresia python folosită pentru a calcula suma comisionului pentru rând.\n"
+"Se evaluează cu:\n"
+"- suma: suma inițială"
 
+#, fuzzy
 msgctxt "help:commission.plan.line,plan:"
 msgid "The plan to which the line belongs."
-msgstr ""
+msgstr "Planul căruia îi aparține rândul."
 
+#, fuzzy
 msgctxt "help:commission.plan.line,product:"
 msgid "Apply only to the product."
-msgstr ""
+msgstr "Aplicare numai acestui produs."
 
 msgctxt "help:commission.reporting.context,invoiced:"
 msgid "Only include invoiced commissions."
-msgstr ""
+msgstr "Includeți doar comisioanele facturate."
 
 msgctxt "help:product.product,principals:"
 msgid "The principals who pay a commission when the product is sold."
 msgstr ""
 
 msgctxt "help:product.template,principals:"
 msgid "The principals who pay a commission when the product is sold."
@@ -414,205 +397,199 @@
 
 msgctxt "help:sale.line,principal:"
 msgid "The principal who pays a commission for the line."
 msgstr ""
 
 msgctxt "help:sale.sale,agent:"
 msgid "The agent who receives a commission for the sale."
-msgstr ""
+msgstr "Agentul care primește un comision pentru vânzare."
 
 msgctxt "model:account.journal,name:journal_commission"
 msgid "Commission"
-msgstr "Commission"
+msgstr "Comision"
 
-#, fuzzy
 msgctxt "model:commission,name:"
 msgid "Commission"
-msgstr "Commission"
+msgstr "Comision"
 
-#, fuzzy
 msgctxt "model:commission.agent,name:"
 msgid "Commission Agent"
-msgstr "Commission Plans"
+msgstr ""
 
 msgctxt "model:commission.agent.selection,name:"
 msgid "Agent Selection"
-msgstr ""
+msgstr "Selectarea agentului"
 
-#, fuzzy
 msgctxt "model:commission.create_invoice.ask,name:"
 msgid "Create Commission Invoice"
-msgstr "Create Commission Invoices"
+msgstr "Creați factura de comision"
 
 #, fuzzy
 msgctxt "model:commission.plan,name:"
 msgid "Commission Plan"
-msgstr "Commission Plans"
+msgstr "Plan de Comisioane"
 
 #, fuzzy
 msgctxt "model:commission.plan.line,name:"
 msgid "Commission Plan Line"
-msgstr "Commission Plans"
+msgstr "Rând Plan de Comisioane"
 
-#, fuzzy
 msgctxt "model:commission.reporting.agent,name:"
 msgid "Commission Reporting per Agent"
-msgstr "Commission Plans"
+msgstr "Raportarea Comisioanelor per Agent"
 
-#, fuzzy
 msgctxt "model:commission.reporting.agent.time_series,name:"
 msgid "Commission Reporting per Agent"
-msgstr "Commission Plans"
+msgstr "Raportarea Comisioanelor per Agent"
 
 #, fuzzy
 msgctxt "model:commission.reporting.context,name:"
 msgid "Commission Reporting Context"
-msgstr "Commission Plans"
+msgstr "Contextul de raportare a Comisioanelor"
 
 msgctxt "model:ir.action,name:act_agent_form"
 msgid "Agents"
-msgstr "Agents"
+msgstr "Agenți"
 
 msgctxt "model:ir.action,name:act_agent_selections"
 msgid "Selections"
-msgstr ""
+msgstr "Selecții"
 
 msgctxt "model:ir.action,name:act_commission_create_invoice"
 msgid "Create Commission Invoices"
-msgstr "Create Commission Invoices"
+msgstr "Creați facturi de comision"
 
 msgctxt "model:ir.action,name:act_commission_form"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr "Comisioane"
 
 msgctxt "model:ir.action,name:act_commission_form2"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr "Comisioane"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_commission_from_relate"
 msgid "From Commissions"
-msgstr "From Commissions"
+msgstr "Din comisioane"
 
 msgctxt "model:ir.action,name:act_commission_relate"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr "Comisioane"
 
 msgctxt "model:ir.action,name:act_plan_form"
 msgid "Plans"
-msgstr ""
+msgstr "Planuri"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_agent"
 msgid "Commissions per Agent"
-msgstr "Commission Plans"
+msgstr "Comisioane per agent"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_agent_time_series"
 msgid "Commissions per Agent"
-msgstr "Commission Plans"
+msgstr "Comisioane per agent"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_commission_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "Tot"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_commission_form_domain_to_invoice"
 msgid "To Invoice"
-msgstr "Invoice"
+msgstr "De Facturat"
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_commission"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending commissions "
 "with company \"%(company)s\"."
 msgstr ""
+"Nu se poate șterge partea \"%(party)s\" în timp ce aceasta are achiziții în "
+"așteptare cu compania \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_plan_line_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in commission plan line \"%(line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
+"Formula \"%(formula)s\" nu este valabilă în rândul planului de comisioane "
+"\"%(line)s\" cu excepția \"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:commission_invoice_button"
 msgid "Invoice"
-msgstr "Invoice"
+msgstr "Factură"
 
 msgctxt "model:ir.rule.group,name:rule_group_agent_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_agent_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_agent_time_series_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.ui.menu,name:menu_agent_form"
 msgid "Agents"
-msgstr "Agents"
+msgstr "Agenți"
 
 msgctxt "model:ir.ui.menu,name:menu_commission"
 msgid "Commission"
-msgstr "Commission"
+msgstr "Comision"
 
 msgctxt "model:ir.ui.menu,name:menu_commission_create_invoice"
 msgid "Create Commission Invoices"
-msgstr "Create Commission Invoices"
+msgstr "Creare facturi de comision"
 
 msgctxt "model:ir.ui.menu,name:menu_commission_form"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr "Comisioane"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Configurare"
 
 msgctxt "model:ir.ui.menu,name:menu_plan_form"
 msgid "Plans"
-msgstr ""
+msgstr "Planuri"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "报告"
+msgstr "Raportare"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_commission"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr "Comisioane"
 
 msgctxt "model:product.template-commission.agent,name:"
 msgid "Product Template - Commission Agent"
 msgstr ""
 
 msgctxt "model:res.group,name:group_commission"
 msgid "Commission"
-msgstr "Commission"
+msgstr ""
 
 msgctxt "model:res.group,name:group_commission_admin"
 msgid "Commission Administration"
-msgstr "Commission Administration"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Commission"
-msgstr "Commission"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:commission,invoice_state:"
 msgid "Cancelled"
-msgstr "取消"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:commission,invoice_state:"
 msgid "Invoiced"
-msgstr "Invoice"
+msgstr ""
 
 msgctxt "selection:commission,invoice_state:"
 msgid "Paid"
 msgstr ""
 
 msgctxt "selection:commission,type_:"
 msgid "Incoming"
@@ -666,40 +643,34 @@
 msgid "Incoming"
 msgstr ""
 
 msgctxt "selection:commission.reporting.context,type:"
 msgid "Outgoing"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:account.invoice.line:"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr ""
 
 msgctxt "view:commission.agent.selection:"
 msgid "Criteria"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:party.party:"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:product.template:"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:sale.line:"
 msgid "Commissions"
-msgstr "Commissions"
+msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:commission.create_invoice,ask,create_:"
 msgid "OK"
-msgstr "确定"
+msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:commission.create_invoice,ask,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr ""
```

### Comparing `trytond_commission-7.0.0/message.xml` & `trytond_commission-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/party.py` & `trytond_commission-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/product.py` & `trytond_commission-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/sale.py` & `trytond_commission-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/sale.xml` & `trytond_commission-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/setup.py` & `trytond_commission-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/stock.py` & `trytond_commission-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/stock_reporting_margin.py` & `trytond_commission-7.2.0/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/stock_reporting_margin.xml` & `trytond_commission-7.2.0/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/tests/scenario_agent_selection.rst` & `trytond_commission-7.2.0/tests/scenario_agent_selection.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ========================
 Agent Selection Scenario
 ========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules(['commission', 'sale'])
@@ -72,16 +70,15 @@
 
 The agent is assigned on quotation::
 
     >>> sale.agent
     >>> sale.click('quote')
     >>> sale.state
     'quotation'
-    >>> sale.agent == agent
-    True
+    >>> assertEqual(sale.agent, agent)
 
 Agent is not set for yesterday sales::
 
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
     >>> sale.sale_date = yesterday
     >>> sale.party = customer
@@ -103,11 +100,9 @@
 
     >>> sale = Sale()
     >>> sale.party = other_customer
     >>> sale.agent
     >>> sale.click('quote')
     >>> sale.state
     'quotation'
-    >>> sale.quoted_by == employee
-    True
-    >>> sale.agent == agent
-    True
+    >>> assertEqual(sale.quoted_by, employee)
+    >>> assertEqual(sale.agent, agent)
```

### Comparing `trytond_commission-7.0.0/tests/scenario_commission.rst` & `trytond_commission-7.2.0/tests/scenario_commission.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Commission Scenario
 ===================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('commission')
@@ -180,34 +180,32 @@
     >>> pay = Wizard('account.invoice.pay', [invoice])
     >>> pay.form.payment_method = payment_method
     >>> pay.form.date = tomorrow
     >>> pay.execute('choice')
     >>> pay.state
     'end'
     >>> Commission = Model.get('commission')
-    >>> [c.date == tomorrow for c in Commission.find([])]
-    [True, True]
+    >>> for commission in Commission.find([]):
+    ...     assertEqual(commission.date, tomorrow)
 
 Create commission invoices::
 
     >>> create_invoice = Wizard('commission.create_invoice')
     >>> create_invoice.form.from_ = None
     >>> create_invoice.form.to = None
     >>> create_invoice.execute('create_')
 
     >>> invoice, = Invoice.find([
     ...         ('type', '=', 'in'),
     ...         ])
     >>> invoice.total_amount
     Decimal('10.00')
-    >>> invoice.party == agent_party
-    True
+    >>> assertEqual(invoice.party, agent_party)
     >>> invoice_line, = invoice.lines
-    >>> invoice_line.product == commission_product
-    True
+    >>> assertEqual(invoice_line.product, commission_product)
 
     >>> invoice, = Invoice.find([
     ...         ('type', '=', 'out'),
     ...         ('party', '=', principal.party.id),
     ...         ])
     >>> invoice.total_amount
     Decimal('10.00')
@@ -221,31 +219,29 @@
     >>> invoice, = Invoice.find([
     ...         ('type', '=', 'out'),
     ...         ('agent', '=', agent.id),
     ...         ])
     >>> credit = Wizard('account.invoice.credit', [invoice])
     >>> credit.execute('credit')
     >>> credit_note, = credit.actions[0]
-    >>> credit_note.agent == agent
-    True
+    >>> assertEqual(credit_note.agent, agent)
 
 Check commission reporting per agent::
 
     >>> with config.set_context(type='out', period='day'):
     ...     reporting_agent, = ReportingAgent.find([])
     ...     reporting_agent_timeseries, = ReportingAgentTimeseries.find([])
 
-    >>> reporting_agent.base_amount == Decimal('100.00')
-    True
-    >>> reporting_agent.amount == Decimal('10.0000')
-    True
+    >>> reporting_agent.base_amount
+    Decimal('100.00')
+    >>> reporting_agent.amount
+    Decimal('10.00')
     >>> reporting_agent.number
     1
 
-    >>> reporting_agent_timeseries.date == tomorrow
-    True
-    >>> reporting_agent_timeseries.base_amount == Decimal('100.00')
-    True
-    >>> reporting_agent_timeseries.amount == Decimal('10.00')
-    True
+    >>> assertEqual(reporting_agent_timeseries.date, tomorrow)
+    >>> reporting_agent_timeseries.base_amount
+    Decimal('100.00')
+    >>> reporting_agent_timeseries.amount
+    Decimal('10.00')
     >>> reporting_agent_timeseries.number
     1
```

### Comparing `trytond_commission-7.0.0/tests/scenario_commission_credit_posted_invoice.rst` & `trytond_commission-7.2.0/tests/scenario_commission_credit_posted_invoice.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =========================================
 Commission Credit Posted Invoice Scenario
 =========================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('commission')
 
     >>> Agent = Model.get('commission.agent')
     >>> Commission = Model.get('commission')
```

### Comparing `trytond_commission-7.0.0/tests/scenario_commission_stock.rst` & `trytond_commission-7.2.0/tests/scenario_commission_stock.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 =========================
 Commission Stock Scenario
 =========================
 
 Imports::
 
-    >>> from decimal import Decimal
     >>> import datetime as dt
+    >>> from decimal import Decimal
 
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
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules(
@@ -143,24 +142,24 @@
 
     >>> shipment, = sale.shipments
     >>> move, = shipment.inventory_moves
     >>> move.quantity = 3
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> sale.reload()
     >>> _, shipment = sale.shipments
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Post the invoice::
 
     >>> invoice, = sale.invoices
     >>> invoice.click('post')
@@ -179,26 +178,26 @@
     >>> context = {
     ...     'from_date': yesterday,
     ...     'to_date': today,
     ...     'period': 'day',
     ...     }
     >>> with config.set_context(context=context):
     ...     report, = MarginProduct.find([])
-    >>> report.cost == Decimal('250.0000')
-    True
-    >>> report.revenue == Decimal('500.0000')
-    True
+    >>> report.cost
+    Decimal('250.00')
+    >>> report.revenue
+    Decimal('500.00')
 
     >>> context['include_commission'] = True
     >>> with config.set_context(context=context):
     ...     report, = MarginProduct.find([])
-    >>> report.cost == Decimal('275.0000')
-    True
-    >>> report.revenue == Decimal('500.0000')
-    True
+    >>> report.cost
+    Decimal('275.00')
+    >>> report.revenue
+    Decimal('500.00')
 
 Update commission amount::
 
     >>> commission, = Commission.find([('agent.type_', '=', 'agent')])
     >>> commission.amount = Decimal('60.0000')
 
 Create commission invoice::
```

### Comparing `trytond_commission-7.0.0/tests/test_module.py` & `trytond_commission-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/tox.ini` & `trytond_commission-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/trytond_commission.egg-info/PKG-INFO` & `trytond_commission-7.2.0/trytond_commission.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-commission
-Version: 7.0.0
+Name: trytond_commission
+Version: 7.2.0
 Summary: Tryton module for commission
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
@@ -51,28 +51,28 @@
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
 Requires-Dist: python-sql
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: sparklines
 Requires-Dist: pygal; extra == "sparklines"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 #################
 Commission Module
 #################
 
 The *Commission Module* allows you to manage commission for sale's agent.
 A commission move is created when posting the invoice, following the agent's
```

### Comparing `trytond_commission-7.0.0/trytond_commission.egg-info/SOURCES.txt` & `trytond_commission-7.2.0/trytond_commission.egg-info/SOURCES.txt`

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

### Comparing `trytond_commission-7.0.0/view/agent_selection_form.xml` & `trytond_commission-7.2.0/view/agent_selection_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/view/commission_form.xml` & `trytond_commission-7.2.0/view/commission_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/view/invoice_line_form.xml` & `trytond_commission-7.2.0/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/view/plan_line_form.xml` & `trytond_commission-7.2.0/view/plan_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-7.0.0/view/reporting_context_form.xml` & `trytond_commission-7.2.0/view/reporting_context_form.xml`

 * *Files identical despite different names*

