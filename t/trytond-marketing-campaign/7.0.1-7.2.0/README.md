# Comparing `tmp/trytond_marketing_campaign-7.0.1.tar.gz` & `tmp/trytond_marketing_campaign-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_campaign-7.0.1.tar", last modified: Mon Jan  1 12:09:22 2024, max compression
+gzip compressed data, was "trytond_marketing_campaign-7.2.0.tar", last modified: Mon Apr 29 15:41:34 2024, max compression
```

## Comparing `trytond_marketing_campaign-7.0.1.tar` & `trytond_marketing_campaign-7.2.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:09:22.955583 trytond_marketing_campaign-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-01-01 12:09:20.000000 trytond_marketing_campaign-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-01-01 12:09:20.000000 trytond_marketing_campaign-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2024-01-01 12:09:22.955583 trytond_marketing_campaign-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1801 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:09:22.945583 trytond_marketing_campaign-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      873 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:09:22.948916 trytond_marketing_campaign-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5142 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5264 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5127 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5167 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5056 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5123 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-12-27 10:51:24.000000 trytond_marketing_campaign-7.0.1/marketing.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4266 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      839 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1123 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3520 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/sale_opportunity_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/sale_opportunity_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3805 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2071 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-01 12:09:22.955583 trytond_marketing_campaign-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4790 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:09:22.948916 trytond_marketing_campaign-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5296 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/tests/scenario_marketing_campaign_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-30 17:55:12.000000 trytond_marketing_campaign-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:09:22.952250 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2024-01-01 12:09:22.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2536 2024-01-01 12:09:22.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-01 12:09:22.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-01-01 12:09:22.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:52.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-01-01 12:09:22.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-01 12:09:22.000000 trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:09:22.952250 trytond_marketing_campaign-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/campaign_mixin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/parameter_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/parameter_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/sale_opportunity_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/sale_opportunity_reporting_marketing_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/sale_opportunity_reporting_marketing_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/sale_reporting_marketing_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-10-30 17:06:38.000000 trytond_marketing_campaign-7.0.1/view/sale_reporting_marketing_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      561 2024-04-29 15:20:37.000000 trytond_marketing_campaign-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:20:37.000000 trytond_marketing_campaign-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2316 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.444311 trytond_marketing_campaign-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_marketing_campaign-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:12.000000 trytond_marketing_campaign-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.444311 trytond_marketing_campaign-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5878 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6018 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5903 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5780 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5857 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-29 13:17:17.000000 trytond_marketing_campaign-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5652 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/marketing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4956 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      839 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1123 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3520 2024-02-04 18:51:26.000000 trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3805 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2071 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4940 2024-04-27 16:30:39.000000 trytond_marketing_campaign-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.444311 trytond_marketing_campaign-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5284 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/tests/scenario_marketing_campaign_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1646 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:12.000000 trytond_marketing_campaign-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-29 15:20:33.000000 trytond_marketing_campaign-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2534 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:34.000000 trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:34.447645 trytond_marketing_campaign-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/campaign_mixin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/parameter_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/parameter_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_marketing_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_marketing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_reporting_marketing_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_marketing_campaign-7.2.0/view/sale_reporting_marketing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2024-04-22 12:14:36.000000 trytond_marketing_campaign-7.2.0/web.py
```

### Comparing `trytond_marketing_campaign-7.0.1/COPYRIGHT` & `trytond_marketing_campaign-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2022-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2022-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_marketing_campaign-7.0.1/LICENSE` & `trytond_marketing_campaign-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/PKG-INFO` & `trytond_marketing_campaign-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_campaign
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to manage marketing campaign
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-marketing-campaign
+Project-URL: Documentation, https://docs.tryton.org/modules-marketing-campaign
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing campaign sale UTM
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_marketing<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_marketing<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_opportunity<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_marketing_email<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_marketing_automation<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_opportunity<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_web_shortener<7.3,>=7.2; extra == "test"
 
 #########################
 Marketing Campaign Module
 #########################
 
 The *Marketing Campaign Module* helps collecting data about marketing campaigns.
