# Comparing `tmp/trytond_incoterm-7.0.1.tar.gz` & `tmp/trytond_incoterm-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_incoterm-7.0.1.tar", last modified: Fri Nov 17 18:52:59 2023, max compression
+gzip compressed data, was "trytond_incoterm-7.2.0.tar", last modified: Mon Apr 29 15:41:07 2024, max compression
```

## Comparing `trytond_incoterm-7.0.1.tar` & `trytond_incoterm-7.2.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:52:59.681019 trytond_incoterm-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      197 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      855 2023-11-17 18:52:57.000000 trytond_incoterm-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-11-17 18:52:56.000000 trytond_incoterm-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3413 2023-11-17 18:52:59.681019 trytond_incoterm-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1636 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6269 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:52:59.681019 trytond_incoterm-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2809 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3169 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/incoterm.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11274 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/incoterm.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:52:59.674352 trytond_incoterm-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5670 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5744 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5717 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5743 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4575 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4510 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5607 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1055 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3971 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1866 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2326 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3730 2023-11-15 17:15:53.000000 trytond_incoterm-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-11-17 18:52:59.681019 trytond_incoterm-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5076 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1499 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1404 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:52:59.674352 trytond_incoterm-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6212 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/tests/scenario_incoterm.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      628 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-30 17:55:12.000000 trytond_incoterm-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:52:59.681019 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3413 2023-11-17 18:52:59.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2787 2023-11-17 18:52:59.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-11-17 18:52:59.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-11-17 18:52:59.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:51.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-11-17 18:52:59.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-11-17 18:52:59.000000 trytond_incoterm-7.0.1/trytond_incoterm.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-11-17 18:52:59.677685 trytond_incoterm-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/carrier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/party_form_purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/party_form_sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/party_incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/party_incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/purchase_request_quotation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/sale_opportunity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/stock_shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/stock_shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/stock_shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-10-30 17:06:38.000000 trytond_incoterm-7.0.1/view/stock_shipment_out_return_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      855 2024-04-29 15:20:17.000000 trytond_incoterm-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:20:17.000000 trytond_incoterm-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1636 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6269 2024-01-27 09:58:52.000000 trytond_incoterm-7.2.0/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.938338 trytond_incoterm-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:11.000000 trytond_incoterm-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3169 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/incoterm.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11251 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/incoterm.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.941671 trytond_incoterm-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5670 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5744 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5717 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5743 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4510 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5607 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1055 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3971 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2326 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3730 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5068 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1499 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1404 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.941671 trytond_incoterm-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6119 2024-04-22 12:14:36.000000 trytond_incoterm-7.2.0/tests/scenario_incoterm.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1200 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:11.000000 trytond_incoterm-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-29 15:20:12.000000 trytond_incoterm-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2769 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/carrier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_form_purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_form_sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/purchase_request_quotation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/sale_opportunity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_out_return_form.xml
```

### Comparing `trytond_incoterm-7.0.1/CHANGELOG` & `trytond_incoterm-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2023-11-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_incoterm-7.0.1/COPYRIGHT` & `trytond_incoterm-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_incoterm-7.0.1/LICENSE` & `trytond_incoterm-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/PKG-INFO` & `trytond_incoterm-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_incoterm
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for incoterms
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-incoterm/
+Project-URL: Documentation, https://docs.tryton.org/modules-incoterm/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton incoterm
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,30 +48,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_request_quotation<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_opportunity<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_invoice_grouping<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_request_quotation<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_opportunity<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_grouping<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 ###############
 Incoterm Module
 ###############
 
 This *Incoterm Model* is used to manage the `Incoterms
 <https://en.wikipedia.org/wiki/Incoterms>`_ on sales, purchases and shipments.
```

### Comparing `trytond_incoterm-7.0.1/__init__.py` & `trytond_incoterm-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/account.py` & `trytond_incoterm-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/carrier.xml` & `trytond_incoterm-7.2.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/common.py` & `trytond_incoterm-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/doc/conf.py` & `trytond_incoterm-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_incoterm-7.0.1/incoterm.py` & `trytond_incoterm-7.2.0/incoterm.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/incoterm.xml` & `trytond_incoterm-7.2.0/incoterm.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_incoterm-7.0.1/incoterm.xml` & `trytond_incoterm-7.2.0/incoterm.xml`

```diff
@@ -25,15 +25,15 @@
     <record model="ir.action.act_window.view" id="act_incoterm_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="incoterm_view_form"/>
       <field name="act_window" ref="act_incoterm_form"/>
     </record>
     <menuitem parent="company.menu_company" sequence="30" action="act_incoterm_form" id="menu_incoterm"/>
     <record model="ir.model.access" id="access_incoterm">
