# Comparing `tmp/trytond_account_es-7.0.1.tar.gz` & `tmp/trytond_account_es-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es-7.0.1.tar", last modified: Thu Apr  4 07:52:47 2024, max compression
+gzip compressed data, was "trytond_account_es-7.2.0.tar", last modified: Mon Apr 29 15:32:59 2024, max compression
```

## Comparing `trytond_account_es-7.0.1.tar` & `trytond_account_es-7.2.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.274936 trytond_account_es-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2258 2024-04-04 07:52:44.000000 trytond_account_es-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2024-04-04 07:52:44.000000 trytond_account_es-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-04 07:52:47.271603 trytond_account_es-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)   454723 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   417678 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1356 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   311313 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/account_pyme.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1186 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1087 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/aeat349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-03-25 21:39:48.000000 trytond_account_es-7.0.1/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/create_chart.xsl
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.264937 trytond_account_es-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2789 2024-03-03 16:24:20.000000 trytond_account_es-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.268270 trytond_account_es-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10593 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10727 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10656 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10242 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9321 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10537 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9119 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9682 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10407 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9020 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36721 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/reporting_tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12080 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/reporting_tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:52:47.274936 trytond_account_es-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3912 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   151042 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax_groups.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   158875 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   156637 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tax_pyme.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.268270 trytond_account_es-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/303_compensate.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4589 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_ec_operation_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8625 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5349 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_cancelled_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4400 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_compensate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4672 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tests/scenario_reporting_surcharge_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tests/vat_book.csv
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-02-05 16:24:27.000000 trytond_account_es-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.271603 trytond_account_es-7.0.1/trytond_account_es.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3430 2024-04-04 07:52:47.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:32.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:52:46.000000 trytond_account_es-7.0.1/trytond_account_es.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:52:47.271603 trytond_account_es-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/es_ec_operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/es_ec_operation_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/print_aeat_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_book_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_book_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view/vat_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-10-30 17:06:38.000000 trytond_account_es-7.0.1/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2258 2024-04-29 15:13:42.000000 trytond_account_es-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2024-04-29 15:13:42.000000 trytond_account_es-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   454723 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   417678 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/account_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1356 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/account_payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:14.000000 trytond_account_es-7.2.0/account_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   311313 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/account_pyme.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1186 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/aeat111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/aeat115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/aeat303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1087 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/aeat347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/aeat349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/create_chart.xsl
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.047791 trytond_account_es-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:53.000000 trytond_account_es-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_es-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.051124 trytond_account_es-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10593 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10727 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10656 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10242 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9321 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10537 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9119 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9682 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10407 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10148 2024-04-29 13:17:17.000000 trytond_account_es-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2024-02-04 18:51:26.000000 trytond_account_es-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36721 2024-01-27 09:58:52.000000 trytond_account_es-7.2.0/reporting_tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11942 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/reporting_tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3912 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   151042 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tax_groups.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   158875 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tax_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   156637 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tax_pyme.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.051124 trytond_account_es-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/tests/111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/tests/115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/303_compensate.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/tests/347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/tests/349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4577 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_ec_operation_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8647 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/tests/scenario_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4244 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5300 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_cancelled_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4394 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_compensate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4616 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_surcharge_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/vat_book.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:53.000000 trytond_account_es-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-04-29 15:13:37.000000 trytond_account_es-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/trytond_account_es.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3430 2024-04-29 15:32:59.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/es_ec_operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/es_ec_operation_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/view/print_aeat_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_book_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_book_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view.xml
```

### Comparing `trytond_account_es-7.0.1/CHANGELOG` & `trytond_account_es-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-04-04
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_es-7.0.1/COPYRIGHT` & `trytond_account_es-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/LICENSE` & `trytond_account_es-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/PKG-INFO` & `trytond_account_es-7.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_es
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton with Spanish chart of accounts
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
@@ -30,27 +30,27 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=1.1.0
 Requires-Dist: phonenumbers
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_eu<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_eu<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_asset<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_payment_sepa<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_advance_payment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_gift_card<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_asset<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_payment_sepa<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_advance_payment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_gift_card<7.3,>=7.2; extra == "test"
 
 Spanish Account Module
 ######################
 
 The Spanish account module defines the following charts of account:
 
  * Plan General Contable Español 2008
