# Comparing `tmp/trytond_sale_product_recommendation_association_rule-7.0.0.tar.gz` & `tmp/trytond_sale_product_recommendation_association_rule-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_product_recommendation_association_rule-7.0.0.tar", last modified: Mon Oct 30 17:39:19 2023, max compression
+gzip compressed data, was "trytond_sale_product_recommendation_association_rule-7.2.0.tar", last modified: Mon Apr 29 15:49:05 2024, max compression
```

## Comparing `trytond_sale_product_recommendation_association_rule-7.0.0.tar` & `trytond_sale_product_recommendation_association_rule-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:19.168146 trytond_sale_product_recommendation_association_rule-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2023-10-22 17:23:20.000000 trytond_sale_product_recommendation_association_rule-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:12:49.000000 trytond_sale_product_recommendation_association_rule-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:12:49.000000 trytond_sale_product_recommendation_association_rule-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3094 2023-10-30 17:39:19.168146 trytond_sale_product_recommendation_association_rule-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:19.164813 trytond_sale_product_recommendation_association_rule-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-10-22 17:23:20.000000 trytond_sale_product_recommendation_association_rule-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1067 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:20.000000 trytond_sale_product_recommendation_association_rule-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:19.164813 trytond_sale_product_recommendation_association_rule-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4536 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4546 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4534 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4586 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4342 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-28 12:11:25.000000 trytond_sale_product_recommendation_association_rule-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10390 2023-06-10 11:39:56.000000 trytond_sale_product_recommendation_association_rule-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2785 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:39:19.168146 trytond_sale_product_recommendation_association_rule-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5013 2023-10-27 17:38:49.000000 trytond_sale_product_recommendation_association_rule-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:19.164813 trytond_sale_product_recommendation_association_rule-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4782 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/tests/scenario_sale_product_recommendation_association_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_product_recommendation_association_rule-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-30 17:12:46.000000 trytond_sale_product_recommendation_association_rule-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:19.168146 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3094 2023-10-30 17:39:18.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-10-30 17:39:19.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:39:18.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2023-10-30 17:39:18.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-10-30 17:39:18.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:39:18.000000 trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:19.164813 trytond_sale_product_recommendation_association_rule-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      862 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/view/product_association_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.0.0/view/product_association_rule_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:26:07.000000 trytond_sale_product_recommendation_association_rule-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:26:07.000000 trytond_sale_product_recommendation_association_rule-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:05.622511 trytond_sale_product_recommendation_association_rule-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3107 2024-04-27 16:30:39.000000 trytond_sale_product_recommendation_association_rule-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1067 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:28.000000 trytond_sale_product_recommendation_association_rule-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4536 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4546 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4534 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4586 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4342 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2024-04-27 16:43:26.000000 trytond_sale_product_recommendation_association_rule-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10390 2023-06-10 11:39:56.000000 trytond_sale_product_recommendation_association_rule-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-27 16:30:39.000000 trytond_sale_product_recommendation_association_rule-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5004 2024-04-27 16:30:39.000000 trytond_sale_product_recommendation_association_rule-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4759 2024-04-22 12:14:36.000000 trytond_sale_product_recommendation_association_rule-7.2.0/tests/scenario_sale_product_recommendation_association_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:28.000000 trytond_sale_product_recommendation_association_rule-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-29 15:26:03.000000 trytond_sale_product_recommendation_association_rule-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-29 15:49:05.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1963 2024-04-29 15:49:05.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:05.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      126 2024-04-29 15:49:05.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-29 15:49:05.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:05.000000 trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:05.625844 trytond_sale_product_recommendation_association_rule-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      862 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/view/product_association_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_sale_product_recommendation_association_rule-7.2.0/view/product_association_rule_list.xml
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/COPYRIGHT` & `trytond_sale_product_recommendation_association_rule-7.2.0/COPYRIGHT`

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

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/LICENSE` & `trytond_sale_product_recommendation_association_rule-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/PKG-INFO` & `trytond_sale_product_recommendation_association_rule-7.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale_product_recommendation_association_rule
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to learn association rule for recommendation
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-product-recommendation-association-rule
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-product-recommendation-association-rule
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale product recommendation association rule learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: efficient-apriori
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_product_recommendation<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_product_recommendation<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
 
 ###################################################
 Sale Product Recommendation Association Rule Module
 ###################################################
 
 The *Sale Product Recommendation Association Rule Module* implements
 recommendation based on `association rule learning
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/__init__.py` & `trytond_sale_product_recommendation_association_rule-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/doc/conf.py` & `trytond_sale_product_recommendation_association_rule-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/doc/design.rst` & `trytond_sale_product_recommendation_association_rule-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/doc/usage.rst` & `trytond_sale_product_recommendation_association_rule-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/bg.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/ca.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/cs.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/de.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/es.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/es_419.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/et.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/fa.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/fi.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/fr.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/hu.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/id.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/it.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/lo.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/lt.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/nl.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/pl.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/pt.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/ro.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/ru.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/sl.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/tr.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/uk.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/locale/zh_CN.po` & `trytond_sale_product_recommendation_association_rule-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/sale.py` & `trytond_sale_product_recommendation_association_rule-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/sale.xml` & `trytond_sale_product_recommendation_association_rule-7.2.0/sale.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/sale.xml` & `trytond_sale_product_recommendation_association_rule-7.2.0/sale.xml`

```diff
@@ -30,15 +30,15 @@
     <record model="ir.action.act_window.view" id="act_product_association_rule_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="product_association_rule_view_form"/>
       <field name="act_window" ref="act_product_association_rule_form"/>
     </record>
     <menuitem parent="sale.menu_product" action="act_product_association_rule_form" sequence="50" id="menu_product_association_rule_form"/>
     <record model="ir.model.access" id="access_product_association_rule">
