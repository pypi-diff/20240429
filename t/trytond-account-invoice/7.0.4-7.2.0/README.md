# Comparing `tmp/trytond_account_invoice-7.0.4.tar.gz` & `tmp/trytond_account_invoice-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice-7.0.4.tar", last modified: Wed Apr 17 10:45:40 2024, max compression
+gzip compressed data, was "trytond_account_invoice-7.2.0.tar", last modified: Mon Apr 29 15:33:33 2024, max compression
```

## Comparing `trytond_account_invoice-7.0.4.tar` & `trytond_account_invoice-7.2.0.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.091000 trytond_account_invoice-7.0.4/
--rw-r--r--   0 ced       (1000) ced       (1000)     8321 2024-04-17 10:45:37.000000 trytond_account_invoice-7.0.4/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-17 10:45:36.000000 trytond_account_invoice-7.0.4/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-17 10:45:40.091000 trytond_account_invoice-7.0.4/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1977 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14844 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4994 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.081000 trytond_account_invoice-7.0.4/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-03-03 16:24:20.000000 trytond_account_invoice-7.0.4/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.081000 trytond_account_invoice-7.0.4/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/doc/usage/amend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/doc/usage/prepare.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3685 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.081000 trytond_account_invoice-7.0.4/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/icons/tryton-invoice.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    93989 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/invoice.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)   135624 2024-04-12 22:38:27.000000 trytond_account_invoice-7.0.4/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24229 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.084333 trytond_account_invoice-7.0.4/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37836 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38969 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32667 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39531 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38699 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33590 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36710 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40759 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32628 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39437 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35285 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35155 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35914 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38488 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36664 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38646 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33293 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36237 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37024 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38499 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37347 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32610 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31192 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37385 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6174 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3274 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2389 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-02-12 10:16:44.000000 trytond_account_invoice-7.0.4/payment_term.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/payment_term.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:45:40.091000 trytond_account_invoice-7.0.4/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-03-03 16:24:03.000000 trytond_account_invoice-7.0.4/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.084333 trytond_account_invoice-7.0.4/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3188 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_cancelling_invoice_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4029 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_credit_note.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    13194 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5700 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2856 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_alternate_currency_lower_rate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3472 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_alternate_currency_rate_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_alternative_payee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_customer_sequential.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_group_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1868 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2606 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_manual_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3521 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_overpayment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2506 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_report_revision.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_reschedule_lines.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3480 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_supplier_post_paid.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3585 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_tax_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3408 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_invoice_with_credit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-04 07:51:34.000000 trytond_account_invoice-7.0.4/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.091000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-17 10:45:39.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     6188 2024-04-17 10:45:40.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:45:39.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-17 10:45:39.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:33.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-17 10:45:39.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:45:39.000000 trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:40.091000 trytond_account_invoice-7.0.4/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4672 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_report_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_report_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_sequence_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_tax_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_tax_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/invoice_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/move_line_list_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/pay_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_method_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/view/payment_term_line_relativedelta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/view/payment_term_line_relativedelta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-02-05 16:24:27.000000 trytond_account_invoice-7.0.4/view/payment_term_line_relativedelta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account_invoice-7.0.4/view/payment_term_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.430225 trytond_account_invoice-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8135 2024-04-29 15:14:14.000000 trytond_account_invoice-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:14:13.000000 trytond_account_invoice-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-29 15:33:33.430225 trytond_account_invoice-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1977 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14844 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4877 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.420225 trytond_account_invoice-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:54.000000 trytond_account_invoice-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.420225 trytond_account_invoice-7.2.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/amend.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/prepare.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.420225 trytond_account_invoice-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/icons/tryton-invoice.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    94000 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/invoice.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)   139705 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23815 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.423559 trytond_account_invoice-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    38393 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39802 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33224 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40399 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39520 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34147 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37479 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41650 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33185 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40336 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35842 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35712 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36471 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39045 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37221 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39539 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33850 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38882 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39056 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38148 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33167 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31749 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38154 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6873 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3324 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2389 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-04-13 17:12:23.000000 trytond_account_invoice-7.2.0/payment_term.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/payment_term.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:33.430225 trytond_account_invoice-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.423559 trytond_account_invoice-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3122 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_cancelling_invoice_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4010 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_credit_note.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    13167 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6057 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_exchange.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_lower_rate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3488 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_rate_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_alternative_payee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2666 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_customer_sequential.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_group_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2581 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_manual_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3501 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_overpayment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_report_revision.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2989 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_reschedule_lines.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7240 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3373 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier_post_paid.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3986 2024-04-27 16:30:39.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_tax_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3349 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_invoice_with_credit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3632 2024-04-22 12:14:36.000000 trytond_account_invoice-7.2.0/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:54.000000 trytond_account_invoice-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-29 15:14:09.000000 trytond_account_invoice-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.426892 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     6312 2024-04-29 15:33:33.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:32.000000 trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:33.426892 trytond_account_invoice-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-07-26 15:07:10.000000 trytond_account_invoice-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4830 2024-04-29 13:17:17.000000 trytond_account_invoice-7.2.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-03-15 08:41:28.000000 trytond_account_invoice-7.2.0/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/invoice_report_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/invoice_report_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/invoice_sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/invoice_sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/invoice_sequence_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_tax_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/invoice_tax_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-28 07:43:48.000000 trytond_account_invoice-7.2.0/view/invoice_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/move_line_list_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-26 15:26:42.000000 trytond_account_invoice-7.2.0/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/pay_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-01-27 09:58:52.000000 trytond_account_invoice-7.2.0/view/pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-02-04 18:51:26.000000 trytond_account_invoice-7.2.0/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_method_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-01-16 14:00:20.000000 trytond_account_invoice-7.2.0/view/payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2024-03-17 11:01:36.000000 trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-03-17 11:01:36.000000 trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-03-17 11:01:36.000000 trytond_account_invoice-7.2.0/view/payment_term_line_relativedelta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_account_invoice-7.2.0/view/payment_term_tree.xml
```

### Comparing `trytond_account_invoice-7.0.4/CHANGELOG` & `trytond_account_invoice-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 
-Version 7.0.4 - 2024-04-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.3 - 2024-04-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-02-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Raise a warning when validating invoice with non default taxes
+* Book currency exchange amount in dedicated account
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Always allow editing invoice reference, description and comment by accounting administrator
 * Allow refreshing invoice report cache
```

### Comparing `trytond_account_invoice-7.0.4/COPYRIGHT` & `trytond_account_invoice-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/LICENSE` & `trytond_account_invoice-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/PKG-INFO` & `trytond_account_invoice-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.0.4
+Version: 7.2.0
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -50,23 +50,23 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ######################
 Account Invoice Module
 ######################
 
 The *Account Invoice Module* adds the concept of invoicing to Tryton.
 It allows the creation of customer and supplier invoices, and can handle the
```

### Comparing `trytond_account_invoice-7.0.4/__init__.py` & `trytond_account_invoice-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/account.py` & `trytond_account_invoice-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/account.xml` & `trytond_account_invoice-7.2.0/account.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_invoice-7.0.4/account.xml` & `trytond_account_invoice-7.2.0/account.xml`

```diff
@@ -62,31 +62,31 @@
     <record model="ir.ui.view" id="invoice_sequence_view_list_sequence">
       <field name="model">account.fiscalyear.invoice_sequence</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">invoice_sequence_list_sequence</field>
     </record>
     <record model="ir.model.access" id="access_invoice_sequence">
-      <field name="model" search="[('model', '=', 'account.fiscalyear.invoice_sequence')]"/>
+      <field name="model">account.fiscalyear.invoice_sequence</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_sequence_admin">
-      <field name="model" search="[('model', '=', 'account.fiscalyear.invoice_sequence')]"/>
+      <field name="model">account.fiscalyear.invoice_sequence</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_invoice_sequence_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.fiscalyear.invoice_sequence')]"/>
+      <field name="model">account.fiscalyear.invoice_sequence</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_invoice_sequence_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_invoice_sequence_companies"/>
     </record>
   </data>
```

### Comparing `trytond_account_invoice-7.0.4/company.py` & `trytond_account_invoice-7.2.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/doc/conf.py` & `trytond_account_invoice-7.2.0/doc/conf.py`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_invoice-7.0.4/doc/configuration.rst` & `trytond_account_invoice-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/doc/design.rst` & `trytond_account_invoice-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/doc/usage/amend.rst` & `trytond_account_invoice-7.2.0/doc/usage/amend.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/doc/usage/prepare.rst` & `trytond_account_invoice-7.2.0/doc/usage/prepare.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/doc/usage/process.rst` & `trytond_account_invoice-7.2.0/doc/usage/process.inc.rst`

 * *Files 3% similar despite different names*

```diff
@@ -81,18 +81,19 @@
 Paying an invoice
 =================
 
 Each `Invoice <model-account.invoice>` tracks how much still needs to be paid.
 Once an invoice has been fully paid it automatically updates its state to
 indicate that it is now paid.
 
-If you are manually registering payments against invoices, then you can use
-the invoice's :guilabel:`Pay` button to run the
-`Pay Invoice <wizard-account.invoice.pay>` wizard and register a cash payment
-against the invoice.
+If you are manually registering payments against invoices, you must configure
+at least one `Payment Method <model-account.invoice.payment.method>` then you
+can use the invoice's :guilabel:`Pay` button to run the `Pay Invoice
+<wizard-account.invoice.pay>` wizard and register a cash payment against the
+invoice.
 
 When doing this you will need to have already setup an appropriate
 `Invoice Payment Method <model-account.invoice.payment.method>`.
 This then makes it easy to use consistent
 `Journals <account:model-account.journal>` and
 `Accounts <account:model-account.account>` when manually entering payments.
```

### Comparing `trytond_account_invoice-7.0.4/exceptions.py` & `trytond_account_invoice-7.2.0/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,13 +37,17 @@
     pass
 
 
 class InvoiceFutureWarning(UserWarning):
     pass
 
 
+class InvoiceTaxesWarning(UserWarning):
+    pass
+
+
 class InvoiceSimilarWarning(UserWarning):
     pass
 
 
 class CancelInvoiceMoveWarning(UserWarning):
     pass
```

### Comparing `trytond_account_invoice-7.0.4/icons/LICENSE` & `trytond_account_invoice-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/invoice.fodt` & `trytond_account_invoice-7.2.0/invoice.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_account_invoice-7.0.4/invoice.fodt` & `trytond_account_invoice-7.2.0/invoice.fodt`

```diff
@@ -718,15 +718,15 @@
   <office:master-styles>
     <style:master-page style:name="Standard" style:page-layout-name="pm1" draw:style-name="dp1">
       <style:header>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;invoice.company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in invoice.company.header.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in invoice.company.header_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -738,15 +738,15 @@
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;invoice.company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in invoice.company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in invoice.company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -923,18 +923,18 @@
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A5" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
-              <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.product&quot;&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.product_name&quot;&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="Table_20_Contents">
-              <text:placeholder text:placeholder-type="text">&lt;line.product.rec_name&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;line.product_name&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="Table_20_Contents">
               <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.description&quot;&gt;</text:placeholder>
             </text:p>
```

### Comparing `trytond_account_invoice-7.0.4/invoice.py` & `trytond_account_invoice-7.2.0/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,32 +15,34 @@
 from trytond import backend
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, Unique, Workflow, dualmethod,
     fields, sequence_ordered)
 from trytond.model.exceptions import AccessError