```

### Comparing `trytond_account_es-7.0.1/README.rst` & `trytond_account_es-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/__init__.py` & `trytond_account_es-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/account.py` & `trytond_account_es-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/account.xml` & `trytond_account_es-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/account_normal.xml` & `trytond_account_es-7.2.0/account_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/account_payment.py` & `trytond_account_es-7.2.0/account_payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/account_payment.xml` & `trytond_account_es-7.2.0/account_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/account_pyme.xml` & `trytond_account_es-7.2.0/account_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/aeat111.txt` & `trytond_account_es-7.2.0/aeat111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/aeat303.txt` & `trytond_account_es-7.2.0/aeat303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/aeat347.txt` & `trytond_account_es-7.2.0/aeat347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/aeat349.txt` & `trytond_account_es-7.2.0/aeat349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/company.py` & `trytond_account_es-7.2.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/create_chart.xsl` & `trytond_account_es-7.2.0/create_chart.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/doc/conf.py` & `trytond_account_es-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
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

### Comparing `trytond_account_es-7.0.1/doc/index.rst` & `trytond_account_es-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/bg.po` & `trytond_account_es-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/ca.po` & `trytond_account_es-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/cs.po` & `trytond_account_es-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/de.po` & `trytond_account_es-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/es.po` & `trytond_account_es-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/es_419.po` & `trytond_account_es-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/et.po` & `trytond_account_es-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/fa.po` & `trytond_account_es-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/fi.po` & `trytond_account_es-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/fr.po` & `trytond_account_es-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/hu.po` & `trytond_account_es-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/id.po` & `trytond_account_es-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/it.po` & `trytond_account_es-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/lo.po` & `trytond_account_es-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/lt.po` & `trytond_account_es-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/nl.po` & `trytond_account_es-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/pl.po` & `trytond_account_es-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/pt.po` & `trytond_account_es-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/ro.po` & `trytond_account_es-7.2.0/locale/ru.po`

 * *Files 9% similar despite different names*

```diff
@@ -16,79 +16,75 @@
 
 msgctxt "field:account.reporting.aeat.start,report:"
 msgid "Report"
 msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list,company_tax_identifier:"
 msgid "Company Tax Identifier"
 msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list,party_tax_identifier:"
 msgid "Party Tax Identifier"
 msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list.context,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.es_ec_operation_list.context,end_date:"
 msgid "End Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list.context,fiscalyear:"
 msgid "Fiscal Year"
-msgstr "An Fiscal"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list.context,period:"
 msgid "Period"
-msgstr "Perioadă"
+msgstr ""
 
 msgctxt "field:account.reporting.es_ec_operation_list.context,start_date:"
 msgid "Start Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es,base_amount:"
 msgid "Base Amount"
-msgstr "Suma"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_book_es,invoice:"
 msgid "Invoice"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_book_es,invoice_date:"
 msgid "Invoice Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_book_es,party_tax_identifier:"
 msgid "Party Tax Identifier"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_book_es,surcharge_tax:"
 msgid "Surcharge Tax"
@@ -98,70 +94,65 @@
 msgid "Surcharge Tax Amount"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_book_es,tax:"
 msgid "Tax"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es,tax_amount:"
 msgid "Tax Amount"
-msgstr "Suma"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es.context,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es.context,end_period:"
 msgid "End Period"
-msgstr "Perioadă"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_book_es.context,es_vat_book_type:"
 msgid "Type"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es.context,fiscalyear:"
 msgid "Fiscal Year"
-msgstr "An Fiscal"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.reporting.vat_book_es.context,start_period:"
 msgid "Start Period"
-msgstr "Perioadă"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,company_tax_identifier:"
 msgid "Company Tax Identifier"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,first_period_amount:"
 msgid "First Period Amount"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,fourth_period_amount:"
 msgid "Fourth Period Amount"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,party_tax_identifier:"
 msgid "Party Tax Identifier"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es,province_code:"
 msgid "Province Code"
@@ -173,19 +164,19 @@
 
 msgctxt "field:account.reporting.vat_list_es,third_period_amount:"
 msgid "Third Period Amount"
 msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es.context,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.reporting.vat_list_es.context,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.tax,es_ec_purchases_list_code:"
 msgid "Spanish EC Purchases List Code"
 msgstr ""
 
 msgctxt "field:account.tax,es_exclude_from_vat_book:"
 msgid "Exclude from Spanish VAT Book"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_es-7.0.1/locale/ru.po` & `trytond_account_es-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/sl.po` & `trytond_account_es-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/tr.po` & `trytond_account_es-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/locale/uk.po` & `trytond_account_es-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/party.py` & `trytond_account_es-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/reporting_tax.py` & `trytond_account_es-7.2.0/reporting_tax.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/reporting_tax.xml` & `trytond_account_es-7.2.0/reporting_tax.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_account_es-7.0.1/reporting_tax.xml` & `trytond_account_es-7.2.0/reporting_tax.xml`

