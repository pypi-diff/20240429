# Comparing `tmp/trytond_production_routing-7.0.0.tar.gz` & `tmp/trytond_production_routing-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_routing-7.0.0.tar", last modified: Mon Oct 30 17:33:55 2023, max compression
+gzip compressed data, was "trytond_production_routing-7.2.0.tar", last modified: Mon Apr 29 15:44:15 2024, max compression
```

## Comparing `trytond_production_routing-7.0.0.tar` & `trytond_production_routing-7.2.0.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:55.283268 trytond_production_routing-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:11.000000 trytond_production_routing-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1477 2023-10-30 17:09:42.000000 trytond_production_routing-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-10-30 17:09:42.000000 trytond_production_routing-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2944 2023-10-30 17:33:55.283268 trytond_production_routing-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:55.279935 trytond_production_routing-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:11.000000 trytond_production_routing-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:11.000000 trytond_production_routing-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:55.276601 trytond_production_routing-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1661 2023-10-30 16:47:45.000000 trytond_production_routing-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1779 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1691 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1506 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1708 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1799 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1653 2023-10-30 16:47:45.000000 trytond_production_routing-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1686 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1712 2023-10-28 12:11:24.000000 trytond_production_routing-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1582 2023-10-07 15:40:36.000000 trytond_production_routing-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_production_routing-7.0.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1650 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/routing.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5490 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/routing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:33:55.283268 trytond_production_routing-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4529 2023-10-27 17:38:49.000000 trytond_production_routing-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:55.276601 trytond_production_routing-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2200 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/tests/scenario_stock_supply_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_production_routing-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-10-30 17:09:39.000000 trytond_production_routing-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:55.279935 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2944 2023-10-30 17:33:54.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2375 2023-10-30 17:33:55.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:54.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:33:54.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2023-10-30 17:33:54.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:33:54.000000 trytond_production_routing-7.0.0/trytond_production_routing.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:55.279935 trytond_production_routing-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-08-13 15:26:13.000000 trytond_production_routing-7.0.0/view/operation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/view/operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/product_bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/product_bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-07 17:14:58.000000 trytond_production_routing-7.0.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/production_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/production_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/production_lead_time_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/routing_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/view/routing_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:21.000000 trytond_production_routing-7.0.0/view/routing_step_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/view/routing_step_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_production_routing-7.0.0/view/routing_step_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:15.530098 trytond_production_routing-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1578 2024-04-29 15:22:40.000000 trytond_production_routing-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2024-04-29 15:22:40.000000 trytond_production_routing-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-29 15:44:15.530098 trytond_production_routing-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:15.526765 trytond_production_routing-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_production_routing-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:18.000000 trytond_production_routing-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:15.526765 trytond_production_routing-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1661 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1710 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1779 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1691 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1697 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1710 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1506 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1710 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1708 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1746 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1799 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1653 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1686 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-04-27 16:43:25.000000 trytond_production_routing-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1582 2024-02-04 18:51:26.000000 trytond_production_routing-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_production_routing-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1650 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/routing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5398 2024-04-27 16:30:39.000000 trytond_production_routing-7.2.0/routing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:15.530098 trytond_production_routing-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4529 2024-03-17 11:01:36.000000 trytond_production_routing-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:15.526765 trytond_production_routing-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2201 2024-04-22 12:14:36.000000 trytond_production_routing-7.2.0/tests/scenario_stock_supply_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:18.000000 trytond_production_routing-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-04-29 15:22:36.000000 trytond_production_routing-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:15.530098 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-29 15:44:15.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2024-04-29 15:44:15.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:15.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:44:15.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-04-29 15:44:15.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:15.000000 trytond_production_routing-7.2.0/trytond_production_routing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:15.530098 trytond_production_routing-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-01-27 09:58:52.000000 trytond_production_routing-7.2.0/view/operation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/view/operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/product_bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/product_bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-02-04 18:51:26.000000 trytond_production_routing-7.2.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/production_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/production_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/production_lead_time_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/routing_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/view/routing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:21.000000 trytond_production_routing-7.2.0/view/routing_step_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/view/routing_step_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_production_routing-7.2.0/view/routing_step_list_sequence.xml
```

### Comparing `trytond_production_routing-7.0.0/CHANGELOG` & `trytond_production_routing-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_production_routing-7.0.0/COPYRIGHT` & `trytond_production_routing-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2023 Cédric Krier.
-Copyright (C) 2015-2023 B2CK SPRL.
+Copyright (C) 2015-2024 Cédric Krier.
+Copyright (C) 2015-2024 B2CK SPRL.
 Copyright (C) 2013-2015 NaN·tic.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_production_routing-7.0.0/LICENSE` & `trytond_production_routing-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/PKG-INFO` & `trytond_production_routing-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_production_routing
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for production routing
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
@@ -49,19 +49,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply_production<7.3,>=7.2; extra == "test"
 
 Production Routing Module
 #########################
 
 The production routing module defines the routings for production: Routing,
 Step and Operation.