-      <field name="model" search="[('model', '=', 'sale.product.association.rule')]"/>
+      <field name="model">sale.product.association.rule</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.cron" id="cron_product_association_rule_compute">
       <field name="method">sale.product.association.rule|compute</field>
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/setup.py` & `trytond_sale_product_recommendation_association_rule-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-sale-product-recommendation-association-rule'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale product recommendation association rule learning',
     package_dir={
         'trytond.modules.sale_product_recommendation_association_rule': '.',
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/tests/scenario_sale_product_recommendation_association_rule.rst` & `trytond_sale_product_recommendation_association_rule-7.2.0/tests/scenario_sale_product_recommendation_association_rule.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 =====================================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate modules::
 
     >>> config = activate_modules('sale_product_recommendation_association_rule')
 
     >>> Cron = Model.get('ir.cron')
     >>> Party = Model.get('party.party')
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/tox.ini` & `trytond_sale_product_recommendation_association_rule-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/PKG-INFO` & `trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-sale-product-recommendation-association-rule
-Version: 7.0.0
+Name: trytond_sale_product_recommendation_association_rule
+Version: 7.2.0
 Summary: Tryton module to learn association rule for recommendation
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-product-recommendation-association-rule
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-product-recommendation-association-rule
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale product recommendation association rule learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: efficient-apriori
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_product_recommendation<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_product_recommendation<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
 
 ###################################################
 Sale Product Recommendation Association Rule Module
 ###################################################
 
 The *Sale Product Recommendation Association Rule Module* implements
 recommendation based on `association rule learning
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/trytond_sale_product_recommendation_association_rule.egg-info/SOURCES.txt` & `trytond_sale_product_recommendation_association_rule-7.2.0/trytond_sale_product_recommendation_association_rule.egg-info/SOURCES.txt`

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
 ir.py
```

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/view/configuration_form.xml` & `trytond_sale_product_recommendation_association_rule-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_recommendation_association_rule-7.0.0/view/product_association_rule_form.xml` & `trytond_sale_product_recommendation_association_rule-7.2.0/view/product_association_rule_form.xml`

 * *Files identical despite different names*