```diff
@@ -75,22 +75,22 @@
     <menuitem parent="account.menu_reporting" action="act_vat_list_form" sequence="50" id="menu_vat_list"/>
     <record model="ir.ui.view" id="vat_list_context_view_form">
       <field name="model">account.reporting.vat_list_es.context</field>
       <field name="type">form</field>
       <field name="name">vat_list_context_form</field>
     </record>
     <record model="ir.model.access" id="access_vat_list">
-      <field name="model" search="[('model', '=', 'account.reporting.vat_list_es')]"/>
+      <field name="model">account.reporting.vat_list_es</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_vat_list_account">
-      <field name="model" search="[('model', '=', 'account.reporting.vat_list_es')]"/>
+      <field name="model">account.reporting.vat_list_es</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.report" id="report_aeat_347">
@@ -125,22 +125,22 @@
     <menuitem parent="account.menu_reporting" sequence="50" action="act_es_ec_operation_list_form" id="menu_es_ec_operation_list"/>
     <record model="ir.ui.view" id="es_ec_operation_list_context_view_form">
       <field name="model">account.reporting.es_ec_operation_list.context</field>
       <field name="type">form</field>
       <field name="name">es_ec_operation_list_context_form</field>
     </record>
     <record model="ir.model.access" id="access_es_ec_operation_list">
-      <field name="model" search="[('model', '=', 'account.reporting.es_ec_operation_list')]"/>
+      <field name="model">account.reporting.es_ec_operation_list</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_es_ec_operation_list_account">
-      <field name="model" search="[('model', '=', 'account.reporting.es_ec_operation_list')]"/>
+      <field name="model">account.reporting.es_ec_operation_list</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.report" id="report_aeat_349">
@@ -175,22 +175,22 @@
     <record model="ir.action.act_window.view" id="act_vat_book_list_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="vat_book_view_list"/>
       <field name="act_window" ref="act_vat_book_list"/>
     </record>
     <menuitem parent="account.menu_reporting" action="act_vat_book_list" id="menu_vat_book"/>
     <record model="ir.model.access" id="access_vat_book">
-      <field name="model" search="[('model', '=', 'account.reporting.vat_book_es')]"/>
+      <field name="model">account.reporting.vat_book_es</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_vat_book_account">
-      <field name="model" search="[('model', '=', 'account.reporting.vat_book_es')]"/>
+      <field name="model">account.reporting.vat_book_es</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.report" id="report_aeat_vat_book">
```