```

### Comparing `trytond_production_routing-7.0.0/__init__.py` & `trytond_production_routing-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/doc/conf.py` & `trytond_production_routing-7.2.0/doc/conf.py`

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

### Comparing `trytond_production_routing-7.0.0/locale/bg.po` & `trytond_production_routing-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/ca.po` & `trytond_production_routing-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/cs.po` & `trytond_production_routing-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/de.po` & `trytond_production_routing-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/es.po` & `trytond_production_routing-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/es_419.po` & `trytond_production_routing-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/et.po` & `trytond_production_routing-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/fa.po` & `trytond_production_routing-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/fi.po` & `trytond_production_routing-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/fr.po` & `trytond_production_routing-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/hu.po` & `trytond_production_routing-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/id.po` & `trytond_production_routing-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/it.po` & `trytond_production_routing-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/lo.po` & `trytond_production_routing-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/lt.po` & `trytond_production_routing-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/nl.po` & `trytond_production_routing-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/pl.po` & `trytond_production_routing-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/pt.po` & `trytond_production_routing-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/ro.po` & `trytond_production_routing-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/ru.po` & `trytond_production_routing-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/sl.po` & `trytond_production_routing-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/tr.po` & `trytond_production_routing-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/uk.po` & `trytond_production_routing-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/locale/zh_CN.po` & `trytond_production_routing-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/product.py` & `trytond_production_routing-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/product.xml` & `trytond_production_routing-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/production.py` & `trytond_production_routing-7.2.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/routing.py` & `trytond_production_routing-7.2.0/routing.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/routing.xml` & `trytond_production_routing-7.2.0/routing.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_production_routing-7.0.0/routing.xml` & `trytond_production_routing-7.2.0/routing.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_routing_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="routing_view_form"/>
       <field name="act_window" ref="act_routing_list"/>
     </record>
     <menuitem parent="production.menu_configuration" action="act_routing_list" sequence="20" id="menu_routing_list"/>
     <record model="ir.model.access" id="access_routing">
-      <field name="model" search="[('model', '=', 'production.routing')]"/>
+      <field name="model">production.routing</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_routing_admin">
-      <field name="model" search="[('model', '=', 'production.routing')]"/>
+      <field name="model">production.routing</field>
       <field name="group" ref="production.group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="operation_view_list">
@@ -65,22 +65,22 @@
     <record model="ir.action.act_window.view" id="act_operation_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="operation_view_form"/>
       <field name="act_window" ref="act_operation_list"/>
     </record>
     <menuitem parent="menu_routing_list" action="act_operation_list" sequence="10" id="menu_operation_list"/>
     <record model="ir.model.access" id="access_operation">
-      <field name="model" search="[('model', '=', 'production.routing.operation')]"/>
+      <field name="model">production.routing.operation</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_operation_admin">
-      <field name="model" search="[('model', '=', 'production.routing.operation')]"/>
+      <field name="model">production.routing.operation</field>
       <field name="group" ref="production.group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="routing_step_view_list">
```

### Comparing `trytond_production_routing-7.0.0/setup.py` & `trytond_production_routing-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/tests/scenario_stock_supply_production.rst` & `trytond_production_routing-7.2.0/tests/scenario_stock_supply_production.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ===========================
 Production Request Scenario
 ===========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['stock_supply_production', 'production_routing'])
 
 Create company::
@@ -71,9 +71,8 @@
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
 
 There is now a production request with the routing::
 
     >>> Production = Model.get('production')
     >>> production, = Production.find([])
-    >>> production.routing == routing
-    True
+    >>> assertEqual(production.routing, routing)
```

### Comparing `trytond_production_routing-7.0.0/tox.ini` & `trytond_production_routing-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-7.0.0/trytond_production_routing.egg-info/PKG-INFO` & `trytond_production_routing-7.2.0/trytond_production_routing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-production-routing
-Version: 7.0.0
+Name: trytond_production_routing
+Version: 7.2.0
 Summary: Tryton module for production routing
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
@@ -49,19 +49,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply_production<7.3,>=7.2; extra == "test"
 
 Production Routing Module
 #########################
 
 The production routing module defines the routings for production: Routing,
 Step and Operation.
```

### Comparing `trytond_production_routing-7.0.0/trytond_production_routing.egg-info/SOURCES.txt` & `trytond_production_routing-7.2.0/trytond_production_routing.egg-info/SOURCES.txt`

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
 product.py
```

### Comparing `trytond_production_routing-7.0.0/view/routing_form.xml` & `trytond_production_routing-7.2.0/view/routing_form.xml`

 * *Files identical despite different names*