-      <field name="model" search="[('model', '=', 'incoterm.incoterm')]"/>
+      <field name="model">incoterm.incoterm</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
   <data grouped="1">
```

### Comparing `trytond_incoterm-7.0.1/locale/bg.po` & `trytond_incoterm-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/ca.po` & `trytond_incoterm-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/cs.po` & `trytond_incoterm-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/de.po` & `trytond_incoterm-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/es.po` & `trytond_incoterm-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/es_419.po` & `trytond_incoterm-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/et.po` & `trytond_incoterm-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/fa.po` & `trytond_incoterm-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/fi.po` & `trytond_incoterm-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/fr.po` & `trytond_incoterm-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/hu.po` & `trytond_incoterm-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/id.po` & `trytond_incoterm-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/it.po` & `trytond_incoterm-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/lo.po` & `trytond_incoterm-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/lt.po` & `trytond_incoterm-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/nl.po` & `trytond_incoterm-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/pl.po` & `trytond_incoterm-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/pt.po` & `trytond_incoterm-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/ro.po` & `trytond_incoterm-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/ru.po` & `trytond_incoterm-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/sl.po` & `trytond_incoterm-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/tr.po` & `trytond_incoterm-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/uk.po` & `trytond_incoterm-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/locale/zh_CN.po` & `trytond_incoterm-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/message.xml` & `trytond_incoterm-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/party.py` & `trytond_incoterm-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/party.xml` & `trytond_incoterm-7.2.0/party.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_incoterm-7.0.1/party.xml` & `trytond_incoterm-7.2.0/party.xml`

```diff
@@ -25,15 +25,15 @@
     <record model="ir.ui.view" id="party_incoterm_view_list">
       <field name="model">party.incoterm</field>
       <field name="type">tree</field>
       <field name="name">party_incoterm_list</field>
     </record>
     <record model="ir.rule.group" id="rule_group_party_incoterm_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'party.incoterm')]"/>
+      <field name="model">party.incoterm</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_party_incoterm_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_party_incoterm_companies"/>
     </record>
   </data>
```

### Comparing `trytond_incoterm-7.0.1/purchase.py` & `trytond_incoterm-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/purchase.xml` & `trytond_incoterm-7.2.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/sale.py` & `trytond_incoterm-7.2.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         shipment = super()._get_shipment_sale(Shipment, key)
         if isinstance(shipment, ShipmentOut):
             shipment.incoterm = self.incoterm
             shipment.incoterm_location = self.incoterm_location
         return shipment
 
     def _get_shipment_grouping_fields(self, shipment):
-        return super()._get_shipment_grouping_fields(shipment) + [
-            'incoterm', 'incoterm_location']
+        return super()._get_shipment_grouping_fields(shipment) | {
+            'incoterm', 'incoterm_location'}
 
     @property
     @fields.depends('company', 'warehouse', 'shipment_address')
     def _incoterm_required(self):
         if self.company.incoterms:
             if (self.warehouse and self.warehouse.address
                     and self.shipment_address):