### Comparing `trytond_account_es-7.0.1/setup.py` & `trytond_account_es-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tax.xml` & `trytond_account_es-7.2.0/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tax_groups.xml` & `trytond_account_es-7.2.0/tax_groups.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tax_normal.xml` & `trytond_account_es-7.2.0/tax_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tax_pyme.xml` & `trytond_account_es-7.2.0/tax_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tests/111.txt` & `trytond_account_es-7.2.0/tests/111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tests/115.txt` & `trytond_account_es-7.2.0/tests/115.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tests/303.txt` & `trytond_account_es-7.2.0/tests/303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tests/303_compensate.txt` & `trytond_account_es-7.2.0/tests/303_compensate.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/tests/349.txt` & `trytond_account_es-7.2.0/tests/349.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-13492018B01000009DUNDER MIFFLIN                          T000000000DUNDER MIFFLIN                          3492018010001  000000000000001000000001000000000010000000000000000000000000015                                                                                                                                                                                                                                                                                                                           
+13492018B01000009DUNDER MIFFLIN                          T666666666DUNDER MIFFLIN                          3492018010001  000000000000001000000001000000000010000000000000000000000000015                                                                                                                                                                                                                                                                                                                           
 23492018B01000009                                                          BE0897290877     INTRACOMUNITARY SUPPLIER                A0000000010000
```

### Comparing `trytond_account_es-7.0.1/tests/scenario_ec_operation_list.rst` & `trytond_account_es-7.2.0/tests/scenario_ec_operation_list.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =====================================
 Account ES EC Operation List Scenario
 =====================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_fiscalyear)
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
@@ -45,30 +45,30 @@
 
     >>> Party = Model.get('party.party')
     >>> TaxRule = Model.get('account.tax.rule')
     >>> tax_rule, = TaxRule.find([
     ...         ('company', '=', company.id),
     ...         ('kind', '=', 'purchase'),
     ...         ('name', '=', 'Compras Intracomunitarias'),
-    ...     ])
+    ...         ])
     >>> party = Party(name='Intracomunitary Supplier')
     >>> party.supplier_tax_rule = tax_rule
     >>> tax_identifier = party.identifiers.new()
     >>> tax_identifier.type = 'eu_vat'
     >>> tax_identifier.code = 'BE0897290877'
     >>> party.save()
 
 Create account category::
 
     >>> Tax = Model.get('account.tax')
     >>> tax, = Tax.find([
     ...         ('company', '=', company.id),
     ...         ('group.kind', '=', 'purchase'),
     ...         ('name', '=', 'IVA 21% (bienes)'),
-    ...     ])
+    ...         ])
     >>> ProductCategory = Model.get('product.category')
     >>> account_category = ProductCategory(name="Account Category")
     >>> account_category.accounting = True
     >>> account_category.account_expense = expense
     >>> account_category.account_revenue = revenue
     >>> account_category.supplier_taxes.append(tax)
     >>> account_category.save()
@@ -141,9 +141,9 @@
     >>> credit.execute('credit')
     >>> invoice.reload()
 
 Operation appears in report with amount zero::
 
     >>> with config.set_context(context):
     ...     record, = ECOperationList.find([])
-    >>> record.amount == Decimal('0.0')
-    True
+    >>> record.amount
+    Decimal('0.00')
```

### Comparing `trytond_account_es-7.0.1/tests/scenario_reporting.rst` & `trytond_account_es-7.2.0/tests/scenario_reporting.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 Account ES Reporting Scenario
 =============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.tools import file_open
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model, Report, Wizard
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_fiscalyear)
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+    >>> from trytond.tools import file_open
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
     >>> tax_identifier = company.party.identifiers.new()
     >>> tax_identifier.type = 'eu_vat'
     >>> tax_identifier.code = 'ESB01000009'
+    >>> phone = company.party.contact_mechanisms.new()
+    >>> phone.value = '+34 666 66 66 66'
     >>> company.party.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
     ...     create_fiscalyear(
     ...         company, (dt.date(2018, 1, 1), dt.date(2018, 12, 31))))