```

### Comparing `trytond_marketing_campaign-7.0.1/__init__.py` & `trytond_marketing_campaign-7.2.0/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     SaleAbstract = None
 try:
     from trytond.modules.sale_opportunity.opportunity_reporting import \
         Abstract as OpportunityAbstract
 except ImportError:
     OpportunityAbstract = None
 
-from . import marketing, sale, sale_opportunity_reporting, sale_reporting
-from .marketing import MarketingCampaignMixin, Parameter
+from . import marketing, sale, sale_opportunity_reporting, sale_reporting, web
+from .marketing import MarketingCampaignMixin, MarketingCampaignUTM, Parameter
 
-__all__ = ['register', 'Parameter', 'MarketingCampaignMixin']
+__all__ = [
+    'register', 'Parameter', 'MarketingCampaignMixin', 'MarketingCampaignUTM']
 
 
 def register():
     Pool.register(
         marketing.Campaign,
         marketing.Medium,
         marketing.Source,
@@ -37,14 +38,26 @@
         sale_opportunity_reporting.MarketingContext,
         sale_opportunity_reporting.Marketing,
         module='marketing_campaign', type_='model',
         depends=['sale_opportunity'])
     Pool.register(
         sale.POSSale,
         module='marketing_campaign', type_='model', depends=['sale_point'])