+from trytond.modules.account.exceptions import AccountMissing
 from trytond.modules.account.tax import TaxableMixin
 from trytond.modules.company.model import (
     employee_field, reset_employee, set_employee)
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, Id, If
 from trytond.report import Report
 from trytond.rpc import RPC
-from trytond.tools import firstline, grouped_slice, reduce_ids, slugify
+from trytond.tools import (
+    cached_property, firstline, grouped_slice, reduce_ids, slugify)
 from trytond.transaction import Transaction
 from trytond.wizard import (
     Button, StateAction, StateReport, StateTransition, StateView, Wizard)
 
 from .exceptions import (
     InvoiceFutureWarning, InvoiceNumberError, InvoicePaymentTermDateWarning,
-    InvoiceSimilarWarning, InvoiceTaxValidationError, InvoiceValidationError,
-    PayInvoiceError)
+    InvoiceSimilarWarning, InvoiceTaxesWarning, InvoiceTaxValidationError,
+    InvoiceValidationError, PayInvoiceError)
 
 if config.getboolean('account_invoice', 'filestore', default=False):
     file_id = 'invoice_report_cache_id'
     store_prefix = config.get('account_invoice', 'store_prefix', default=None)
 else:
     file_id = None
     store_prefix = None
@@ -69,20 +71,24 @@
     company = fields.Many2One(
         'company.company', "Company", required=True,
         states={
             'readonly': (
                 _states['readonly']
                 | Eval('party', True)
                 | Eval('lines', [0])),
+            },
+        context={
+            'party_contact_mechanism_usage': 'invoice',
             })
     company_party = fields.Function(
         fields.Many2One(
             'party.party', "Company Party",
             context={
                 'company': Eval('company', -1),
+                'party_contact_mechanism_usage': 'invoice',
                 },
             depends={'company'}),
         'on_change_with_company_party')
     tax_identifier = fields.Many2One(
         'party.identifier', "Tax Identifier", ondelete='RESTRICT',
         states=_states)
     type = fields.Selection([
@@ -138,14 +144,15 @@
         help="The date from which the payment term is calculated.\n"
         "Leave empty to use the invoice date.")
     sequence = fields.Integer("Sequence", readonly=True)
     party = fields.Many2One(
         'party.party', 'Party', required=True, states=_states,
         context={
             'company': Eval('company', -1),
+            'party_contact_mechanism_usage': 'invoice',
             },
         depends={'company'})
     party_tax_identifier = fields.Many2One(
         'party.identifier', "Party Tax Identifier", ondelete='RESTRICT',
         states=_states)
     party_lang = fields.Function(fields.Char('Party Language'),
         'on_change_with_party_lang')
@@ -485,15 +492,17 @@
 
         # Migration from 6.6: drop not null on journal
         table.not_null_action('journal', 'remove')
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @staticmethod
     def default_type():
         return Transaction().context.get('type', 'out')
 
     @staticmethod
     def default_state():
@@ -506,14 +515,25 @@
             company = Company(Transaction().context['company'])
             return company.currency.id
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
+    @fields.depends(
+        'company', 'tax_identifier', methods=['on_change_with_company_party'])
+    def on_change_company(self):
+        company_party = self.on_change_with_company_party()
+        if self.company:
+            if self.tax_identifier:
+                if self.tax_identifier.party != company_party:
+                    self.tax_identifier = None
+        else:
+            self.tax_identifier = None
+
     @fields.depends('company')
     def on_change_with_company_party(self, name=None):
         return self.company.party if self.company else None
 
     @fields.depends(methods=['set_journal', 'on_change_party'])
     def on_change_type(self):
         self.set_journal()
@@ -540,27 +560,28 @@
     @classmethod
     def order_accounting_date(cls, tables):
         table, _ = tables[None]
         return [Coalesce(table.accounting_date, table.invoice_date)]
 
     @fields.depends('party', 'type', methods=['_update_account'])
     def on_change_party(self):
-        self.invoice_address = None
         if self.party:
             self.invoice_address = self.party.address_get(type='invoice')
             self.party_tax_identifier = self.party.tax_identifier
             if self.type == 'out':
                 self.account = self.party.account_receivable_used
                 self.payment_term = self.party.customer_payment_term
             elif self.type == 'in':
                 self.account = self.party.account_payable_used
                 self.payment_term = self.party.supplier_payment_term
         else:
-            self.payment_term = None
+            self.invoice_address = None
             self.account = None
+            self.payment_term = None
+            self.party_tax_identifier = None
         self._update_account()
 
     @fields.depends(methods=['_update_account'])
     def on_change_accounting_date(self):
         self._update_account()
 
     @fields.depends(methods=['_update_account'])
@@ -799,15 +820,15 @@
 
     @classmethod
     def get_amount_to_pay(cls, invoices, name):
         pool = Pool()
         Currency = pool.get('currency.currency')
         Date = pool.get('ir.date')
 
-        res = dict((x.id, Decimal(0)) for x in invoices)
+        amounts = defaultdict(Decimal)
         for company, grouped_invoices in groupby(
                 invoices, key=lambda i: i.company):
             with Transaction().set_context(company=company.id):
                 today = Date.today()
             for invoice in grouped_invoices:
                 if invoice.state != 'posted':
                     continue
@@ -829,22 +850,22 @@
                     if line.reconciliation:
                         continue
                     if (line.second_currency
                             and line.second_currency == invoice.currency):
                         amount_currency += line.amount_second_currency
                     else:
                         amount += line.debit - line.credit
-                if amount != Decimal(0):
+                if amount:
                     with Transaction().set_context(date=invoice.currency_date):
                         amount_currency += Currency.compute(
                             invoice.company.currency, amount, invoice.currency)
                 if invoice.type == 'in' and amount_currency:
                     amount_currency *= -1
-                res[invoice.id] = amount_currency
-        return res
+                amounts[invoice.id] = amount_currency
+        return amounts
 
     @classmethod
     def search_total_amount(cls, name, clause):
         pool = Pool()
         Rule = pool.get('ir.rule')
         Line = pool.get('account.invoice.line')
         Tax = pool.get('account.invoice.tax')
@@ -1077,39 +1098,76 @@
         Return move line
         '''
         pool = Pool()
         Currency = pool.get('currency.currency')
         MoveLine = pool.get('account.move.line')
         line = MoveLine()
         if self.currency != self.company.currency:
-            with Transaction().set_context(date=self.currency_date):
-                line.amount_second_currency = Currency.compute(
-                    self.company.currency, amount, self.currency)
+            line.amount_second_currency = amount
             line.second_currency = self.currency
+            with Transaction().set_context(date=self.currency_date):
+                amount = Currency.compute(
+                    self.currency, amount, self.company.currency)
         else:
             line.amount_second_currency = None
             line.second_currency = None
-        if amount <= 0:
-            line.debit, line.credit = -amount, 0
+        if amount >= 0:
+            if self.type == 'out':
+                line.debit, line.credit = amount, 0
+            else:
+                line.debit, line.credit = 0, amount
         else:
-            line.debit, line.credit = 0, amount
+            if self.type == 'out':
+                line.debit, line.credit = 0, -amount
+            else:
+                line.debit, line.credit = -amount, 0
         if line.amount_second_currency:
             line.amount_second_currency = (
                 line.amount_second_currency.copy_sign(
                     line.debit - line.credit))
         line.account = self.account
         if self.account.party_required:
             if self.alternative_payees:
                 line.party, = self.alternative_payees
             else:
                 line.party = self.party
         line.maturity_date = date
         line.description = self.description
         return line
 
+    def _get_exchange_move_line(self, amount):
+        pool = Pool()
+        Configuration = pool.get('account.configuration')
+        MoveLine = pool.get('account.move.line')
+        configuration = Configuration(1)
+        line = MoveLine()
+        line.debit = -amount if amount < 0 else 0
+        line.credit = amount if amount > 0 else 0
+        if line.credit:
+            line.account = configuration.get_multivalue(
+                'currency_exchange_credit_account', company=self.company.id)
+            if not line.account:
+                raise AccountMissing(gettext(
+                        'account_invoice.'
+                        'msg_invoice_currency_exchange_credit_account_missing',
+                        invoice=self.rec_name,
+                        company=self.company.rec_name))
+        else:
+            line.account = configuration.get_multivalue(
+                'currency_exchange_debit_account', company=self.company.id)
+            if not line.account:
+                raise AccountMissing(gettext(
+                        'account_invoice.'
+                        'msg_invoice_currency_exchange_debit_account_missing',
+                        invoice=self.rec_name,
+                        company=self.company.rec_name))
+        line.amount_second_currency = None
+        line.second_currency = None
+        return line
+
     def get_move(self):
         '''
         Compute account move for the invoice and return the created move
         '''
         pool = Pool()
         Move = pool.get('account.move')
         Period = pool.get('account.period')
@@ -1124,45 +1182,40 @@
         self.update_taxes(exception=True)
         move_lines = []
         for line in self.lines:
             move_lines += line.get_move_lines()
         for tax in self.taxes:
             move_lines += tax.get_move_lines()
 
-        total = sum(l.debit - l.credit for l in move_lines)
+        remainder = sum(l.debit - l.credit for l in move_lines)
         if self.payment_term:
             payment_date = self.payment_term_date or self.invoice_date or today
             term_lines = self.payment_term.compute(
-                total, self.company.currency, payment_date)
+                self.total_amount, self.currency, payment_date)
         else:
-            term_lines = [(self.payment_term_date or today, total)]
-        if self.currency != self.company.currency:
-            remainder_total_currency = self.total_amount.copy_sign(total)
-        else:
-            remainder_total_currency = 0
+            term_lines = [(self.payment_term_date or today, self.total_amount)]
         past_payment_term_dates = []
         for date, amount in term_lines:
             line = self._get_move_line(date, amount)
-            if line.amount_second_currency:
-                remainder_total_currency += line.amount_second_currency
             move_lines.append(line)
+            remainder += line.debit - line.credit
             if self.type == 'out' and date < today:
                 past_payment_term_dates.append(date)
+        if self.currency != self.company.currency and remainder:
+            line = self._get_exchange_move_line(remainder)
+            move_lines.append(line)
         if any(past_payment_term_dates):
             lang = Lang.get()
             warning_key = Warning.format('invoice_payment_term', [self])
             if Warning.check(warning_key):
                 raise InvoicePaymentTermDateWarning(warning_key,
                     gettext('account_invoice'
                         '.msg_invoice_payment_term_date_past',
                         invoice=self.rec_name,
                         date=lang.strftime(min(past_payment_term_dates))))
-        if not self.currency.is_zero(remainder_total_currency):
-            move_lines[-1].amount_second_currency -= \
-                remainder_total_currency
 
         accounting_date = self.accounting_date or self.invoice_date or today
         period = Period.find(self.company, date=accounting_date)
 
         move = Move()
         move.journal = self.journal
         move.period = period
@@ -1720,18 +1773,20 @@
     @ModelView.button
     @Workflow.transition('validated')
     @set_employee('validated_by')
     def validate_invoice(cls, invoices):
         pool = Pool()
         Move = pool.get('account.move')
 
+        cls._check_taxes(invoices)
+        cls._check_similar(invoices)
+
         invoices_in = cls.browse([i for i in invoices if i.type == 'in'])
         cls.set_number(invoices_in)
         cls._store_cache(invoices)
-        cls._check_similar(invoices)
         moves = []
         for invoice in invoices_in:
             move = invoice.get_move()
             if move != invoice.move:
                 invoice.move = move
                 moves.append(move)
         if moves:
@@ -1781,15 +1836,17 @@
                     names += '...'
                 warning_key = Warning.format(
                     'invoice_date_future', future_invoices)
                 if Warning.check(warning_key):
                     raise InvoiceFutureWarning(warning_key,
                         gettext('account_invoice.msg_invoice_date_future',
                             invoices=names))
-        cls._check_similar([i for i in invoices if i.state != 'validated'])
+        to_check = [i for i in invoices if i.state != 'validated']
+        cls._check_taxes(to_check)
+        cls._check_similar(to_check)
         cls._post(invoices)
 
     @classmethod
     def _post(cls, invoices):
         pool = Pool()
         Move = pool.get('account.move')
         transaction = Transaction()
@@ -1820,14 +1877,40 @@
             cls.__queue__.print_invoice(to_print)
         if reconciled:
             with transaction.set_context(
                     queue_batch=context.get('queue_batch', True)):
                 cls.__queue__.process(reconciled)
 
     @classmethod
+    def _check_taxes(cls, invoices):
+        pool = Pool()
+        Line = pool.get('account.invoice.line')
+        Warning = pool.get('res.user.warning')
+        for invoice in invoices:
+            different_lines = []
+            for line in invoice.lines:
+                test_line = Line(line.id)
+                test_line.on_change_product()
+                if (set(test_line.taxes) != set(line.taxes)
+                        or test_line.taxes_deductible_rate
+                        != line.taxes_deductible_rate):
+                    different_lines.append(line)
+            if different_lines:
+                warning_key = Warning.format(
+                    'invoice_taxes', [invoice])
+                if Warning.check(warning_key):
+                    lines = ', '.join(l.rec_name for l in different_lines[:5])
+                    if len(different_lines) > 5:
+                        lines += '...'
+                    raise InvoiceTaxesWarning(warning_key,
+                        gettext('account_invoice.msg_invoice_default_taxes',
+                            invoice=invoice.rec_name,
+                            lines=lines))
+
+    @classmethod
     def _check_similar(cls, invoices, type='in'):
         pool = Pool()
         Warning = pool.get('res.user.warning')
         for sub_invoices in grouped_slice(invoices):
             sub_invoices = list(sub_invoices)
             domain = list(filter(None,
                         (i._similar_domain() for i in sub_invoices
@@ -2083,14 +2166,15 @@
             'readonly': _states['readonly'] & Bool(Eval('invoice')),
             })
     invoice_party = fields.Function(
         fields.Many2One(
             'party.party', "Party",
             context={
                 'company': Eval('company', -1),
+                'party_contact_mechanism_usage': 'invoice',
                 },
             depends=['company']),
         'on_change_with_invoice_party', searcher='search_invoice_party')
     invoice_description = fields.Function(
         fields.Char("Invoice Description"),
         'on_change_with_invoice_description',
         searcher='search_invoice_description')
@@ -2107,24 +2191,28 @@
         'party.party', "Party",
         states={
             'required': ~Eval('invoice'),
             'readonly': _states['readonly'],
             },
         context={
             'company': Eval('company', -1),
+            'party_contact_mechanism_usage': 'invoice',
             },
         depends={'company'})
     party_lang = fields.Function(fields.Char('Party Language'),
         'on_change_with_party_lang')
     currency = fields.Many2One(
         'currency.currency', "Currency", required=True,
         states=_states)
     company = fields.Many2One(
         'company.company', "Company", required=True,
-        states=_states)
+        states=_states,
+        context={
+            'party_contact_mechanism_usage': 'invoice',
+            })
     type = fields.Selection([
         ('line', 'Line'),
         ('subtotal', 'Subtotal'),
         ('title', 'Title'),
         ('comment', 'Comment'),
         ], "Type", required=True,
         states={
@@ -2513,15 +2601,16 @@
             date = self.invoice.accounting_date or self.invoice.invoice_date
         else:
             date = None
         return {
             'date': date,
             }
 
-    @fields.depends('product', 'unit', '_parent_invoice.type',
+    @fields.depends(
+        'product', 'unit', 'taxes', '_parent_invoice.type',
         '_parent_invoice.party', 'party', 'invoice', 'invoice_type',
         '_parent_invoice.invoice_date', '_parent_invoice.accounting_date',
         'company',
         methods=['_get_tax_rule_pattern'])
     def on_change_product(self):
         if not self.product:
             return
@@ -2579,19 +2668,24 @@
                     taxes.update(tax_ids)
             self.taxes = taxes
 
         category = self.product.default_uom.category
         if not self.unit or self.unit.category != category:
             self.unit = self.product.default_uom.id
 
+    @cached_property
+    def product_name(self):
+        return self.product.rec_name if self.product else ''
+
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
         return self.product.default_uom_category if self.product else None
 
-    @fields.depends('account', 'product', 'invoice',
+    @fields.depends(
+        'account', 'product', 'invoice', 'taxes',
         '_parent_invoice.party', '_parent_invoice.type',
         'party', 'invoice', 'invoice_type',
         methods=['_get_tax_rule_pattern'])
     def on_change_account(self):
         if self.product:
             return
         taxes = set()
@@ -2806,15 +2900,14 @@
         line.taxes = self.taxes
         return line
 
 
 class InvoiceLineTax(ModelSQL):
     'Invoice Line - Tax'
     __name__ = 'account.invoice.line-account.tax'
-    _table = 'account_invoice_line_account_tax'
     line = fields.Many2One(
         'account.invoice.line', "Invoice Line",
         ondelete='CASCADE', required=True)
     tax = fields.Many2One('account.tax', 'Tax', ondelete='RESTRICT',
             required=True)
 
     @classmethod
@@ -2822,14 +2915,21 @@
         super().__setup__()
         t = cls.__table__()
         cls._sql_constraints += [
             ('line_tax_unique', Unique(t, t.line, t.tax),
                 'account_invoice.msg_invoice_line_tax_unique'),
             ]
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'account_invoice_line_account_tax', cls._table)
+        super().__register__(module)
+
 
 class InvoiceTax(sequence_ordered(), ModelSQL, ModelView):
     'Invoice Tax'
     __name__ = 'account.invoice.tax'
     _rec_name = 'description'
     _states = {
         'readonly': Eval('invoice_state') != 'draft',
@@ -3403,21 +3503,24 @@
             amount *= -1
         return invoice.get_reconcile_lines_for_amount(
             amount, currency, party=self.start.payee)
 
     def default_start(self, fields):
         default = {}
         invoice = self.record
+        payee = None
         if not invoice.alternative_payees:
-            default['payee'] = invoice.party.id
+            payee = invoice.party
         else:
             try:
-                default['payee'], = invoice.alternative_payees
+                payee, = invoice.alternative_payees
             except ValueError:
                 pass
+        if payee:
+            default['payee'] = payee.id
         default['payees'] = (
             [invoice.party.id] + [p.id for p in invoice.alternative_payees])
         default['company'] = invoice.company.id
         default['currency'] = invoice.currency.id
         default['amount'] = (invoice.amount_to_pay_today
             or invoice.amount_to_pay)
         default['invoice_account'] = invoice.account.id
```

### Comparing `trytond_account_invoice-7.0.4/invoice.xml` & `trytond_account_invoice-7.2.0/invoice.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account_invoice-7.0.4/invoice.xml` & `trytond_account_invoice-7.2.0/invoice.xml`

```diff
@@ -160,71 +160,71 @@
     </record>
     <record model="ir.action.keyword" id="act_invoice_relate_keyword_party">
       <field name="keyword">form_relate</field>
       <field name="model">party.party,-1</field>
       <field name="action" ref="act_invoice_relate"/>
     </record>
     <record model="ir.model.access" id="access_invoice">
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
+      <field name="model">account.invoice</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_account">
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
+      <field name="model">account.invoice</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="invoice_cancel_button">
+      <field name="model">account.invoice</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
       <field name="confirm">Are you sure you want to cancel the invoices?</field>
       <field name="help">Cancel the invoice</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_draft_button">
+      <field name="model">account.invoice</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_validate_button">
+      <field name="model">account.invoice</field>
       <field name="name">validate_invoice</field>
       <field name="string">Validate</field>
       <field name="help">Also known as Pro Forma</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_post_button">
+      <field name="model">account.invoice</field>
       <field name="name">post</field>
       <field name="string">Post</field>
       <field name="confirm">Are you sure you want to post the invoices?</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_pay_button">
+      <field name="model">account.invoice</field>
       <field name="name">pay</field>
       <field name="string">Pay</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_reschedule_lines_to_pay_button">
+      <field name="model">account.invoice</field>
       <field name="name">reschedule_lines_to_pay</field>
       <field name="string">Reschedule</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_delegate_lines_to_pay_button">
+      <field name="model">account.invoice</field>
       <field name="name">delegate_lines_to_pay</field>
       <field name="string">Modify Payee</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button" id="invoice_process_button">
+      <field name="model">account.invoice</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
     </record>
     <record model="ir.model.button-res.group" id="invoice_process_button_group_account_admin">
       <field name="button" ref="invoice_process_button"/>
       <field name="group" ref="account.group_account_admin"/>
     </record>
     <record model="ir.action.wizard" id="refresh_invoice_report_wizard">
       <field name="name">Invoice (revised)</field>
@@ -247,15 +247,15 @@
     </record>
     <record model="ir.ui.view" id="invoice_report_revision_view_form">
       <field name="model">account.invoice.report.revision</field>
       <field name="type">form</field>
       <field name="name">invoice_report_revision_form</field>
     </record>
     <record model="ir.model.access" id="access_invoice_report_revision">
-      <field name="model" search="[('model', '=', 'account.invoice.report.revision')]"/>
+      <field name="model">account.invoice.report.revision</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.report" id="report_invoice">
       <field name="name">Invoice</field>
@@ -294,22 +294,22 @@
     <record model="ir.ui.view" id="invoice_line_view_tree_sequence">
       <field name="model">account.invoice.line</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">invoice_line_tree_sequence</field>
     </record>
     <record model="ir.model.access" id="access_invoice_line">
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
+      <field name="model">account.invoice.line</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_line_account">
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
+      <field name="model">account.invoice.line</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="invoice_tax_view_form">
@@ -362,30 +362,30 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="payment_method_view_form"/>
       <field name="act_window" ref="act_payment_method_form"/>
     </record>
     <menuitem parent="account.menu_journal_configuration" action="act_payment_method_form" sequence="50" id="menu_payment_method_form"/>
     <record model="ir.rule.group" id="rule_group_payment_method_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.invoice.payment.method')]"/>
+      <field name="model">account.invoice.payment.method</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_method_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_payment_method_companies"/>
     </record>
     <record model="ir.model.access" id="access_payment_method">
-      <field name="model" search="[('model', '=', 'account.invoice.payment.method')]"/>
+      <field name="model">account.invoice.payment.method</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_method_account_admin">
-      <field name="model" search="[('model', '=', 'account.invoice.payment.method')]"/>
+      <field name="model">account.invoice.payment.method</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="credit_start_view_form">
@@ -401,24 +401,24 @@
     <record model="ir.action.keyword" id="credit_keyword">
       <field name="keyword">form_action</field>
       <field name="model">account.invoice,-1</field>
       <field name="action" ref="credit"/>
     </record>
     <record model="ir.rule.group" id="rule_group_invoice_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
+      <field name="model">account.invoice</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_invoice_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_invoice_companies"/>
     </record>
     <record model="ir.rule.group" id="rule_group_invoice_line_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
+      <field name="model">account.invoice.line</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_invoice_line_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_invoice_line_companies"/>
     </record>
     <record model="ir.action.wizard" id="act_reschedule_lines_to_pay_wizard">
```

### Comparing `trytond_account_invoice-7.0.4/locale/bg.po` & `trytond_account_invoice-7.2.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -1029,14 +1029,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1436,14 +1450,18 @@
 msgid "General"
 msgstr "Основен"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Бележки"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 #, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.0.4/locale/ca.po` & `trytond_account_invoice-7.2.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -953,14 +953,34 @@
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "No podeu abonar la factura rectificativa \"%(invoice)s\" perquè no està "
 "comptabilitzada."
 
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Per poder comptabilitzar la factura \"%(invoice)s\" heu de definir una "
+"seqüència per l'exercici fical \"%(fiscalyear)s\"."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Per poder comptabilitzar la factura \"%(invoice)s\" heu de definir una "
+"seqüència per l'exercici fical \"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "No podeu cancel·lar la factura de client \"%(invoice)s\" perquè està "
 "comptabilitzada i la configuració de l'empresa no ho permet."
@@ -1375,14 +1395,18 @@
 msgid "General"
 msgstr "General"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notes"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr "Hora"
```

### Comparing `trytond_account_invoice-7.0.4/locale/cs.po` & `trytond_account_invoice-7.2.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -983,14 +983,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1384,14 +1398,18 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 #, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.0.4/locale/de.po` & `trytond_account_invoice-7.2.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -957,14 +957,34 @@
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "Rechnung \"%(invoice)s\" kann nicht verrechnet werden, da sie noch nicht "
 "festgeschrieben wurde."
 
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Um Rechnung invoice \"%(invoice)s\" festschreiben zu können, muss ein "
+"Nummernkreis für das Geschäftsjahr \"%(fiscalyear)s\" definiert sein."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Um Rechnung invoice \"%(invoice)s\" festschreiben zu können, muss ein "
+"Nummernkreis für das Geschäftsjahr \"%(fiscalyear)s\" definiert sein."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Rechnung \"%(invoice)s\" kann nicht annulliert werden, da sie "
 "festgeschrieben ist und das Annullieren für das Unternehmen nicht zulässig "
@@ -1074,15 +1094,15 @@
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "Die Rechnung \"%(invoice)s\" produziert ein Zahlungsdatum \"%(date)s\" in "
 "der Vergangenheit."
 
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
-msgstr "Die Rechnungen \"%(invoices)s\" ist ähnlich zu Rechnung \"%(similar)s\"."
+msgstr "Die Rechnung \"%(invoice)s\" ist ähnlich zu Rechnung \"%(similar)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
 "You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
 " draft state."
 msgstr ""
 "Zu Rechnung \"%(invoice)s\" kann keine Steuer hinzugefügt werden, da sie "
@@ -1389,14 +1409,18 @@
 msgid "General"
 msgstr "Allgemein"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notizen"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr "Uhrzeit"
```

### Comparing `trytond_account_invoice-7.0.4/locale/es.po` & `trytond_account_invoice-7.2.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -951,14 +951,34 @@
 "No puede eliminar el tercero \"%(party)s\" mientras tenga facturas "
 "pendientes con la companía \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr "No puede abonar la factura \"%(invoice)s\" porque no está contabilizada."
 
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Para contabilizar la factura \"%(invoice)s\", debe definir una secuencia "
+"para el ejercicio fiscal \"%(fiscalyear)s\"."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Para contabilizar la factura \"%(invoice)s\", debe definir una secuencia "
+"para el ejercicio fiscal \"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "No puede cancelar la factura de cliente \"%(invoice)s\" porque está "
 "contabilizada y la configuración de la empresa no lo permite."
@@ -1374,14 +1394,18 @@
 msgid "General"
 msgstr "General"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notas"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr "Hora"
```

### Comparing `trytond_account_invoice-7.0.4/locale/es_419.po` & `trytond_account_invoice-7.2.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -967,14 +967,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "No puede agregar el impuesto a la factura \"%(invoice)s\" porque está "
@@ -1379,14 +1393,18 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/et.po` & `trytond_account_invoice-7.2.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -984,14 +984,34 @@
 "\"%(ettevõte)tega\" avatud arveid"
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr "Arvet \"%(arve)id\" ei saa hüvitada, kuna see on postitamata."
 
 #, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Arve \"%(arve)te\" postitamiseks tuleb määrata majandusaasta "
+"\"%(majandusaasta)te\" jada."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Arve \"%(arve)te\" postitamiseks tuleb määrata majandusaasta "
+"\"%(majandusaasta)te\" jada."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr "Kliendiarvet \"%(arve)id\" ei saa tühistada, kuna need on postitatud."
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1408,14 +1428,18 @@
 msgid "General"
 msgstr "Peamine"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Märtkused"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/fa.po` & `trytond_account_invoice-7.2.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -988,14 +988,34 @@
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "شما نمی توانید صورتحساب : \"%(invoice)s\" را بازپرداخت شده کنید، چرا که "
 "ارسال نشده است."
 
 #, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"برای ارسال صورتحساب : \"%(invoice)s\"،شما باید یک دنباله در سال مالی : "
+"\"%(fiscalyear)s\" تعریف کنید."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"برای ارسال صورتحساب : \"%(invoice)s\"،شما باید یک دنباله در سال مالی : "
+"\"%(fiscalyear)s\" تعریف کنید."
+
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "شما نمیتوانید صورتحساب مشتری : \"%(invoice)s\" را لغو کنید، چراکه آن ارسال "
 "شده است."
@@ -1416,14 +1436,18 @@
 msgid "General"
 msgstr "عمومی"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "یادداشت ها"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/fi.po` & `trytond_account_invoice-7.2.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -980,14 +980,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1204,15 +1218,14 @@
 msgstr "Payment Terms"
 
 #, fuzzy
 msgctxt "model:party.party.payment_term,name:"
 msgid "Party Payment Term"
 msgstr "Test Payment Term"
 
-#, fuzzy
 msgctxt "report:account.invoice:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:account.invoice:"
 msgid "Amount"
 msgstr ""
@@ -1381,15 +1394,18 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
-#, fuzzy
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/fr.po` & `trytond_account_invoice-7.2.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -955,14 +955,32 @@
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "Vous ne pouvez pas rembourser la facture « %(invoice)s » car elle n'est pas "
 "comptabilisée."
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Pour comptabiliser la facture « %(invoice)s », vous devez définir un compte "
+"de crédit de change de devis pour « %(company)s »."
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Pour comptabiliser la facture « %(invoice)s », vous devez définir une compte"
+" de débit de change de devise pour « %(company)s »."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Vous ne pouvez pas annuler la facture client « %(invoice)s » car elle est "
 "comptabilisée et la configuration de la société ne le permet pas."
@@ -1382,14 +1400,18 @@
 msgid "General"
 msgstr "Général"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notes"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr "Les opérations sont appliquées dans cet ordre affiché."
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr "Heure"
```

### Comparing `trytond_account_invoice-7.0.4/locale/hu.po` & `trytond_account_invoice-7.2.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -975,14 +975,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1374,14 +1388,18 @@
 msgid "General"
 msgstr "Általános"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Jegyzetek"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/id.po` & `trytond_account_invoice-7.2.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -970,14 +970,28 @@
 "Anda tidak dapat menghapus pihak \"%(party)s\" selagi mereka memiliki faktur"
 " yang tertunda dengan perusahaan \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Anda tidak dapat membatalkan faktur \"%(invoice)s\" karena dibukukan dan "
 "pengaturan perusahaan tidak mengizinkannya."
@@ -1377,14 +1391,18 @@
 msgid "General"
 msgstr "Umum"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Catatan-Catatan"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/it.po` & `trytond_account_invoice-7.2.0/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -994,14 +994,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Non puoi aggiungere/variare l'imposta nella fattura \"%(invoice)s\" perché è"
@@ -1411,14 +1425,18 @@
 msgid "General"
 msgstr "Generale"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Note"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/lo.po` & `trytond_account_invoice-7.2.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -1046,14 +1046,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1455,14 +1469,18 @@
 msgid "General"
 msgstr "ທົ່ວໄປ"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "ໝາຍເຫດ"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 #, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.0.4/locale/lt.po` & `trytond_account_invoice-7.2.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -981,14 +981,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1377,14 +1391,18 @@
 msgid "General"
 msgstr "Pagrindinis"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Pastabos"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/nl.po` & `trytond_account_invoice-7.2.0/locale/nl.po`

 * *Files 3% similar despite different names*

```diff
@@ -953,14 +953,32 @@
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 "U kunt de factuur \"%(invoice)s\" niet terugbetalen omdat ze niet geboekt "
 "is."
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Om factuur \"%(invoice)s\" te kunnen boeken, moet u een credit "
+"grootboekrekening voor de wisselkoers definiëren voor \"%(company)s\"."
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Om factuur \"%(invoice)s\" te kunnen boeken, moet u een debet "
+"grootboekrekening voor de wisselkoers definiëren voor \"%(company)s\"."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "U kunt klant factuur \"% (invoice)s\" niet annuleren omdat deze is geboekt "
 "en de bedrijfsinstellingen dit niet toelaten."
@@ -1378,14 +1396,18 @@
 msgid "General"
 msgstr "Algemeen"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notities"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr "Bewerkingen worden in de weergegeven volgorde uitgevoerd."
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr "Tijd"
```

### Comparing `trytond_account_invoice-7.0.4/locale/pl.po` & `trytond_account_invoice-7.2.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1000,14 +1000,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1406,14 +1420,18 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notatki"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/pt.po` & `trytond_account_invoice-7.2.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1007,14 +1007,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Você não pode adicionar a linha \"%(line)s\" à fatura \"%(invoice)s\" porque"
@@ -1424,14 +1438,18 @@
 msgid "General"
 msgstr "Geral"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Observações"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/ro.po` & `trytond_account_invoice-7.2.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 msgctxt "field:account.invoice,allow_cancel:"
 msgid "Allow Cancel Invoice"
 msgstr "Permis Anulare Factura"
 
 msgctxt "field:account.invoice,alternative_payees:"
 msgid "Alternative Payee"
-msgstr ""
+msgstr "Beneficiar Alternativ"
 
 msgctxt "field:account.invoice,amount_to_pay:"
 msgid "Amount to Pay"
 msgstr "Sumă de Plătit"
 
 msgctxt "field:account.invoice,amount_to_pay_today:"
 msgid "Amount to Pay Today"
@@ -99,22 +99,21 @@
 msgid "Currency Date"
 msgstr "Data Valută"
 
 msgctxt "field:account.invoice,description:"
 msgid "Description"
 msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.invoice,has_payment_method:"
 msgid "Has Payment Method"
-msgstr "Metodă Plata"
+msgstr "Are Metodă de Plată"
 
 msgctxt "field:account.invoice,has_report_cache:"
 msgid "Has Report Cached"
-msgstr ""
+msgstr "Are raport în cache"
 
 msgctxt "field:account.invoice,invoice_address:"
 msgid "Invoice Address"
 msgstr "Adresa de facturare"
 
 msgctxt "field:account.invoice,invoice_date:"
 msgid "Invoice Date"
@@ -128,18 +127,17 @@
 msgid "Invoice Report ID"
 msgstr "Raport Factura ID"
 
 msgctxt "field:account.invoice,invoice_report_format:"
 msgid "Invoice Report Format"
 msgstr "Format Raport Factura"
 
-#, fuzzy
 msgctxt "field:account.invoice,invoice_report_revisions:"
 msgid "Invoice Report Revisions"
-msgstr "Raport Factura"
+msgstr "Revizii Raport Factură"
 
 msgctxt "field:account.invoice,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "field:account.invoice,lines:"
 msgid "Lines"
@@ -181,18 +179,17 @@
 msgid "Payment Term"
 msgstr "Termen de plata"
 
 msgctxt "field:account.invoice,payment_term_date:"
 msgid "Payment Term Date"
 msgstr "Data Termen de Plata"
 
-#, fuzzy
 msgctxt "field:account.invoice,posted_by:"
 msgid "Posted By"
-msgstr "Postat"
+msgstr "Postat De"
 
 msgctxt "field:account.invoice,reconciled:"
 msgid "Reconciled"
 msgstr "Reconciliat"
 
 msgctxt "field:account.invoice,reconciliation_lines:"
 msgid "Payment Lines"
@@ -212,67 +209,63 @@
 
 msgctxt "field:account.invoice,tax_amount:"
 msgid "Tax"
 msgstr "Impozit"
 
 msgctxt "field:account.invoice,tax_amount_cache:"
 msgid "Tax Cache"
-msgstr ""
+msgstr "Cache Taxe"
 
 msgctxt "field:account.invoice,tax_identifier:"
 msgid "Tax Identifier"
 msgstr "Identificator fiscal"
 
 msgctxt "field:account.invoice,taxes:"
 msgid "Tax Lines"
 msgstr "Rânduri Impozit"
 
 msgctxt "field:account.invoice,total_amount:"
 msgid "Total"
 msgstr "Total"
 
-#, fuzzy
 msgctxt "field:account.invoice,total_amount_cache:"
 msgid "Total Cache"
-msgstr "Total"
+msgstr "Cache Total"
 
 msgctxt "field:account.invoice,type:"
 msgid "Type"
 msgstr "Tip"
 
 msgctxt "field:account.invoice,type_name:"
 msgid "Type"
 msgstr "Tip"
 
 msgctxt "field:account.invoice,untaxed_amount:"
 msgid "Untaxed"
 msgstr "Neimpozitat"
 
-#, fuzzy
 msgctxt "field:account.invoice,untaxed_amount_cache:"
 msgid "Untaxed Cache"
-msgstr "Neimpozitat"
+msgstr "Cache Neimpozitat"
 
-#, fuzzy
 msgctxt "field:account.invoice,validated_by:"
 msgid "Validated By"
-msgstr "Validat"
+msgstr "Validat de"
 
 msgctxt "field:account.invoice-account.move.line,invoice:"
 msgid "Invoice"
 msgstr "Factura fiscala"
 
 msgctxt "field:account.invoice-account.move.line,invoice_account:"
 msgid "Invoice Account"
 msgstr "Cont Facturare"
 
-#, fuzzy
 msgctxt "field:account.invoice-account.move.line,invoice_alternative_payees:"
 msgid "Invoice Alternative Payees"
-msgstr "Plata Facturi"
+msgstr "Plătitori Alternativi Factură"
 
 msgctxt "field:account.invoice-account.move.line,invoice_party:"
 msgid "Invoice Party"
 msgstr "Parte Facturata"
 
 msgctxt "field:account.invoice-account.move.line,line:"
 msgid "Payment Line"
@@ -282,22 +275,21 @@
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "field:account.invoice-additional-account.move,move:"
 msgid "Additional Move"
 msgstr "Mişcări Suplimentare"
 
-#, fuzzy
 msgctxt "field:account.invoice.alternative_payee,invoice:"
 msgid "Invoice"
-msgstr "Factura fiscala"
+msgstr "Factura"
 
 msgctxt "field:account.invoice.alternative_payee,party:"
 msgid "Payee"
-msgstr ""
+msgstr "Beneficiar"
 
 msgctxt "field:account.invoice.credit.start,invoice_date:"
 msgid "Invoice Date"
 msgstr "Data Factura"
 
 msgctxt "field:account.invoice.credit.start,with_refund:"
 msgid "With Refund"
@@ -327,20 +319,18 @@
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:account.invoice.line,invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,invoice_description:"
 msgid "Invoice Description"
-msgstr "Descriere"
+msgstr "Descrierea Facturii"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,invoice_party:"
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:account.invoice.line,invoice_state:"
 msgid "Invoice State"
 msgstr "Stare Factura"
@@ -369,15 +359,14 @@
 msgid "Party Language"
 msgstr "Limba Părții"
 
 msgctxt "field:account.invoice.line,product:"
 msgid "Product"
 msgstr "Produs"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr "Categorie UM Produs"
 
 msgctxt "field:account.invoice.line,quantity:"
 msgid "Quantity"
 msgstr "Cantitate"
@@ -426,15 +415,14 @@
 msgid "Write-Off Amount"
 msgstr "Sumă Prescriere"
 
 msgctxt "field:account.invoice.pay.ask,company:"
 msgid "Company"
 msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.invoice.pay.ask,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.invoice.pay.ask,invoice:"
 msgid "Invoice"
 msgstr "Factura"
@@ -481,19 +469,19 @@
 
 msgctxt "field:account.invoice.pay.start,invoice_account:"
 msgid "Invoice Account"
 msgstr "Cont Facturare"
 
 msgctxt "field:account.invoice.pay.start,payee:"
 msgid "Payee"
-msgstr ""
+msgstr "Beneficiar"
 
 msgctxt "field:account.invoice.pay.start,payees:"
 msgid "Payees"
-msgstr ""
+msgstr "Beneficiari"
 
 msgctxt "field:account.invoice.pay.start,payment_method:"
 msgid "Payment Method"
 msgstr "Metodă Plata"
 
 msgctxt "field:account.invoice.payment.method,company:"
 msgid "Company"
@@ -611,40 +599,34 @@
 msgid "Currency"
 msgstr "Valută"
 
 msgctxt "field:account.invoice.payment_term.test.result,date:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,date:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,filename:"
 msgid "File Name"
-msgstr "Denumire"
+msgstr "Denumire Fisier"
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,invoice:"
 msgid "Invoice"
-msgstr "Factura fiscala"
+msgstr "Factura"
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,invoice_report_cache:"
 msgid "Invoice Report"
 msgstr "Raport Factura"
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,invoice_report_cache_id:"
 msgid "Invoice Report ID"
-msgstr "Raport Factura ID"
+msgstr "ID Raport Factura"
 
-#, fuzzy
 msgctxt "field:account.invoice.report.revision,invoice_report_format:"
 msgid "Invoice Report Format"
 msgstr "Format Raport Factura"
 
 msgctxt "field:account.invoice.tax,account:"
 msgid "Account"
 msgstr "Cont"
@@ -747,15 +729,15 @@
 
 msgctxt "help:account.invoice.credit.start,with_refund:"
 msgid "If true, the current invoice(s) will be cancelled."
 msgstr "Daca este adevărat, factura curenta va fi anulata."
 
 msgctxt "help:account.invoice.line,product_uom_category:"
 msgid "The category of Unit of Measure for the product."
-msgstr ""
+msgstr "Categoria de Unitate de Masura pentru produs."
 
 msgctxt "help:account.invoice.line,taxes_date:"
 msgid ""
 "The date at which the taxes are computed.\n"
 "Leave empty for the accounting date."
 msgstr ""
 "Data la care se vor calcula impozitele.\n"
@@ -785,18 +767,17 @@
 msgid "Invoice - Payment Line"
 msgstr "Factura - Rând Plata"
 
 msgctxt "model:account.invoice-additional-account.move,name:"
 msgid "Invoice Additional Move"
 msgstr "Mişcare Suplimentara Factura"
 
-#, fuzzy
 msgctxt "model:account.invoice.alternative_payee,name:"
 msgid "Invoice Alternative Payee"
-msgstr "Stare Factura"
+msgstr "Plătitori Alternativi Factură"
 
 msgctxt "model:account.invoice.credit.start,name:"
 msgid "Credit Invoice"
 msgstr "Factura Storno"
 
 msgctxt "model:account.invoice.line,name:"
 msgid "Invoice Line"
@@ -834,41 +815,38 @@
 msgid "Test Payment Term"
 msgstr "Proba Termen de Plata"
 
 msgctxt "model:account.invoice.payment_term.test.result,name:"
 msgid "Test Payment Term"
 msgstr "Proba Termen de Plata"
 
-#, fuzzy
 msgctxt "model:account.invoice.report.revision,name:"
 msgid "Invoice Report Revision"
-msgstr "Raport Factura"
+msgstr "Revize Raport Factură"
 
 msgctxt "model:account.invoice.tax,name:"
 msgid "Invoice Tax"
 msgstr "Impozit Factura"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_delegate_lines_to_pay_wizard"
 msgid "Delegate Lines to Pay"
-msgstr "Reprogramare Rânduri de Plata"
+msgstr "Delegați Rânduri de Plată"
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
 msgstr "Facturi"
 
 msgctxt "model:ir.action,name:act_invoice_in_form"
 msgid "Supplier Invoices"
 msgstr "Facturi Furnizor"
 
 msgctxt "model:ir.action,name:act_invoice_out_form"
 msgid "Customer Invoices"
 msgstr "Facturi Client"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_invoice_relate"
 msgid "Invoices"
 msgstr "Facturi"
 
 msgctxt "model:ir.action,name:act_payment_method_form"
 msgid "Invoice Payment Methods"
 msgstr "Metode Plata Factura"
@@ -881,18 +859,17 @@
 msgid "Reschedule Lines to Pay"
 msgstr "Reprogramare Rânduri de Plata"
 
 msgctxt "model:ir.action,name:credit"
 msgid "Credit"
 msgstr "Credit"
 
-#, fuzzy
 msgctxt "model:ir.action,name:refresh_invoice_report_wizard"
 msgid "Invoice (revised)"
-msgstr "Rând Factura"
+msgstr "Factura (revizuita)"
 
 msgctxt "model:ir.action,name:report_invoice"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "model:ir.action,name:wizard_pay"
 msgid "Pay Invoice"
@@ -932,38 +909,37 @@
 msgstr "Postat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_invoice_out_domain_validated"
 msgid "Validated"
 msgstr "Validat"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_all"
 msgid "All"
 msgstr "Tot"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_paid"
 msgid "Paid"
 msgstr "Plătit"
 
 msgctxt "model:ir.action.act_window.domain,name:act_invoice_relate_pending"
 msgid "Pending"
-msgstr ""
+msgstr "In Derulare"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_cancel_invoice_move"
 msgid "The moves \"%(moves)s\" have the posted invoices \"%(invoices)s\" as origin."
-msgstr "Pentru a închide perioadele trebuie postate facturile \"%(invoices)s\"."
+msgstr "Mişcările \"%(moves)s\" au facturile \"%(invoices)s\" ca origine."
 
 msgctxt "model:ir.message,text:msg_cancel_invoice_move_description"
 msgid ""
 "Cancelling them will reconcile the move lines thus paying the invoices. You "
 "might want to cancel the invoices first."
 msgstr ""
+"Anularea va reconcilia rândurile mişcării, plătind astfel facturile. Poate "
+"doriți să anulați mai întâi facturile."
 
 msgctxt "model:ir.message,text:msg_close_period_non_posted_invoices"
 msgid "To close the periods you must post the invoices \"%(invoices)s\"."
 msgstr "Pentru a închide perioadele trebuie postate facturile \"%(invoices)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_invoice"
 msgid ""
@@ -973,14 +949,34 @@
 "Nu se poate şterge partea \"%(party)s\" când exista facturi nevalidate cu "
 "compania \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr "Nu se poate storna factura \"%(invoice)s\" pentru ca nu a fost postată."
 
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Pentru a posta \"%(invoice)s\" trebuie definita o secvenţa pe anul fiscal "
+"\"%(fiscalyear)s\"."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Pentru a posta \"%(invoice)s\" trebuie definita o secvenţa pe anul fiscal "
+"\"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Nu se poate anula factura de client \"%(invoice)s\" pentru că este postata "
 "şi configurarea companiei nu permite acest lucru."
@@ -993,22 +989,21 @@
 msgid "To delete invoice \"%(invoice)s\" you must cancel it."
 msgstr "Pentru a şterge factura \"%(invoice)s\" trebuie anulata."
 
 msgctxt "model:ir.message,text:msg_invoice_delete_numbered"
 msgid "You cannot delete invoice \"%(invoice)s\" because it has a number."
 msgstr "Nu se poate şterge factura \"%(invoice)s\" pentru că are un număr."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_line_create_draft"
 msgid ""
 "You cannot add lines to invoice \"%(invoice)s\" because it is no longer in a"
 " draft state."
 msgstr ""
-"Nu se poate adăuga un rând la factura \"%(invoice)s\" pentru că este "
-"postată, plătita sau anulată."
+"Nu se poate adăuga un rând la factura \"%(invoice)s\" pentru că nu mai este "
+"in starea de ciorna."
 
 msgctxt "model:ir.message,text:msg_invoice_line_modify"
 msgid ""
 "You cannot modify line \"%(line)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
 "Rândul \"%(line)s\" nu se poate modifica pentru ca factura \"%(invoice)s\" "
@@ -1036,28 +1031,33 @@
 
 msgctxt "model:ir.message,text:msg_invoice_number_after"
 msgid ""
 "To number the invoice \"%(invoice)s\", you must set an invoice date after "
 "\"%(date)s\" because the sequence \"%(sequence)s\" has already been used for"
 " invoice \"%(after_invoice)s\"."
 msgstr ""
+"Pentru a numerota factura \"%(invoice)s\", trebuie să setați o dată a "
+"facturii după \"%(date)s\", deoarece secvența \"%(sequence)s\" a fost deja "
+"utilizată pentru factura \"%(after_invoice)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_overpay_paid"
 msgid ""
 "You cannot overpay invoice \"%(invoice)s\" because there is no more left to "
 "pay."
 msgstr ""
 "Nu se poate supra-plati factura \"%(invoice)s\" pentru ca nu a ramas nimic "
 "de platit."
 
 msgctxt "model:ir.message,text:msg_invoice_pay_amount_greater_amount_to_pay"
 msgid ""
 "You cannot add a partial payment on invoice \"%(invoice)s\" with an amount "
 "greater than the amount to pay \"%(amount_to_pay)s\"."
 msgstr ""
+"Nu puteți adăuga o plată parțială pe factura %(invoice)s\" cu o sumă mai "
+"mare decât suma de plată \"%(amount_to_pay)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_line_unique"
 msgid "A payment line can be linked to only one invoice."
 msgstr "Un rând de plata poate fi legat de o singura factura."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_lines_add_remove_paid"
 msgid "You cannot add/remove payment lines on paid invoice \"%(invoice)s\"."
@@ -1066,62 +1066,70 @@
 "\"%(invoice)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_lines_greater_amount"
 msgid ""
 "Payment lines amount on invoice \"%(invoice)s\" can not be greater than the "
 "invoice amount."
 msgstr ""
+"Suma rândurilor de plată de pe factura \"%(invoice)s\" nu poate fi mai mare "
+"decât suma facturii."
 
 msgctxt "model:ir.message,text:msg_invoice_payment_term_date_past"
 msgid "The invoice \"%(invoice)s\" generates a payment date \"%(date)s\" in the past."
 msgstr ""
 "Factura \"%(invoice)s\" genereaza data \"%(date)s\" de plata care este in "
 "trecut."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_similar"
 msgid "The invoice \"%(invoice)s\" is similar to invoice \"%(similar)s\"."
-msgstr "Facturile \"%(invoices)s\" au o data în viitor."
+msgstr "Factura \"%(invoice)s\" este similară cu factura \"%(similar)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_tax_create"
 msgid ""
 "You cannot add taxes to invoice \"%(invoice)s\" because it is no longer in a"
 " draft state."
 msgstr ""
-"Nu se poate adăuga un rând la factura \"%(invoice)s\" pentru că este "
-"postată, plătita sau anulată."
+"Nu se poate adăuga un rând la factura \"%(invoice)s\" pentru că nu mai este "
+"in stare de ciornă."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_invalid"
 msgid ""
 "The taxes on invoice \"%(invoice)s\" are not valid, you must save it again "
 "to force them to be recalculated."
 msgstr ""
+"Taxele pe factura \"%(invoice)s\" nu sunt valabile, trebuie să o salvați din"
+" nou pentru a forța recalcularea acestora."
 
 msgctxt "model:ir.message,text:msg_invoice_tax_modify"
 msgid ""
 "You cannot modify tax \"%(tax)s\" because its invoice \"%(invoice)s\" is "
 "posted, paid or cancelled."
 msgstr ""
+"Nu se poate modifica impozit \"%(tax)s\" deoarece factura sa \"%(invoice)s\""
+" este postată, plătită sau anulată."
 
 msgctxt "model:ir.message,text:msg_payment_term_invalid_ratio_divisor"
 msgid "The ratio and divisor are not consistent on line \"%(line)s\"."
-msgstr ""
+msgstr "Raportul și divizorul nu sunt consecvente pe rândul \"%(line)s\"."
 
 msgctxt "model:ir.message,text:msg_payment_term_missing_last_remainder"
 msgid ""
 "To save payment term \"%(payment_term)s\", you must append a last remainder "
 "line."
 msgstr ""
+"Pentru a salva termenul de plată \"%(payment_term)s\", trebuie să atașați un"
+" ultim rând."
 
 msgctxt "model:ir.message,text:msg_payment_term_missing_remainder"
 msgid ""
 "To compute terms, you must append a remainder line on payment term "
 "\"%(payment_term)s\"."
 msgstr ""
+"Pentru a calcula termenii, trebuie să adăugați un rând la termenul de plată "
+"\"%(payment_term)s\"."
 
 msgctxt "model:ir.model.button,confirm:invoice_cancel_button"
 msgid "Are you sure you want to cancel the invoices?"
 msgstr "Sigur doriţi să anulaţi facturile?"
 
 msgctxt "model:ir.model.button,confirm:invoice_post_button"
 msgid "Are you sure you want to post the invoices?"
@@ -1137,15 +1145,15 @@
 
 msgctxt "model:ir.model.button,string:invoice_cancel_button"
 msgid "Cancel"
 msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:invoice_delegate_lines_to_pay_button"
 msgid "Modify Payee"
-msgstr ""
+msgstr "Modifica Beneficiar"
 
 msgctxt "model:ir.model.button,string:invoice_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:invoice_pay_button"
 msgid "Pay"
@@ -1383,21 +1391,25 @@
 msgid "General"
 msgstr "General"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Notițe"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
-msgstr ""
+msgstr "Timp"
 
 msgctxt "view:account.invoice:"
 msgid "Invoice"
 msgstr "Factura"
 
 msgctxt "view:account.invoice:"
 msgid "Other Info"
```

### Comparing `trytond_account_invoice-7.0.4/locale/ru.po` & `trytond_account_invoice-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -1030,14 +1030,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Вы не можете добавить строчку \"%(line)s\" в инвойс \"%(invoice)s\" так как "
@@ -1450,14 +1464,18 @@
 msgid "General"
 msgstr "Основной"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Комментарии"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 #, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
```

### Comparing `trytond_account_invoice-7.0.4/locale/sl.po` & `trytond_account_invoice-7.2.0/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -961,14 +961,34 @@
 "Ni mogoče izbrisati partnerja \"%(party)s\" dokler ima fakture v teku z "
 "družbo \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+"Za knjiženje fakture \"%(invoice)s\", je potrebno nastaviti šifrant na "
+"poslovnem letu \"%(fiscalyear)s\"."
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+"Za knjiženje fakture \"%(invoice)s\", je potrebno nastaviti šifrant na "
+"poslovnem letu \"%(fiscalyear)s\"."
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 "Ni mogoče preklicati fakture kupca \"%(invoice)s\", saj je knjižena. "
 "Nastavitve podjetja ne dovoljujejo preklica faktur."
@@ -1377,14 +1397,18 @@
 msgid "General"
 msgstr "Splošno"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "Zapiski"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/tr.po` & `trytond_account_invoice-7.2.0/locale/fi.po`

 * *Files 4% similar despite different names*

```diff
@@ -980,14 +980,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1204,14 +1218,15 @@
 msgstr "Payment Terms"
 
 #, fuzzy
 msgctxt "model:party.party.payment_term,name:"
 msgid "Party Payment Term"
 msgstr "Test Payment Term"
 
+#, fuzzy
 msgctxt "report:account.invoice:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:account.invoice:"
 msgid "Amount"
 msgstr ""
@@ -1380,14 +1395,19 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
+#, fuzzy
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/uk.po` & `trytond_account_invoice-7.2.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -941,14 +941,28 @@
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr ""
 
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr ""
+
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1330,14 +1344,18 @@
 msgid "General"
 msgstr ""
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr ""
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr ""
```

### Comparing `trytond_account_invoice-7.0.4/locale/zh_CN.po` & `trytond_account_invoice-7.2.0/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -945,14 +945,30 @@
 "company \"%(company)s\"."
 msgstr "当参与者 \"%(party)s\" 具有公司 \"%(company)s\" 的待定凭证时，不能删除。"
 
 msgctxt "model:ir.message,text:msg_invoice_credit_refund_not_posted"
 msgid "You cannot refund invoice \"%(invoice)s\" because it is not posted."
 msgstr "无法退还凭证 \"%(invoice)s\" ，因为它未过帐。"
 
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_credit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange credit "
+"account for \"%(company)s\"."
+msgstr "要对 \"%(invoice)s\" 入账，必须在会计年度 \"%(fiscalyear)s\" 上定义一个序列。"
+
+#, fuzzy
+msgctxt ""
+"model:ir.message,text:msg_invoice_currency_exchange_debit_account_missing"
+msgid ""
+"To post invoice \"%(invoice)s\", you must define a currency exchange debit "
+"account for \"%(company)s\"."
+msgstr "要对 \"%(invoice)s\" 入账，必须在会计年度 \"%(fiscalyear)s\" 上定义一个序列。"
+
 msgctxt "model:ir.message,text:msg_invoice_customer_cancel_move"
 msgid ""
 "You cannot cancel customer invoice \"%(invoice)s\" because it is posted and "
 "company setup does not allow it."
 msgstr "无法取消客户原始凭证 \"%(invoice)s\"，因为它已过帐并且公司设置不允许。"
 
 msgctxt "model:ir.message,text:msg_invoice_date_future"
@@ -1336,14 +1352,18 @@
 msgid "General"
 msgstr "基本"
 
 msgctxt "view:account.invoice.line:"
 msgid "Notes"
 msgstr "注释"
 
+msgctxt "view:account.invoice.payment_term.line.delta:"
+msgid "Operations are applied in this displayed order."
+msgstr ""
+
 msgctxt "view:account.invoice.payment_term.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:account.invoice.report.revision:"
 msgid "Time"
 msgstr "时间"
```

### Comparing `trytond_account_invoice-7.0.4/message.xml` & `trytond_account_invoice-7.2.0/message.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_account_invoice-7.0.4/message.xml` & `trytond_account_invoice-7.2.0/message.xml`

```diff
@@ -74,18 +74,27 @@
     </record>
     <record model="ir.message" id="msg_close_period_non_posted_invoices">
       <field name="text">To close the periods you must post the invoices &quot;%(invoices)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_invoice_date_future">
       <field name="text">The invoices &quot;%(invoices)s&quot; have an invoice date in the future.</field>
     </record>
+    <record model="ir.message" id="msg_invoice_default_taxes">
+      <field name="text">The invoice &quot;%(invoice)s&quot; does not have the default taxes for %(lines)s.</field>
+    </record>
     <record model="ir.message" id="msg_invoice_similar">
       <field name="text">The invoice &quot;%(invoice)s&quot; is similar to invoice &quot;%(similar)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_cancel_invoice_move">
       <field name="text">The moves &quot;%(moves)s&quot; have the posted invoices &quot;%(invoices)s&quot; as origin.</field>
     </record>
     <record model="ir.message" id="msg_cancel_invoice_move_description">
       <field name="text">Cancelling them will reconcile the move lines thus paying the invoices. You might want to cancel the invoices first.</field>
     </record>
+    <record model="ir.message" id="msg_invoice_currency_exchange_credit_account_missing">
+      <field name="text">To post invoice &quot;%(invoice)s&quot;, you must define a currency exchange credit account for &quot;%(company)s&quot;.</field>
+    </record>
+    <record model="ir.message" id="msg_invoice_currency_exchange_debit_account_missing">
+      <field name="text">To post invoice &quot;%(invoice)s&quot;, you must define a currency exchange debit account for &quot;%(company)s&quot;.</field>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_invoice-7.0.4/party.py` & `trytond_account_invoice-7.2.0/party.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # this repository contains the full copyright notices and license terms.
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, ValueMixin, fields
 from trytond.modules.party.exceptions import EraseError
 from trytond.pool import Pool, PoolMeta
 
 customer_payment_term = fields.Many2One(
-    'account.invoice.payment_term', "Customer Payment Term")
+    'account.invoice.payment_term', "Customer Payment Term",
+    ondelete='RESTRICT')
 supplier_payment_term = fields.Many2One(
-    'account.invoice.payment_term', "Supplier Payment Term")
+    'account.invoice.payment_term', "Supplier Payment Term",
+    ondelete='RESTRICT')
 
 
 class Address(metaclass=PoolMeta):
     __name__ = 'party.address'
     invoice = fields.Boolean('Invoice')
```

### Comparing `trytond_account_invoice-7.0.4/party.xml` & `trytond_account_invoice-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/payment_term.py` & `trytond_account_invoice-7.2.0/payment_term.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/payment_term.xml` & `trytond_account_invoice-7.2.0/payment_term.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account_invoice-7.0.4/payment_term.xml` & `trytond_account_invoice-7.2.0/payment_term.xml`

```diff
@@ -26,22 +26,22 @@
     <record model="ir.action.act_window.view" id="act_payment_term_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="payment_term_view_form"/>
       <field name="act_window" ref="act_payment_term_form"/>
     </record>
     <menuitem parent="menu_payment_terms_configuration" action="act_payment_term_form" sequence="10" id="menu_payment_term_form"/>
     <record model="ir.model.access" id="access_payment_term">
-      <field name="model" search="[('model', '=', 'account.invoice.payment_term')]"/>
+      <field name="model">account.invoice.payment_term</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_term_account_admin">
-      <field name="model" search="[('model', '=', 'account.invoice.payment_term')]"/>
+      <field name="model">account.invoice.payment_term</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="payment_term_line_view_list">
```

### Comparing `trytond_account_invoice-7.0.4/setup.py` & `trytond_account_invoice-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_cancelling_invoice_move.rst` & `trytond_account_invoice-7.2.0/tests/scenario_cancelling_invoice_move.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ================================
 Cancelling Invoice Move Scenario
 ================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
-    >>> from trytond.modules.account_invoice.exceptions import (
-    ...     CancelInvoiceMoveWarning)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.exceptions import CancelInvoiceMoveWarning
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
     >>> ProductUom = Model.get('product.uom')
@@ -79,15 +78,15 @@
 Post invoice and cancel the created move::
 
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
     >>> cancel_move = Wizard('account.move.cancel', [invoice.move])
     >>> cancel_move.form.description = 'Cancel'
-    >>> cancel_move.execute('cancel')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> cancel_move.execute('cancel')
     Traceback (most recent call last):
         ...
     CancelInvoiceMoveWarning: ...
 
 Bypass the warning and cancel the move::
 
     >>> try:
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_credit_note.rst` & `trytond_account_invoice-7.2.0/tests/scenario_credit_note.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ====================
 Credit Note Scenario
 ====================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
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
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Invoice Scenario
 ================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
@@ -172,31 +172,28 @@
     >>> invoice.save()
     >>> bool(invoice.has_report_cache)
     False
 
 Test change tax::
 
     >>> tax_line, = invoice.taxes
-    >>> tax_line.tax == tax
-    True
+    >>> assertEqual(tax_line.tax, tax)
     >>> tax_line.tax = None
     >>> tax_line.tax = tax
 
 Validate invoice::
 
     >>> invoice.click('validate_invoice')
-    >>> invoice.validated_by == employee
-    True
+    >>> assertEqual(invoice.validated_by, employee)
 
 Post invoice::
 
     >>> invoice.invoice_date = today
     >>> invoice.click('post')
-    >>> invoice.posted_by == employee
-    True
+    >>> assertEqual(invoice.posted_by, employee)
     >>> invoice.state
     'posted'
     >>> invoice.tax_identifier.code
     'BE0897290877'
     >>> bool(invoice.has_report_cache)
     True
     >>> invoice.untaxed_amount
@@ -248,16 +245,16 @@
     'cancelled'
     >>> bool(invoice.reconciled)
     True
     >>> credit_note, = Invoice.find([
     ...     ('type', '=', 'out'), ('id', '!=', invoice.id)])
     >>> credit_note.state
     'paid'
-    >>> all(line.taxes_date == today for line in credit_note.lines)
-    True
+    >>> for line in credit_note.lines:
+    ...     assertEqual(line.taxes_date, today)
     >>> receivable.reload()
     >>> receivable.debit
     Decimal('240.00')
     >>> receivable.credit
     Decimal('240.00')
     >>> revenue.reload()
     >>> revenue.debit
@@ -366,24 +363,21 @@
     >>> line = invoice.lines.new()
     >>> line.product = product
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('0.0035')
     >>> invoice.save()
     >>> invoice.untaxed_amount
     Decimal('0.00')
-    >>> invoice.taxes[0].base == invoice.untaxed_amount
-    True
+    >>> assertEqual(invoice.taxes[0].base, invoice.untaxed_amount)
     >>> empty_invoice, found_invoice = Invoice.find(
     ...     [('untaxed_amount', '=', Decimal(0))], order=[('id', 'ASC')])
-    >>> found_invoice.id == invoice.id
-    True
+    >>> assertEqual(found_invoice, invoice)
     >>> empty_invoice, found_invoice = Invoice.find(
     ...     [('total_amount', '=', Decimal(0))], order=[('id', 'ASC')])
-    >>> found_invoice.id == invoice.id
-    True
+    >>> assertEqual(found_invoice, invoice)
 
 Clear company tax_identifier::
 
     >>> tax_identifier, = company.party.identifiers
     >>> tax_identifier.type = None
     >>> tax_identifier.save()
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_alternate_currency.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 Invoice Scenario Alternate Currency
 ===================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.exceptions import InvoiceTaxesWarning
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    >>> from trytond.tests.tools import activate_modules
+
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
+    >>> Warning = Model.get('res.user.warning')
+
 Create company::
 
     >>> currency = get_currency('USD')
     >>> eur = get_currency('EUR')
     >>> _ = create_company(currency=currency)
     >>> company = get_company()
 
@@ -174,14 +177,23 @@
     Decimal('400.00')
     >>> invoice.untaxed_amount
     Decimal('400.00')
     >>> invoice.tax_amount
     Decimal('-40.00')
     >>> invoice.total_amount
     Decimal('360.00')
+    >>> try:
+    ...     invoice.click('post')
+    ... except InvoiceTaxesWarning as warning:
+    ...     _, (key, *_) = warning.args
+    ...     raise
+    Traceback (most recent call last):
+        ...
+    InvoiceTaxesWarning: ...
+    >>> Warning(user=config.user, name=key).save()
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
     >>> invoice.untaxed_amount
     Decimal('400.00')
     >>> invoice.tax_amount
     Decimal('-40.00')
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_alternate_currency_lower_rate.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_lower_rate.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Invoice Scenario Alternate Currency Lower Rate
 ==============================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
@@ -84,16 +85,15 @@
     Decimal('400.00')
 
 Pay the invoice::
 
     >>> pay = invoice.click('pay')
     >>> pay.form.amount
     Decimal('400.00')
-    >>> pay.form.currency == eur
-    True
+    >>> assertEqual(pay.form.currency, eur)
     >>> pay.form.payment_method = payment_method
     >>> pay.form.date = today
     >>> pay.execute('choice')
     >>> pay.state
     'end'
     >>> invoice.state
     'paid'
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_alternate_currency_rate_change.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternate_currency_rate_change.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
@@ -97,16 +98,15 @@
     Decimal('400.00')
 
 Pay the invoice::
 
     >>> pay = Wizard('account.invoice.pay', [invoice])
     >>> pay.form.amount
     Decimal('400.00')
-    >>> pay.form.currency == eur
-    True
+    >>> assertEqual(pay.form.currency, eur)
     >>> pay.form.payment_method = payment_method
     >>> pay.form.date = tomorrow
     >>> pay.execute('choice')
     >>> pay.state
     'end'
     >>> invoice.state
     'paid'
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_alternative_payee.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_alternative_payee.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 ==================================
 
 Imports::
 
     >>> from decimal import Decimal
 
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
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
     >>> Invoice = Model.get('account.invoice')
     >>> Journal = Model.get('account.journal')
@@ -87,16 +86,15 @@
     >>> party3.reload()
     >>> party3.receivable
     Decimal('0.0')
 
 Copying invoice with single alternative payee is kept::
 
     >>> duplicate_inv, = invoice.duplicate()
-    >>> duplicate_inv.alternative_payees == invoice.alternative_payees
-    True
+    >>> assertEqual(duplicate_inv.alternative_payees, invoice.alternative_payees)
 
 Set another payee::
 
     >>> delegate = Wizard(
     ...     'account.invoice.lines_to_pay.delegate', [invoice])
     >>> delegate_lines, = delegate.actions
     >>> delegate_lines.form.party = party3
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_customer_sequential.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_customer_sequential.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ===========================
 Customer Invoice Sequential
 ===========================
 
 Imports::
 
-    >>> from decimal import Decimal
     >>> import datetime as dt
+    >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+
     >>> today = dt.date.today()
     >>> past_year = today - dt.timedelta(days=365)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
@@ -76,15 +77,15 @@
     >>> invoice.invoice_date = fiscalyear.periods[0].start_date
     >>> line = invoice.lines.new()
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('5')
     >>> line.account = accounts['revenue']
     >>> invoice.save()
 
-    >>> invoice.click('post')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> invoice.click('post')
     Traceback (most recent call last):
         ...
     InvoiceNumberError: ...
 
 Post invoice on the third period::
 
     >>> invoice.invoice_date = fiscalyear.periods[2].start_date
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_group_line.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_group_line.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ================
 Invoice Scenario
 ================
 
 Imports::
 
-    >>> import datetime
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
 
@@ -119,16 +118,16 @@
     >>> move.click('post')
 
     >>> lines = Line.find([
     ...         ('account', '=', receivable.id),
     ...         ('reconciliation', '=', None),
     ...         ])
     >>> reconcile_lines = Wizard('account.move.reconcile_lines', lines)
-    >>> reconcile_lines.state == 'end'
-    True
+    >>> reconcile_lines.state
+    'end'
 
     >>> invoice.reload()
     >>> invoice.state
     'paid'
     >>> invoice.amount_to_pay
     Decimal('0')
     >>> supplier_invoice.reload()
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_in_future.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_in_future.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Invoice in Future
 =================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (create_company,
-    ...     get_company)
-    >>> from trytond.modules.account.tests.tools import (create_fiscalyear,
-    ...     create_chart, get_accounts)
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
+
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
@@ -54,15 +55,15 @@
     >>> line.description = 'Test'
     >>> line.quantity = 1
     >>> line.unit_price = Decimal(20)
 
 Posting an invoice in the future raises a warning::
 
     >>> invoice.invoice_date = tomorrow
-    >>> invoice.click('post')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> invoice.click('post')
     Traceback (most recent call last):
         ...
     InvoiceFutureWarning: ...
 
 Post invoice::
 
     >>> invoice.invoice_date = today
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_manual_tax.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_manual_tax.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Invoice Manual Tax
 ==================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax,
-    ...     create_tax_code)
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
     >>> Invoice = Model.get('account.invoice')
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_overpayment.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_overpayment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 Invoice Overpayment Scenario
 ============================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_report_revision.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_report_revision.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ================================
 Invoice Report Revision Scenario
 ================================
 
 Imports::
 
     >>> import datetime as dt
-
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_reschedule_lines.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_reschedule_lines.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =================================
 Invoice Reschedule Lines Scenario
 =================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
     >>> Invoice = Model.get('account.invoice')
     >>> Journal = Model.get('account.journal')
@@ -75,15 +75,15 @@
 Reschedule line::
 
     >>> reschedule = invoice.click('reschedule_lines_to_pay')
     >>> reschedule_lines, = reschedule.actions
     >>> reschedule_lines.form.total_amount
     Decimal('10.00')
     >>> reschedule_lines.form.start_date = period.end_date
-    >>> reschedule_lines.form.frequency ='monthly'
+    >>> reschedule_lines.form.frequency = 'monthly'
     >>> reschedule_lines.form.number = 2
     >>> reschedule_lines.execute('preview')
     >>> reschedule_lines.execute('reschedule')
 
     >>> invoice.reload()
     >>> invoice.state
     'posted'
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_supplier.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 =========================
 Invoice Supplier Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
@@ -183,33 +182,33 @@
     >>> credit = Wizard('account.invoice.credit', [invoice])
     >>> credit.form.with_refund = False
     >>> credit.execute('credit')
     >>> credit_note, = Invoice.find(
     ...     [('type', '=', 'in'), ('id', '!=', invoice.id)])
     >>> credit_note.state
     'draft'
-    >>> credit_note.untaxed_amount == -invoice.untaxed_amount
-    True
-    >>> credit_note.tax_amount == -invoice.tax_amount
-    True
-    >>> credit_note.total_amount == -invoice.total_amount
-    True
+    >>> credit_note.untaxed_amount
+    Decimal('-110.00')
+    >>> credit_note.tax_amount
+    Decimal('-10.00')
+    >>> credit_note.total_amount
+    Decimal('-120.00')
 
 A warning is raised when creating an invoice with same reference::
 
     >>> invoice = Invoice()
     >>> invoice.type = 'in'
     >>> invoice.party = party
     >>> invoice.invoice_date = today
     >>> invoice.reference = 'FAC001'
     >>> line = invoice.lines.new()
     >>> line.product = product
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('20')
-    >>> invoice.click('post') # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> invoice.click('post')
     Traceback (most recent call last):
         ...
     InvoiceSimilarWarning: ...
     >>> invoice.reference = 'FAC002'
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_supplier_post_paid.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_supplier_post_paid.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 ==========================
 Invoice Supplier Post Paid
 ==========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_tax_deductible.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_tax_deductible.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 Invoice Tax Deductible
 ======================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax)
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.exceptions import InvoiceTaxesWarning
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
     >>> Invoice = Model.get('account.invoice')
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
     >>> ProductTemplate = Model.get('product.template')
     >>> ProductUom = Model.get('product.uom')
+    >>> Warning = Model.get('res.user.warning')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
@@ -85,14 +88,23 @@
     >>> line.taxes_deductible_rate
     Decimal('0.5')
     >>> line.taxes_deductible_rate = Decimal(0)
     >>> line.amount
     Decimal('550.00')
     >>> invoice.untaxed_amount, invoice.tax_amount, invoice.total_amount
     (Decimal('550.00'), Decimal('0.00'), Decimal('550.00'))
+    >>> try:
+    ...     invoice.click('post')
+    ... except InvoiceTaxesWarning as warning:
+    ...     _, (key, *_) = warning.args
+    ...     raise
+    Traceback (most recent call last):
+        ...
+    InvoiceTaxesWarning: ...
+    >>> Warning(user=config.user, name=key).save()
     >>> invoice.click('post')
     >>> invoice.untaxed_amount, invoice.tax_amount, invoice.total_amount
     (Decimal('550.00'), Decimal('0.00'), Decimal('550.00'))
     >>> len(invoice.taxes)
     0
 
 Post a supplier invoice with 50% deductible rate::
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_invoice_with_credit.rst` & `trytond_account_invoice-7.2.0/tests/scenario_invoice_with_credit.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ============================
 Invoice with credit Scenario
 ============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
```

### Comparing `trytond_account_invoice-7.0.4/tests/scenario_renew_fiscalyear.rst` & `trytond_account_invoice-7.2.0/tests/scenario_renew_fiscalyear.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 =========================
 Renew Fiscalyear Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
-    >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model, Wizard
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
-    >>> from trytond.modules.account_invoice.tests.tools \
-    ...     import set_fiscalyear_invoice_sequences
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice')
 
 Create company::
@@ -95,11 +94,11 @@
 
 Renew fiscalyear and test sequence name is updated::
 
     >>> renew_fiscalyear = Wizard('account.fiscalyear.renew')
     >>> renew_fiscalyear.form.reset_sequences = True
     >>> renew_fiscalyear.execute('create_')
     >>> new_fiscalyear, = renew_fiscalyear.actions[0]
-    >>> all(seq.out_invoice_sequence.name ==
-    ...         'Sequence %s' % new_fiscalyear.name
-    ...     for seq in new_fiscalyear.invoice_sequences)
-    True
+    >>> for sequence in new_fiscalyear.invoice_sequences:
+    ...     assertEqual(
+    ...         sequence.out_invoice_sequence.name,
+    ...         'Sequence %s' % new_fiscalyear.name)
```

### Comparing `trytond_account_invoice-7.0.4/tests/test_module.py` & `trytond_account_invoice-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/tests/tools.py` & `trytond_account_invoice-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/tox.ini` & `trytond_account_invoice-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/PKG-INFO` & `trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.0.4
+Version: 7.2.0
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -50,23 +50,23 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ######################
 Account Invoice Module
 ######################
 
 The *Account Invoice Module* adds the concept of invoicing to Tryton.
 It allows the creation of customer and supplier invoices, and can handle the
```

### Comparing `trytond_account_invoice-7.0.4/trytond_account_invoice.egg-info/SOURCES.txt` & `trytond_account_invoice-7.2.0/trytond_account_invoice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_cancelling_invoice_move.rst
 ./tests/scenario_credit_note.rst
 ./tests/scenario_invoice.rst
 ./tests/scenario_invoice_alternate_currency.rst
+./tests/scenario_invoice_alternate_currency_exchange.rst
 ./tests/scenario_invoice_alternate_currency_lower_rate.rst
 ./tests/scenario_invoice_alternate_currency_rate_change.rst
 ./tests/scenario_invoice_alternative_payee.rst
 ./tests/scenario_invoice_customer_sequential.rst
 ./tests/scenario_invoice_group_line.rst
 ./tests/scenario_invoice_in_future.rst
 ./tests/scenario_invoice_manual_tax.rst
@@ -127,18 +128,18 @@
 ./view/payment_term_tree.xml
 doc/conf.py
 doc/configuration.rst
 doc/design.rst
 doc/index.rst
 doc/releases.rst
 doc/requirements-doc.txt
-doc/usage/amend.rst
+doc/usage/amend.inc.rst
 doc/usage/index.rst
-doc/usage/prepare.rst
-doc/usage/process.rst
+doc/usage/prepare.inc.rst
+doc/usage/process.inc.rst
 icons/LICENSE
 icons/tryton-invoice.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
@@ -162,14 +163,15 @@
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_cancelling_invoice_move.rst
 tests/scenario_credit_note.rst
 tests/scenario_invoice.rst
 tests/scenario_invoice_alternate_currency.rst
+tests/scenario_invoice_alternate_currency_exchange.rst
 tests/scenario_invoice_alternate_currency_lower_rate.rst
 tests/scenario_invoice_alternate_currency_rate_change.rst
 tests/scenario_invoice_alternative_payee.rst
 tests/scenario_invoice_customer_sequential.rst
 tests/scenario_invoice_group_line.rst
 tests/scenario_invoice_in_future.rst
 tests/scenario_invoice_manual_tax.rst
```

### Comparing `trytond_account_invoice-7.0.4/view/credit_start_form.xml` & `trytond_account_invoice-7.2.0/view/credit_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_form.xml` & `trytond_account_invoice-7.2.0/view/invoice_form.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_account_invoice-7.0.4/view/invoice_form.xml` & `trytond_account_invoice-7.2.0/view/invoice_form.xml`

```diff
@@ -52,14 +52,18 @@
       <field name="company"/>
       <label name="tax_identifier"/>
       <field name="tax_identifier"/>
       <label name="account"/>
       <field name="account"/>
       <label name="accounting_date"/>
       <field name="accounting_date"/>
+      <label name="validated_by"/>
+      <field name="validated_by"/>
+      <label name="posted_by"/>
+      <field name="posted_by"/>
       <field name="alternative_payees" colspan="4"/>
       <label name="move"/>
       <field name="move"/>
       <label name="cancel_move"/>
       <field name="cancel_move"/>
       <field name="additional_moves" colspan="4"/>
       <separator name="comment" colspan="4"/>
```

### Comparing `trytond_account_invoice-7.0.4/view/invoice_line_form.xml` & `trytond_account_invoice-7.2.0/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_line_tree.xml` & `trytond_account_invoice-7.2.0/view/invoice_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_line_tree_sequence.xml` & `trytond_account_invoice-7.2.0/view/invoice_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_sequence_form.xml` & `trytond_account_invoice-7.2.0/view/invoice_sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_tax_form.xml` & `trytond_account_invoice-7.2.0/view/invoice_tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_tax_tree_sequence.xml` & `trytond_account_invoice-7.2.0/view/invoice_tax_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/invoice_tree.xml` & `trytond_account_invoice-7.2.0/view/invoice_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/move_line_list_payment.xml` & `trytond_account_invoice-7.2.0/view/move_line_list_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/party_form.xml` & `trytond_account_invoice-7.2.0/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/pay_ask_form.xml` & `trytond_account_invoice-7.2.0/view/pay_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/pay_start_form.xml` & `trytond_account_invoice-7.2.0/view/pay_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/payment_method_form.xml` & `trytond_account_invoice-7.2.0/view/payment_method_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/payment_term_form.xml` & `trytond_account_invoice-7.2.0/view/payment_term_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.0.4/view/payment_term_line_form.xml` & `trytond_account_invoice-7.2.0/view/payment_term_line_form.xml`

 * *Files identical despite different names*