@@ -164,80 +166,75 @@
     >>> aeat.form.report = '111'
     >>> aeat.form.periods.append(Period(period.id))
     >>> aeat.execute('choice')
     >>> extension, content, _, name = aeat.actions[0]
     >>> extension
     'txt'
     >>> with file_open('account_es/tests/111.txt') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('AEAT Model 111')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'AEAT Model 111-2018-01'
 
     >>> aeat = Wizard('account.reporting.aeat')
     >>> aeat.form.report = '115'
     >>> period = Period(period.id)
     >>> aeat.form.periods.append(Period(period.id))
     >>> aeat.execute('choice')
     >>> extension, content, _, name = aeat.actions[0]
     >>> extension
     'txt'
     >>> with file_open('account_es/tests/115.txt') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('AEAT Model 115')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'AEAT Model 115-2018-01'
 
     >>> aeat = Wizard('account.reporting.aeat')
     >>> aeat.form.report = '303'
     >>> aeat.form.periods.append(Period(period.id))
     >>> aeat.execute('choice')
     >>> extension, content, _, name = aeat.actions[0]
     >>> extension
     'txt'
     >>> with file_open('account_es/tests/303.txt') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('AEAT Model 303')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'AEAT Model 303-2018-01'
 
     >>> VatList = Model.get('account.reporting.vat_list_es')
     >>> context = {
     ...     'company': company.id,
     ...     'date': period.end_date,
     ...     }
     >>> with config.set_context(context):
     ...     vat_list_records = VatList.find([])
     ...     report = Report('account.reporting.aeat347')
     ...     extension, content, _, name = report.execute(vat_list_records)
     >>> extension
     'txt'
     >>> with file_open('account_es/tests/347.txt') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('AEAT Model 347')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'AEAT Model 347-...'
 
     >>> ECOperationList = Model.get('account.reporting.es_ec_operation_list')
     >>> context = {
     ...     'company': company.id,
     ...     'start_date': period.start_date,
     ...     'end_date': period.end_date,
     ...     }
     >>> with config.set_context(context):
     ...     records = ECOperationList.find([])
     ...     report = Report('account.reporting.aeat349')
     ...     extension, content, _, name = report.execute(records)
     >>> extension
     'txt'
     >>> with file_open('account_es/tests/349.txt') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('AEAT Model 349')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'AEAT Model 349-...'
 
 
 Only one tax of intracomunitary invoices is included on VAT Book::
 
     >>> VatBook = Model.get('account.reporting.vat_book_es')
     >>> context = {
     ...     'company': company.id,
@@ -245,16 +242,16 @@
     ...     'es_vat_book_type': 'R',
     ...     }
     >>> with config.set_context(context):
     ...     records = VatBook.find([])
     >>> len(records)
     2
     >>> supplier_record, = [r for r in records if r.party == supplier]
-    >>> supplier_record.base_amount == Decimal('100.00')
-    True
-    >>> supplier_record.tax_amount == Decimal('21.00')
-    True
+    >>> supplier_record.base_amount
+    Decimal('100.00')
+    >>> supplier_record.tax_amount
+    Decimal('21.00')
     >>> ec_supplier_record, = [r for r in records if r.party == ec_supplier]
-    >>> ec_supplier_record.base_amount == Decimal('100.00')
-    True
-    >>> ec_supplier_record.tax_amount == Decimal('21.00')
-    True
+    >>> ec_supplier_record.base_amount
+    Decimal('100.00')
+    >>> ec_supplier_record.tax_amount
+    Decimal('21.00')
```

### Comparing `trytond_account_es-7.0.1/tests/scenario_reporting_alternate_currency.rst` & `trytond_account_es-7.2.0/tests/scenario_reporting_alternate_currency.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Account ES Reporting Alternate Currency Scenario
 ================================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_fiscalyear)
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
@@ -99,37 +100,34 @@
     >>> VatList = Model.get('account.reporting.vat_list_es')
     >>> context = {
     ...     'company': company.id,
     ...     'date': today,
     ...     }
     >>> with config.set_context(context):
     ...     record, = VatList.find([])