```

### Comparing `trytond_incoterm-7.0.1/sale.xml` & `trytond_incoterm-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/setup.py` & `trytond_incoterm-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,29 +57,29 @@
     get_require_version('trytond_account_invoice_stock'),
     get_require_version('trytond_carrier'),
     get_require_version('trytond_purchase'),
     get_require_version('trytond_purchase_request_quotation'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_sale_shipment_cost'),
     get_require_version('trytond_sale_opportunity'),
-    get_require_version('trytond_sale_invoice_grouping'),
+    get_require_version('trytond_sale_shipment_grouping'),
     get_require_version('trytond_stock'),
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module for incoterms',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-incoterm/',
+        "Documentation": 'https://docs.tryton.org/modules-incoterm/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton incoterm',
     package_dir={'trytond.modules.incoterm': '.'},
     packages=(
         ['trytond.modules.incoterm']
```

### Comparing `trytond_incoterm-7.0.1/stock.py` & `trytond_incoterm-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/stock.xml` & `trytond_incoterm-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/tests/scenario_incoterm.rst` & `trytond_incoterm-7.2.0/tests/scenario_incoterm.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 =================
 Incoterm Scenario
 =================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['incoterm', 'sale', 'sale_shipment_cost', 'purchase'])
 
     >>> Address = Model.get('party.address')
@@ -132,15 +131,15 @@
     >>> carrier = Carrier()
     >>> party = Party(name="Carrier")
     >>> party.save()
     >>> carrier.party = party
     >>> carrier.carrier_product = carrier_product
     >>> carrier.save()
     >>> carrier_waterway, = carrier.duplicate()
-    >>> carrier_waterway.mode= 'waterway'
+    >>> carrier_waterway.mode = 'waterway'
     >>> carrier_waterway.save()
 
 Test incoterms are deducted from sale::
 
     >>> sale = Sale()
     >>> sale.party = customer
     >>> sale.carrier = carrier_waterway
@@ -148,36 +147,35 @@
     'CIF (2020)'
     >>> sale.incoterm_location
     >>> sale.carrier = carrier
     >>> sale.incoterm
     >>> sale.shipment_cost_method = None
     >>> sale.incoterm.rec_name
     'FCA (2020)'
-    >>> sale.incoterm_location == warehouse_address
-    True
+    >>> assertEqual(sale.incoterm_location, warehouse_address)
 
 Try sale without incoterm::
 
     >>> sale = Sale()
     >>> sale.party = customer
     >>> sale.carrier = carrier_waterway
     >>> line = sale.lines.new()
     >>> line.product = product
     >>> line.quantity = 1
     >>> sale.incoterm = None
-    >>> sale.click('quote')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.click('quote')
     Traceback (most recent call last):
         ...
     SaleQuotationError: ...
 
 Try sale with incoterm::
 
     >>> sale.incoterm, = Incoterm.find([
     ...         ('code', '=', 'CIF'), ('version', '=', '2020')])
-    >>> sale.click('quote')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.click('quote')
     Traceback (most recent call last):
         ...
     RequiredValidationError: ...
 
 Try sale with incoterm and location::
 
     >>> sale.incoterm_location, = port.addresses
@@ -189,16 +187,15 @@
 
     >>> sale.click('confirm')
     >>> sale.state
     'processing'
     >>> shipment, = sale.shipments
     >>> shipment.incoterm.rec_name
     'CIF (2020)'
-    >>> shipment.incoterm_location == port.addresses[0]
-    True
+    >>> assertEqual(shipment.incoterm_location, port.addresses[0])
 
 Test incoterm is set on purchase::
 
     >>> purchase = Purchase()
     >>> purchase.party = supplier
     >>> purchase.incoterm.rec_name
     'CFR (2020)'
```

### Comparing `trytond_incoterm-7.0.1/tox.ini` & `trytond_incoterm-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/trytond_incoterm.egg-info/PKG-INFO` & `trytond_incoterm-7.2.0/trytond_incoterm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-incoterm
-Version: 7.0.1
+Name: trytond_incoterm
+Version: 7.2.0
 Summary: Tryton module for incoterms
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-incoterm/
+Project-URL: Documentation, https://docs.tryton.org/modules-incoterm/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton incoterm
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,30 +48,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_request_quotation<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_opportunity<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_invoice_grouping<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_request_quotation<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_opportunity<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_grouping<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
 
 ###############
 Incoterm Module
 ###############
 
 This *Incoterm Model* is used to manage the `Incoterms
 <https://en.wikipedia.org/wiki/Incoterms>`_ on sales, purchases and shipments.
```

### Comparing `trytond_incoterm-7.0.1/trytond_incoterm.egg-info/SOURCES.txt` & `trytond_incoterm-7.2.0/trytond_incoterm.egg-info/SOURCES.txt`

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

### Comparing `trytond_incoterm-7.0.1/view/incoterm_form.xml` & `trytond_incoterm-7.2.0/view/incoterm_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.0.1/view/party_incoterm_form.xml` & `trytond_incoterm-7.2.0/view/party_incoterm_form.xml`

 * *Files identical despite different names*