+    Pool.register(
+        web.ShortenedURL,
+        module='marketing_campaign', type_='model', depends=['web_shortener'])
+    Pool.register(
+        marketing.EmailMessage,
+        module='marketing_campaign', type_='model',
+        depends=['marketing_email'])
+    Pool.register(
+        marketing.AutomationActivity,
+        marketing.AutomationRecordActivity,
+        module='marketing_campaign', type_='model',
+        depends=['marketing_automation'])
     if SaleAbstract:
         Pool.register_mixin(
             sale_reporting.AbstractMarketingCampaign, SaleAbstract,
             module='marketing_campaign')
     if OpportunityAbstract:
         Pool.register_mixin(
             sale_opportunity_reporting.AbstractMarketingCampaign,
```

### Comparing `trytond_marketing_campaign-7.0.1/doc/conf.py` & `trytond_marketing_campaign-7.2.0/doc/conf.py`

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

### Comparing `trytond_marketing_campaign-7.0.1/doc/design.rst` & `trytond_marketing_campaign-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/doc/reference.rst` & `trytond_marketing_campaign-7.2.0/doc/reference.rst`

 * *Files 17% similar despite different names*

```diff
@@ -27,8 +27,14 @@
    :attr:`~trytond:trytond.transaction.Transaction.context` key of the same
    name.
 
 .. classmethod:: MarketingCampaignMixin.marketing_campaign_fields
 
    Yield the field names of the :class:`Parameter` fields.
 
+.. class:: MarketingCampaignUTM
+
+   The *MarketingCampaignUTM* is a mixin_ that helps to add UTM_ parameters to
+   URL.
+
 .. _mixin: https://en.wikipedia.org/wiki/Mixin
+.. _UTM: https://en.wikipedia.org/wiki/UTM_parameters
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/bg.po` & `trytond_marketing_campaign-7.2.0/locale/bg.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/ca.po` & `trytond_marketing_campaign-7.2.0/locale/cs.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,215 +1,247 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:marketing.campaign,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr ""
 
 msgctxt "field:marketing.medium,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr ""
 
 msgctxt "field:marketing.source,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,from_date:"
 msgid "From Date"
-msgstr "Des de la data"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,period:"
 msgid "Period"
-msgstr "Període"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,to_date:"
 msgid "To Date"
-msgstr "Fins a la data"
+msgstr ""
 
 msgctxt "field:sale.reporting.marketing.context,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr ""
 
 msgctxt "field:sale.reporting.marketing.context,from_date:"
 msgid "From Date"
-msgstr "Des de la data"
+msgstr ""
 
 msgctxt "field:sale.reporting.marketing.context,period:"
 msgid "Period"
-msgstr "Període"
+msgstr ""
 
 msgctxt "field:sale.reporting.marketing.context,to_date:"
 msgid "To Date"
-msgstr "Fins a la data"
+msgstr ""
 
 msgctxt "field:sale.reporting.marketing.context,warehouse:"
 msgid "Warehouse"
-msgstr "Magatzem"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_campaign_form"
 msgid "Campaigns"
-msgstr "Campanyes"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_medium_form"
 msgid "Mediums"
-msgstr "Medis"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_sale_opportunity_reporting_marketing"
 msgid "Opportunities per Marketing"
-msgstr "Oportunitats per màrqueting"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_sale_reporting_marketing"
 msgid "Sales per Marketing"
-msgstr "Vendes per màrqueting"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_source_form"
 msgid "Sources"
-msgstr "Orígens"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_marketing_campaign"
 msgid "Marketing Campaign"
-msgstr "Campanyes de màrqueting"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_marketing_medium"
 msgid "Marketing Medium"
-msgstr "Medi de màrqueting"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_marketing_source"
 msgid "Marketing Source"
-msgstr "Orígen de màrqueting"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_parameter_name_unique"
 msgid "Name of active marketing parameter must be unique."
-msgstr "El nom del paràmetre del màrqueting ha de ser únic."
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_campaign_form"
 msgid "Campaigns"
-msgstr "Campanyes"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_medium_form"
 msgid "Mediums"
-msgstr "Medis"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_source_form"
 msgid "Sources"
-msgstr "Orígens"
+msgstr ""
 
 msgctxt "model:marketing.campaign,name:"
 msgid "Marketing Campaign"
-msgstr "Campanya de màrqueting"
+msgstr ""
 
 msgctxt "model:marketing.medium,name:"
 msgid "Marketing Medium"
-msgstr "Medi de màrqueting"
+msgstr ""
 
 msgctxt "model:marketing.source,name:"
 msgid "Marketing Source"
-msgstr "Orígen de màrqueting"
+msgstr ""
 
 msgctxt "model:sale.opportunity.reporting.marketing,name:"
 msgid "Sale Opportunity Reporting per Marketing"
-msgstr "Informe d'oportunitats de venta per màrqueting"
+msgstr ""
 
 msgctxt "model:sale.opportunity.reporting.marketing.context,name:"
 msgid "Sale Opportunity Reporting Context"
-msgstr "Context informe d'oportunitats de venda"
+msgstr ""
 
 msgctxt "model:sale.reporting.marketing,name:"
 msgid "Sale Reporting per Marketing"
-msgstr "Informe de vendes per màrqueting"
+msgstr ""
 
 msgctxt "model:sale.reporting.marketing.context,name:"
 msgid "Sale Reporting Context"
-msgstr "Context informe de vendes"
+msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.marketing.context,period:"
 msgid "Day"
-msgstr "Dia"
+msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.marketing.context,period:"
 msgid "Month"
-msgstr "Mes"
+msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.marketing.context,period:"
 msgid "Year"
-msgstr "Any"
+msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Day"
-msgstr "Dia"
+msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Month"
-msgstr "Mes"
+msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
-msgstr "Any"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
-msgstr "Campanya de màrqueting"
+msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
-msgstr "Agrupar per:"
+msgstr ""
 
 msgctxt "view:sale.opportunity:"
 msgid "Campaign"
-msgstr "Campanya"
+msgstr ""
 
 msgctxt "view:sale.opportunity:"
 msgid "Marketing Campaign"
-msgstr "Campanya de màrqueting"
+msgstr ""
 
 msgctxt "view:sale.opportunity:"
 msgid "Medium"
-msgstr "Medi"
+msgstr ""
 
 msgctxt "view:sale.opportunity:"
 msgid "Source"
-msgstr "Origen"
+msgstr ""
 
 msgctxt "view:sale.point.sale:"
 msgid "Campaign"
-msgstr "Campany"
+msgstr ""
 
 msgctxt "view:sale.point.sale:"
 msgid "Marketing Campaign"
-msgstr "Campanya de màrqueting"
+msgstr ""
 
 msgctxt "view:sale.point.sale:"
 msgid "Medium"
-msgstr "Medi"
+msgstr ""
 
 msgctxt "view:sale.point.sale:"
 msgid "Source"
-msgstr "Origen"
+msgstr ""
 
 msgctxt "view:sale.reporting.context:"
 msgid "Marketing Campaign"
-msgstr "Campanya de màrqueting"
+msgstr ""
 
 msgctxt "view:sale.reporting.marketing.context:"
 msgid "Group by:"
-msgstr "Agrupar per:"
+msgstr ""
 
 msgctxt "view:sale.sale:"
 msgid "Campaign"
-msgstr "Campanya"
+msgstr ""
 
 msgctxt "view:sale.sale:"
 msgid "Marketing Campaign"
-msgstr "Campanya de màrqueting"
+msgstr ""
 
 msgctxt "view:sale.sale:"
 msgid "Medium"
-msgstr "Medi"
+msgstr ""
 
 msgctxt "view:sale.sale:"
 msgid "Source"
-msgstr "Origen"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/cs.po` & `trytond_marketing_campaign-7.2.0/locale/es_419.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/de.po` & `trytond_marketing_campaign-7.2.0/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,54 @@
 msgid "Month"
 msgstr "Monat"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Jahr"
 
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr "Kampagne"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr "Mar­ke­ting­kam­pa­g­ne"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr "Medium"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr "Ursprung"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr "Kampagne"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr "Mar­ke­ting­kam­pa­g­ne"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr "Medium"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr "Ursprung"
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Mar­ke­ting­kam­pa­g­ne"
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr "Gruppiert nach:"
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/es.po` & `trytond_marketing_campaign-7.2.0/locale/ca.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,215 +1,255 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:marketing.campaign,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:marketing.medium,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:marketing.source,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,from_date:"
 msgid "From Date"
-msgstr "Desde la fecha"
+msgstr "Des de la data"
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,period:"
 msgid "Period"
-msgstr "Periodo"
+msgstr "Període"
 
 msgctxt "field:sale.opportunity.reporting.marketing.context,to_date:"
 msgid "To Date"
-msgstr "Hasta la fecha"
+msgstr "Fins a la data"
 
 msgctxt "field:sale.reporting.marketing.context,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:sale.reporting.marketing.context,from_date:"
 msgid "From Date"
-msgstr "Desde la fecha"
+msgstr "Des de la data"
 
 msgctxt "field:sale.reporting.marketing.context,period:"
 msgid "Period"
-msgstr "Periodo"
+msgstr "Període"
 
 msgctxt "field:sale.reporting.marketing.context,to_date:"
 msgid "To Date"
-msgstr "Hasta la fecha"
+msgstr "Fins a la data"
 
 msgctxt "field:sale.reporting.marketing.context,warehouse:"
 msgid "Warehouse"
-msgstr "Almacén"
+msgstr "Magatzem"
 
 msgctxt "model:ir.action,name:act_campaign_form"
 msgid "Campaigns"
-msgstr "Campañas"
+msgstr "Campanyes"
 
 msgctxt "model:ir.action,name:act_medium_form"
 msgid "Mediums"
-msgstr "Medios"
+msgstr "Medis"
 
 msgctxt "model:ir.action,name:act_sale_opportunity_reporting_marketing"
 msgid "Opportunities per Marketing"
-msgstr "Oportuniddes por Marketing"
+msgstr "Oportunitats per màrqueting"
 
 msgctxt "model:ir.action,name:act_sale_reporting_marketing"
 msgid "Sales per Marketing"
-msgstr "Ventas por marketing"
+msgstr "Vendes per màrqueting"
 
 msgctxt "model:ir.action,name:act_source_form"
 msgid "Sources"
-msgstr "Orígenes"
+msgstr "Orígens"
 
 msgctxt "model:ir.message,text:msg_marketing_campaign"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanyes de màrqueting"
 
 msgctxt "model:ir.message,text:msg_marketing_medium"
 msgid "Marketing Medium"
-msgstr "Medio de marketing"
+msgstr "Medi de màrqueting"
 
 msgctxt "model:ir.message,text:msg_marketing_source"
 msgid "Marketing Source"
-msgstr "Orgien de marketing"
+msgstr "Orígen de màrqueting"
 
 msgctxt "model:ir.message,text:msg_parameter_name_unique"
 msgid "Name of active marketing parameter must be unique."
-msgstr "El nombre del parámetro de marketing debe ser único."
+msgstr "El nom del paràmetre del màrqueting ha de ser únic."
 
 msgctxt "model:ir.ui.menu,name:menu_campaign_form"
 msgid "Campaigns"
-msgstr "Campañas"
+msgstr "Campanyes"
 
 msgctxt "model:ir.ui.menu,name:menu_medium_form"
 msgid "Mediums"
-msgstr "Medios"
+msgstr "Medis"
 
 msgctxt "model:ir.ui.menu,name:menu_source_form"
 msgid "Sources"
-msgstr "Orígenes"
+msgstr "Orígens"
 
 msgctxt "model:marketing.campaign,name:"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanya de màrqueting"
 
 msgctxt "model:marketing.medium,name:"
 msgid "Marketing Medium"
-msgstr "Medio marketing"
+msgstr "Medi de màrqueting"
 
 msgctxt "model:marketing.source,name:"
 msgid "Marketing Source"
-msgstr "Origen marketing"
+msgstr "Orígen de màrqueting"
 
 msgctxt "model:sale.opportunity.reporting.marketing,name:"
 msgid "Sale Opportunity Reporting per Marketing"
-msgstr "Informe de oportunidades de venta por marketing"
+msgstr "Informe d'oportunitats de venta per màrqueting"
 
 msgctxt "model:sale.opportunity.reporting.marketing.context,name:"
 msgid "Sale Opportunity Reporting Context"
-msgstr "Contexto informe oportunidades de venta"
+msgstr "Context informe d'oportunitats de venda"
 
 msgctxt "model:sale.reporting.marketing,name:"
 msgid "Sale Reporting per Marketing"
-msgstr "Informe de ventas por marketing"
+msgstr "Informe de vendes per màrqueting"
 
 msgctxt "model:sale.reporting.marketing.context,name:"
 msgid "Sale Reporting Context"
-msgstr "Contexto informe de ventas"
+msgstr "Context informe de vendes"
 
 msgctxt "selection:sale.opportunity.reporting.marketing.context,period:"
 msgid "Day"
-msgstr "Día"
+msgstr "Dia"
 
 msgctxt "selection:sale.opportunity.reporting.marketing.context,period:"
 msgid "Month"
 msgstr "Mes"
 
 msgctxt "selection:sale.opportunity.reporting.marketing.context,period:"
 msgid "Year"
-msgstr "Año"
+msgstr "Any"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Day"
-msgstr "Día"
+msgstr "Dia"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Month"
 msgstr "Mes"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
-msgstr "Año"
+msgstr "Any"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr "Campanya"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr "Campanyes de màrqueting"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr "Medi"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr "Origen"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr "Campanya"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr "Campanyes de màrqueting"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr "Medi"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr "Origen"
 
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanya de màrqueting"
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
-msgstr "Agrupar por:"
+msgstr "Agrupar per:"
 
 msgctxt "view:sale.opportunity:"
 msgid "Campaign"
-msgstr "Campaña"
+msgstr "Campanya"
 
 msgctxt "view:sale.opportunity:"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanya de màrqueting"
 
 msgctxt "view:sale.opportunity:"
 msgid "Medium"
-msgstr "Medio"
+msgstr "Medi"
 
 msgctxt "view:sale.opportunity:"
 msgid "Source"
 msgstr "Origen"
 
 msgctxt "view:sale.point.sale:"
 msgid "Campaign"
-msgstr "Campaña"
+msgstr "Campany"
 
 msgctxt "view:sale.point.sale:"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanya de màrqueting"
 
 msgctxt "view:sale.point.sale:"
 msgid "Medium"
-msgstr "Medio"
+msgstr "Medi"
 
 msgctxt "view:sale.point.sale:"
 msgid "Source"
 msgstr "Origen"
 
 msgctxt "view:sale.reporting.context:"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanya de màrqueting"
 
 msgctxt "view:sale.reporting.marketing.context:"
 msgid "Group by:"
-msgstr "Agrupar por:"
+msgstr "Agrupar per:"
 
 msgctxt "view:sale.sale:"
 msgid "Campaign"
-msgstr "Campaña"
+msgstr "Campanya"
 
 msgctxt "view:sale.sale:"
 msgid "Marketing Campaign"
-msgstr "Campaña de marketing"
+msgstr "Campanya de màrqueting"
 
 msgctxt "view:sale.sale:"
 msgid "Medium"
-msgstr "Medio"
+msgstr "Medi"
 
 msgctxt "view:sale.sale:"
 msgid "Source"
 msgstr "Origen"
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/es_419.po` & `trytond_marketing_campaign-7.2.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/et.po` & `trytond_marketing_campaign-7.2.0/locale/fa.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/fa.po` & `trytond_marketing_campaign-7.2.0/locale/fi.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/fi.po` & `trytond_marketing_campaign-7.2.0/locale/hu.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/fr.po` & `trytond_marketing_campaign-7.2.0/locale/fr.po`

 * *Files 5% similar despite different names*

```diff
@@ -146,14 +146,54 @@
 msgid "Month"
 msgstr "Mois"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Année"
 
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr "Campagne"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr "Campagne de marketing"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr "Médium"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr "Source"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr "Campagne"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr "Campagne de marketing"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr "Médium"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr "Source"
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Campagne de marketing"
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr "Groupé par :"
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/hu.po` & `trytond_marketing_campaign-7.2.0/locale/id.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/id.po` & `trytond_marketing_campaign-7.2.0/locale/it.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/it.po` & `trytond_marketing_campaign-7.2.0/locale/lo.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/lo.po` & `trytond_marketing_campaign-7.2.0/locale/lt.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/lt.po` & `trytond_marketing_campaign-7.2.0/locale/pl.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/nl.po` & `trytond_marketing_campaign-7.2.0/locale/nl.po`

 * *Files 11% similar despite different names*

```diff
@@ -146,14 +146,54 @@
 msgid "Month"
 msgstr "Maand"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Jaar"
 
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr "Campagne"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr "Marketing campagne"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr "Medium"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr "Bron"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr "Campagne"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr "Marketing campagne"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr "Medium"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr "Bron"
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Marketing campagne"
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr "Groeperen op:"
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/pl.po` & `trytond_marketing_campaign-7.2.0/locale/pt.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/pt.po` & `trytond_marketing_campaign-7.2.0/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/ro.po` & `trytond_marketing_campaign-7.2.0/locale/ru.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/ru.po` & `trytond_marketing_campaign-7.2.0/locale/tr.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/sl.po` & `trytond_marketing_campaign-7.2.0/locale/sl.po`

 * *Files 6% similar despite different names*

```diff
@@ -146,14 +146,54 @@
 msgid "Month"
 msgstr "Mesec"
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr "Leto"
 
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr "Kampanija"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr "Marketinška kampanija"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr "Medij"
+
+#, fuzzy
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr "Izvor"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr "Kampanija"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr "Marketinška kampanija"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr "Medij"
+
+#, fuzzy
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr "Izvor"
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr "Marketinška kampanija"
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr "Združi po:"
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/tr.po` & `trytond_marketing_campaign-7.2.0/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/locale/uk.po` & `trytond_marketing_campaign-7.2.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,46 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.reporting.marketing.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:marketing.automation.activity:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "Source"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Marketing Campaign"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Medium"
+msgstr ""
+
+msgctxt "view:marketing.email.message:"
+msgid "Source"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.context:"
 msgid "Marketing Campaign"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.marketing.context:"
 msgid "Group by:"
 msgstr ""
```

### Comparing `trytond_marketing_campaign-7.0.1/marketing.xml` & `trytond_marketing_campaign-7.2.0/marketing.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_marketing_campaign-7.0.1/marketing.xml` & `trytond_marketing_campaign-7.2.0/marketing.xml`

```diff
@@ -75,8 +75,22 @@
     <record model="ir.action.act_window.view" id="act_source_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="source_view_form"/>
       <field name="act_window" ref="act_source_form"/>
     </record>
     <menuitem parent="marketing.menu_marketing" action="act_source_form" sequence="50" id="menu_source_form"/>
   </data>
+  <data depends="marketing_email">
+    <record model="ir.ui.view" id="email_message_view_form">
+      <field name="model">marketing.email.message</field>
+      <field name="inherit" ref="marketing_email.email_message_view_form"/>
+      <field name="name">campaign_mixin_form</field>
+    </record>
+  </data>
+  <data depends="marketing_automation">
+    <record model="ir.ui.view" id="automation_activity_view_form">
+      <field name="model">marketing.automation.activity</field>
+      <field name="inherit" ref="marketing_automation.activity_view_form"/>
+      <field name="name">campaign_mixin_form</field>
+    </record>
+  </data>
 </tryton>
```

### Comparing `trytond_marketing_campaign-7.0.1/message.xml` & `trytond_marketing_campaign-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/sale.py` & `trytond_marketing_campaign-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/sale.xml` & `trytond_marketing_campaign-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/sale_opportunity_reporting.py` & `trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/sale_opportunity_reporting.xml` & `trytond_marketing_campaign-7.2.0/sale_opportunity_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/sale_reporting.py` & `trytond_marketing_campaign-7.2.0/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/sale_reporting.xml` & `trytond_marketing_campaign-7.2.0/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/setup.py` & `trytond_marketing_campaign-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,31 +48,34 @@
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
+    get_require_version('trytond_marketing_email'),
+    get_require_version('trytond_marketing_automation'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_sale_opportunity'),
     get_require_version('trytond_sale_point'),
+    get_require_version('trytond_web_shortener'),
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module to manage marketing campaign',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-marketing-campaign'),
+            'https://docs.tryton.org/modules-marketing-campaign'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton marketing campaign sale UTM',
     package_dir={'trytond.modules.marketing_campaign': '.'},
     packages=(
         ['trytond.modules.marketing_campaign']
```

### Comparing `trytond_marketing_campaign-7.0.1/tests/scenario_marketing_campaign_sale.rst` & `trytond_marketing_campaign-7.2.0/tests/scenario_marketing_campaign_sale.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 Marketing Campaign Sale Scenario
 ================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['marketing_campaign', 'sale', 'sale_opportunity'])
 
     >>> Category = Model.get('product.category')
@@ -100,21 +98,21 @@
     >>> opportunity.marketing_medium.name
     'web'
     >>> opportunity.marketing_source
 
     >>> opportunity.click('opportunity')
     >>> opportunity.state
     'opportunity'
-    >>> opportunity.click('convert')
+    >>> sale, = opportunity.click('convert')
     >>> opportunity.state
     'converted'
+    >>> assertEqual(opportunity.sales, [sale])
 
 Check and confirm sale::
 
-    >>> sale, = opportunity.sales
     >>> sale.marketing_campaign.name
     'campaign'
     >>> sale.marketing_medium.name
     'web'
     >>> sale.marketing_source
     >>> sale.click('quote')
     >>> sale.click('confirm')
@@ -140,36 +138,35 @@
 
     >>> sale.click('quote')
     >>> sale.click('confirm')
 
 Check sale reporting::
 
     >>> report, = ReportingMain.find([])
-    >>> report.revenue == Decimal(110)
-    True
+    >>> report.revenue
+    Decimal('110.00')
 
     >>> with config.set_context(marketing_medium=sale.marketing_medium.id):
     ...     report, = ReportingMain.find([])
-    >>> report.revenue == Decimal(10)
-    True
+    >>> report.revenue
+    Decimal('10.00')
 
     >>> report, = ReportingMarketing.find([])
-    >>> report.revenue == Decimal(110)
-    True
+    >>> report.revenue
+    Decimal('110.00')
     >>> report.marketing_campaign
     >>> report.marketing_medium
     >>> report.marketing_source
 
     >>> with config.set_context(group_by_marketing_medium=True):
     ...     reports = ReportingMarketing.find([])
     >>> len(reports)
     2
-    >>> sorted((r.marketing_medium.name, r.revenue) for r in reports) == (
-    ...     [('phone', Decimal(10)), ('web', Decimal(100))])
-    True
+    >>> sorted((r.marketing_medium.name, r.revenue) for r in reports)
+    [('phone', Decimal('10.00')), ('web', Decimal('100.00'))]
 
     >>> with config.set_context(
     ...         group_by_marketing_campaign=True,
     ...         group_by_marketing_medium=True,
     ...         ):
     ...     reports = ReportingMarketing.find([])
     >>> len(reports)
```

### Comparing `trytond_marketing_campaign-7.0.1/tox.ini` & `trytond_marketing_campaign-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/PKG-INFO` & `trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-marketing-campaign
-Version: 7.0.1
+Name: trytond_marketing_campaign
+Version: 7.2.0
 Summary: Tryton module to manage marketing campaign
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-marketing-campaign
+Project-URL: Documentation, https://docs.tryton.org/modules-marketing-campaign
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing campaign sale UTM
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_marketing<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_marketing<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_opportunity<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_marketing_email<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_marketing_automation<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_opportunity<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_web_shortener<7.3,>=7.2; extra == "test"
 
 #########################
 Marketing Campaign Module
 #########################
 
 The *Marketing Campaign Module* helps collecting data about marketing campaigns.
```

### Comparing `trytond_marketing_campaign-7.0.1/trytond_marketing_campaign.egg-info/SOURCES.txt` & `trytond_marketing_campaign-7.2.0/trytond_marketing_campaign.egg-info/SOURCES.txt`

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
 marketing.py
@@ -13,25 +12,27 @@
 sale_opportunity_reporting.py
 sale_opportunity_reporting.xml
 sale_reporting.py
 sale_reporting.xml
 setup.py
 tox.ini
 tryton.cfg
+web.py
 ./__init__.py
 ./marketing.py
 ./marketing.xml
 ./message.xml
 ./sale.py
 ./sale.xml
 ./sale_opportunity_reporting.py
 ./sale_opportunity_reporting.xml
 ./sale_reporting.py
 ./sale_reporting.xml
 ./tryton.cfg
+./web.py
 ./locale/bg.po
 ./locale/ca.po
 ./locale/cs.po
 ./locale/de.po
 ./locale/es.po
 ./locale/es_419.po
 ./locale/et.po
```

### Comparing `trytond_marketing_campaign-7.0.1/view/campaign_mixin_form.xml` & `trytond_marketing_campaign-7.2.0/view/campaign_mixin_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/view/sale_opportunity_reporting_context_form.xml` & `trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/view/sale_opportunity_reporting_marketing_context_form.xml` & `trytond_marketing_campaign-7.2.0/view/sale_opportunity_reporting_marketing_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/view/sale_reporting_context_form.xml` & `trytond_marketing_campaign-7.2.0/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-7.0.1/view/sale_reporting_marketing_context_form.xml` & `trytond_marketing_campaign-7.2.0/view/sale_reporting_marketing_context_form.xml`

 * *Files identical despite different names*