-    >>> record.party == party
-    True
-    >>> record.amount == Decimal('121.00')
-    True
+    >>> assertEqual(record.party, party)
+    >>> record.amount
+    Decimal('121.00')
     >>> ECOperationList = Model.get('account.reporting.es_ec_operation_list')
     >>> context = {
     ...     'company': company.id,
     ...     'start_date': today,
     ...     'end_date': today,
     ...     }
     >>> with config.set_context(context):
     ...     record, = ECOperationList.find([])
-    >>> record.party == supplier
-    True
-    >>> record.amount == Decimal('50.00')
-    True
+    >>> assertEqual(record.party, supplier)
+    >>> record.amount
+    Decimal('50.00')
     >>> VatBook = Model.get('account.reporting.vat_book_es')
     >>> context = {
     ...     'company': company.id,
     ...     'fiscalyear': fiscalyear.id,
     ...     'es_vat_book_type': 'E',
     ...     }
     >>> with config.set_context(context):
     ...     record, = VatBook.find([])
-    >>> record.party == party
-    True
-    >>> record.base_amount == Decimal('100.00')
-    True
-    >>> record.tax_amount == Decimal('21.00')
-    True
+    >>> assertEqual(record.party, party)
+    >>> record.base_amount
+    Decimal('100.00')
+    >>> record.tax_amount
+    Decimal('21.00')
```

### Comparing `trytond_account_es-7.0.1/tests/scenario_reporting_cancelled_invoices.rst` & `trytond_account_es-7.2.0/tests/scenario_reporting_cancelled_invoices.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ================================================
 Account ES Reporting Cancelled Invoices Scenario
 ================================================
 
 Imports::
 
-    >>> import datetime
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_fiscalyear)
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
@@ -124,16 +123,16 @@
     'cancelled'
 
 Check reports::
 
     >>> with config.set_context(vat_list_context):
     ...     vat_list_records = VatList.find([])
     >>> vat_list_record, = vat_list_records
-    >>> vat_list_record.amount == Decimal(0)
-    True
+    >>> vat_list_record.amount
+    Decimal('0.00')
     >>> with config.set_context(vat_book_context):
     ...     vat_book_records = VatBook.find([])
     >>> len(vat_book_records)
     2
 
 Create another invoice::
 
@@ -145,28 +144,28 @@
     >>> line.product = product
     >>> line.quantity = 5
     >>> line.unit_price = Decimal('40')
     >>> invoice.click('post')
     >>> with config.set_context(vat_list_context):
     ...     vat_list_records = VatList.find([])
     >>> vat_list_record, = vat_list_records
-    >>> vat_list_record.amount == Decimal('242.0')
-    True
+    >>> vat_list_record.amount
+    Decimal('242.00')
     >>> with config.set_context(vat_book_context):
     ...     vat_book_records = VatBook.find([])
     >>> len(vat_book_records)
     3
 
 Cancel the invoice and check reports::
 
     >>> invoice.click('cancel')
     >>> invoice.state
     'cancelled'
     >>> with config.set_context(vat_list_context):
     ...     vat_list_records = VatList.find([])
     >>> vat_list_record, = vat_list_records
-    >>> vat_list_record.amount == Decimal(0)
-    True
+    >>> vat_list_record.amount
+    Decimal('0.00')
     >>> with config.set_context(vat_book_context):
     ...     vat_book_records = VatBook.find([])
     >>> len(vat_book_records)
     2
```

### Comparing `trytond_account_es-7.0.1/tests/scenario_reporting_compensate.rst` & `trytond_account_es-7.2.0/tests/scenario_reporting_compensate.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Account ES Compensated Reporting Scenario
 =========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.tools import file_open
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_fiscalyear)
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+    >>> from trytond.tools import file_open
 
 Activate modules::
 
     >>> config = activate_modules(['account_es', 'account_invoice'])
 
 Create company::
 
@@ -127,11 +127,10 @@
     >>> aeat.form.report = '303'
     >>> aeat.form.periods.append(Period(period.id))
     >>> aeat.execute('choice')
     >>> extension, content, _, name = aeat.actions[0]
     >>> extension
     'txt'
     >>> with file_open('account_es/tests/303_compensate.txt') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('AEAT Model 303')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'AEAT Model 303-2018-02'
```

### Comparing `trytond_account_es-7.0.1/tests/scenario_reporting_surcharge_tax.rst` & `trytond_account_es-7.2.0/tests/scenario_reporting_surcharge_tax.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Account ES Reporting Surcharge Tax Scenario
 ===========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.tools import file_open
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model, Report
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_fiscalyear)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+    >>> from trytond.tools import file_open
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
@@ -115,29 +115,26 @@
     >>> with config.set_context(context):
     ...     records = VatBook.find([])
     ...     report = Report('account.reporting.aeat.vat_book')
     ...     extension, content, _, name = report.execute(records)
     >>> len(records)
     3
     >>> tax_record = [r for r in records if not r.surcharge_tax][0]
-    >>> tax_record.party == party
-    True
-    >>> tax_record.base_amount == Decimal('100.00')
-    True
-    >>> tax_record.tax_amount == Decimal('21.00')
-    True
+    >>> assertEqual(tax_record.party, party)
+    >>> tax_record.base_amount
+    Decimal('100.00')
+    >>> tax_record.tax_amount
+    Decimal('21.00')
     >>> surcharge_tax_record = [r for r in records if r.surcharge_tax][0]
-    >>> surcharge_tax_record.party == surcharge_party
-    True
-    >>> surcharge_tax_record.base_amount == Decimal('50.00')
-    True
-    >>> surcharge_tax_record.tax_amount == Decimal('10.50')
-    True
-    >>> surcharge_tax_record.surcharge_tax_amount == Decimal('2.60')
-    True
+    >>> assertEqual(surcharge_tax_record.party, surcharge_party)
+    >>> surcharge_tax_record.base_amount
+    Decimal('50.00')
+    >>> surcharge_tax_record.tax_amount
+    Decimal('10.50')
+    >>> surcharge_tax_record.surcharge_tax_amount
+    Decimal('2.60')
     >>> with file_open('account_es/tests/vat_book.csv', 'rb') as f:
-    ...     content == f.read()
-    True
-    >>> name.startswith('VAT Book')
-    True
+    ...     assertEqual(content, f.read())
+    >>> name
+    'VAT Book-...'
     >>> extension
     'csv'
```

### Comparing `trytond_account_es-7.0.1/tox.ini` & `trytond_account_es-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/trytond_account_es.egg-info/PKG-INFO` & `trytond_account_es-7.2.0/trytond_account_es.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_es
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton with Spanish chart of accounts
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
@@ -30,27 +30,27 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=1.1.0
 Requires-Dist: phonenumbers
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_eu<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_eu<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_asset<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_payment_sepa<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_advance_payment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_gift_card<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_asset<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_payment_sepa<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_advance_payment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_gift_card<7.3,>=7.2; extra == "test"
 
 Spanish Account Module
 ######################
 
 The Spanish account module defines the following charts of account:
 
  * Plan General Contable Español 2008
```

### Comparing `trytond_account_es-7.0.1/trytond_account_es.egg-info/SOURCES.txt` & `trytond_account_es-7.2.0/trytond_account_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/view/tax_form.xml` & `trytond_account_es-7.2.0/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/view/tax_template_form.xml` & `trytond_account_es-7.2.0/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/view/vat_book_list.xml` & `trytond_account_es-7.2.0/view/vat_book_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/view/vat_list_list.xml` & `trytond_account_es-7.2.0/view/vat_list_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.0.1/view.xml` & `trytond_account_es-7.2.0/view.xml`

 * *Files identical despite different names*

