# Comparing `tmp/trytond_account_asset-7.0.0.tar.gz` & `tmp/trytond_account_asset-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_asset-7.0.0.tar", last modified: Mon Oct 30 17:18:11 2023, max compression
+gzip compressed data, was "trytond_account_asset-7.2.0.tar", last modified: Mon Apr 29 15:31:37 2024, max compression
```

## Comparing `trytond_account_asset-7.0.0.tar` & `trytond_account_asset-7.2.0.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:11.538767 trytond_account_asset-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-22 17:22:47.000000 trytond_account_asset-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2023-10-30 17:00:46.000000 trytond_account_asset-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:00:46.000000 trytond_account_asset-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3611 2023-10-30 17:18:11.538767 trytond_account_asset-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1351 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7220 2023-08-13 15:26:13.000000 trytond_account_asset-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    43075 2023-08-13 15:26:13.000000 trytond_account_asset-7.0.0/asset.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11622 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/asset.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    61964 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/asset_table.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:11.535433 trytond_account_asset-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-10-22 17:22:47.000000 trytond_account_asset-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:47.000000 trytond_account_asset-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3090 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:11.532100 trytond_account_asset-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    19721 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20940 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18189 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21368 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21049 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19616 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20298 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22250 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18189 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21098 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18853 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18548 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19852 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23118 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18567 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20824 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18955 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20787 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17768 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19780 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19968 2023-10-30 16:47:45.000000 trytond_account_asset-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19753 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17526 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18533 2023-10-28 12:11:19.000000 trytond_account_asset-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1552 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3101 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1766 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1751 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3519 2023-08-13 15:26:13.000000 trytond_account_asset-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1111 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:18:11.538767 trytond_account_asset-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4505 2023-10-27 17:38:49.000000 trytond_account_asset-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:11.532100 trytond_account_asset-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8537 2023-06-10 11:39:56.000000 trytond_account_asset-7.0.0/tests/scenario_account_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4600 2023-06-10 11:39:56.000000 trytond_account_asset-7.0.0/tests/scenario_account_asset_depreciated.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3717 2023-10-24 07:56:52.000000 trytond_account_asset-7.0.0/tests/scenario_purchase_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1645 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-06-10 11:39:56.000000 trytond_account_asset-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_asset-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-10-30 17:00:43.000000 trytond_account_asset-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:11.535433 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3611 2023-10-30 17:18:10.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3220 2023-10-30 17:18:11.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:18:10.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:18:10.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:18:10.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:18:10.000000 trytond_account_asset-7.0.0/trytond_account_asset.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:18:11.535433 trytond_account_asset-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/asset_create_moves_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2342 2023-10-07 15:40:36.000000 trytond_account_asset-7.0.0/view/asset_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/asset_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/asset_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      532 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/asset_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      617 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/view/asset_update_show_depreciation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/asset_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/view/print_depreciation_table_start.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:14.000000 trytond_account_asset-7.0.0/view/revision_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:20.000000 trytond_account_asset-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2529 2024-04-29 15:12:43.000000 trytond_account_asset-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:12:43.000000 trytond_account_asset-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3611 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1351 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7220 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    43075 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/asset.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11392 2024-04-27 16:30:39.000000 trytond_account_asset-7.2.0/asset.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    61964 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/asset_table.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.363261 trytond_account_asset-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_account_asset-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account_asset-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.366594 trytond_account_asset-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19721 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20940 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18189 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21368 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21049 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19616 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20298 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22250 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18189 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21098 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18853 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18548 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19852 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23118 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18567 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20824 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18955 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20787 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20474 2024-04-29 13:17:17.000000 trytond_account_asset-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19780 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19968 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19753 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17526 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18533 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3101 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1766 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1751 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3519 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1111 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4505 2024-03-17 11:01:36.000000 trytond_account_asset-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.366594 trytond_account_asset-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8424 2024-04-22 12:14:36.000000 trytond_account_asset-7.2.0/tests/scenario_account_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4517 2024-04-22 12:14:36.000000 trytond_account_asset-7.2.0/tests/scenario_account_asset_depreciated.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3701 2024-04-22 12:14:36.000000 trytond_account_asset-7.2.0/tests/scenario_purchase_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1645 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account_asset-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-29 15:12:39.000000 trytond_account_asset-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3611 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3202 2024-04-29 15:31:37.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_create_moves_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2342 2024-02-04 18:51:26.000000 trytond_account_asset-7.2.0/view/asset_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      532 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      617 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/asset_update_show_depreciation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/print_depreciation_table_start.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/revision_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/template_form.xml
```

### Comparing `trytond_account_asset-7.0.0/CHANGELOG` & `trytond_account_asset-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_account_asset-7.0.0/COPYRIGHT` & `trytond_account_asset-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Copyright (C) 2012-2023 Nicolas Évrard.
-Copyright (C) 2012-2023 Cédric Krier.
+Copyright (C) 2012-2024 Cédric Krier.
 Copyright (C) 2012-2013 Bertrand Chenal.
-Copyright (C) 2012-2023 B2CK SPRL.
+Copyright (C) 2012-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_asset-7.0.0/LICENSE` & `trytond_account_asset-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/PKG-INFO` & `trytond_account_asset-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_asset
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for assets management
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
@@ -50,22 +50,22 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Account Asset Module
 ####################
 
 The account_asset module adds the depreciation of fixed assets.
 
 Asset
```

### Comparing `trytond_account_asset-7.0.0/README.rst` & `trytond_account_asset-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/__init__.py` & `trytond_account_asset-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/account.py` & `trytond_account_asset-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/account.xml` & `trytond_account_asset-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/asset.py` & `trytond_account_asset-7.2.0/asset.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/asset.xml` & `trytond_account_asset-7.2.0/asset.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_account_asset-7.0.0/asset.xml` & `trytond_account_asset-7.2.0/asset.xml`

```diff
@@ -73,74 +73,74 @@
     </record>
     <record model="ir.sequence" id="sequence_asset">
       <field name="name">Asset</field>
       <field name="sequence_type" ref="sequence_type_asset"/>
     </record>
     <record model="ir.rule.group" id="rule_group_asset_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
+      <field name="model">account.asset</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_asset_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_asset_companies"/>
     </record>
     <record model="ir.model.access" id="access_asset">
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
+      <field name="model">account.asset</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_asset_account_admin">
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
+      <field name="model">account.asset</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_asset_account">
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
+      <field name="model">account.asset</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="asset_draft_button">
+      <field name="model">account.asset</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
     </record>
     <record model="ir.model.button" id="asset_close_button">
+      <field name="model">account.asset</field>
       <field name="name">close</field>
       <field name="string">Close</field>
       <field name="confirm">Are you sure you want to close the asset?</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
     </record>
     <record model="ir.model.button" id="asset_run_button">
+      <field name="model">account.asset</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
     </record>
     <record model="ir.model.button" id="asset_create_lines_button">
+      <field name="model">account.asset</field>
       <field name="name">create_lines</field>
       <field name="string">Create Lines</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
     </record>
     <record model="ir.model.button" id="asset_clear_lines_button">
+      <field name="model">account.asset</field>
       <field name="name">clear_lines</field>
       <field name="string">Clear Lines</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
     </record>
     <record model="ir.model.button" id="asset_update_button">
+      <field name="model">account.asset</field>
       <field name="name">update</field>
       <field name="string">Update Asset</field>
-      <field name="model" search="[('model', '=', 'account.asset')]"/>
     </record>
     <record model="ir.ui.view" id="asset_line_view_form">
       <field name="model">account.asset.line</field>
       <field name="type">form</field>
       <field name="name">asset_line_form</field>
     </record>
     <record model="ir.ui.view" id="asset_line_view_tree">
```

### Comparing `trytond_account_asset-7.0.0/asset_table.fodt` & `trytond_account_asset-7.2.0/asset_table.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/doc/conf.py` & `trytond_account_asset-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_asset-7.0.0/doc/index.rst` & `trytond_account_asset-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/invoice.py` & `trytond_account_asset-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/bg.po` & `trytond_account_asset-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/ca.po` & `trytond_account_asset-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/cs.po` & `trytond_account_asset-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/de.po` & `trytond_account_asset-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/es.po` & `trytond_account_asset-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/es_419.po` & `trytond_account_asset-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/et.po` & `trytond_account_asset-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/fa.po` & `trytond_account_asset-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/fi.po` & `trytond_account_asset-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/fr.po` & `trytond_account_asset-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/hu.po` & `trytond_account_asset-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/id.po` & `trytond_account_asset-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/it.po` & `trytond_account_asset-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/lo.po` & `trytond_account_asset-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/lt.po` & `trytond_account_asset-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/nl.po` & `trytond_account_asset-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/pl.po` & `trytond_account_asset-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/pt.po` & `trytond_account_asset-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/ro.po` & `trytond_account_asset-7.2.0/locale/uk.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,fixed_asset:"
 msgid "Fixed Asset"
-msgstr "Mijloc Fix"
+msgstr ""
 
 msgctxt "field:account.account.type.template,fixed_asset:"
 msgid "Fixed Asset"
 msgstr ""
 
 msgctxt "field:account.asset,account_journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr ""
 
 msgctxt "field:account.asset,comment:"
 msgid "Comment"
-msgstr "Cometariu"
+msgstr ""
 
 msgctxt "field:account.asset,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.asset,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
 msgctxt "field:account.asset,customer_invoice_line:"
 msgid "Customer Invoice Line"
 msgstr ""
 
 msgctxt "field:account.asset,depreciated_amount:"
 msgid "Depreciated Amount"
@@ -49,27 +48,27 @@
 
 msgctxt "field:account.asset,frequency:"
 msgid "Frequency"
 msgstr ""
 
 msgctxt "field:account.asset,lines:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "field:account.asset,move:"
 msgid "Account Move"
-msgstr "Mişcare Cont"
+msgstr ""
 
 msgctxt "field:account.asset,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:account.asset,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:account.asset,purchase_date:"
 msgid "Purchase Date"
 msgstr ""
 
 msgctxt "field:account.asset,quantity:"
 msgid "Quantity"
@@ -113,15 +112,15 @@
 
 msgctxt "field:account.asset-update-account.move,move:"
 msgid "Move"
 msgstr ""
 
 msgctxt "field:account.asset.create_moves.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.asset.line,accumulated_depreciation:"
 msgid "Accumulated Depreciation"
 msgstr ""
 
 msgctxt "field:account.asset.line,acquired_value:"
 msgid "Acquired Value"
@@ -131,61 +130,57 @@
 msgid "Actual Value"
 msgstr ""
 
 msgctxt "field:account.asset.line,asset:"
 msgid "Asset"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.asset.line,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
 msgctxt "field:account.asset.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.asset.line,depreciable_basis:"
 msgid "Depreciable Basis"
 msgstr ""
 
 msgctxt "field:account.asset.line,depreciation:"
 msgid "Depreciation"
 msgstr ""
 
 msgctxt "field:account.asset.line,move:"
 msgid "Account Move"
-msgstr "Mişcare Cont"
+msgstr ""
 
 msgctxt "field:account.asset.print_depreciation_table.start,end_date:"
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:account.asset.print_depreciation_table.start,start_date:"
 msgid "Start Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.asset.revision,asset:"
 msgid "Asset"
-msgstr "Mijloc Fix"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.asset.revision,currency:"
 msgid "Currency"
-msgstr "Zecimale valută"
+msgstr ""
 
 msgctxt "field:account.asset.revision,description:"
 msgid "Description"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.asset.revision,end_date:"
 msgid "End Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.asset.revision,origin:"
 msgid "Origin"
 msgstr ""
 
 msgctxt "field:account.asset.revision,residual_value:"
 msgid "Residual Value"
@@ -193,23 +188,23 @@
 
 msgctxt "field:account.asset.revision,value:"
 msgid "Asset Value"
 msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,counterpart_account:"
 msgid "Counterpart Account"
 msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,depreciation_account:"
 msgid "Depreciation Account"
 msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,latest_move_date:"
 msgid "Latest Move Date"
@@ -241,31 +236,31 @@
 
 msgctxt "field:account.configuration.asset_date,asset_bymonthday:"
 msgid "Day of the Month"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_date,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.configuration.asset_frequency,asset_frequency:"
 msgid "Asset Depreciation Frequency"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_frequency,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.configuration.asset_sequence,asset_sequence:"
 msgid "Asset Reference Sequence"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_sequence,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.invoice.line,asset:"
 msgid "Asset"
 msgstr ""
 
 msgctxt "field:account.invoice.line,is_assets_depreciable:"
 msgid "Is Assets depreciable"
@@ -419,15 +414,15 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_closed"
 msgid "Closed"
-msgstr "Închis"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_draft"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_running"
 msgid "Running"
@@ -603,15 +598,15 @@
 
 msgctxt "selection:account.asset,frequency:"
 msgid "Yearly"
 msgstr ""
 
 msgctxt "selection:account.asset,state:"
 msgid "Closed"
-msgstr "Închis"
+msgstr ""
 
 msgctxt "selection:account.asset,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:account.asset,state:"
 msgid "Running"
@@ -735,15 +730,15 @@
 
 msgctxt "view:account.asset.create_moves.start:"
 msgid "Create Assets Moves up to"
 msgstr ""
 
 msgctxt "view:account.asset:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "view:account.asset:"
 msgid "Other Info"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Asset"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_asset-7.0.0/locale/ru.po` & `trytond_account_asset-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/sl.po` & `trytond_account_asset-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/tr.po` & `trytond_account_asset-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/locale/uk.po` & `trytond_account_asset-7.2.0/locale/zh_CN.po`

 * *Files 9% similar despite different names*

```diff
@@ -22,25 +22,28 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.asset,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset,customer_invoice_line:"
 msgid "Customer Invoice Line"
-msgstr ""
+msgstr "供应商发票行项目"
 
+#, fuzzy
 msgctxt "field:account.asset,depreciated_amount:"
 msgid "Depreciated Amount"
-msgstr ""
+msgstr "Depreciation Table"
 
+#, fuzzy
 msgctxt "field:account.asset,depreciating_value:"
 msgid "Depreciating Value"
-msgstr ""
+msgstr "Depreciation Table"
 
 msgctxt "field:account.asset,depreciation_method:"
 msgid "Depreciation Method"
 msgstr ""
 
 msgctxt "field:account.asset,end_date:"
 msgid "End Date"
@@ -80,71 +83,76 @@
 
 msgctxt "field:account.asset,revisions:"
 msgid "Revisions"
 msgstr ""
 
 msgctxt "field:account.asset,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "开始日期"
 
 msgctxt "field:account.asset,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
 msgctxt "field:account.asset,supplier_invoice_line:"
 msgid "Supplier Invoice Line"
-msgstr ""
+msgstr "供应商发票行项目"
 
 msgctxt "field:account.asset,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "单位"
 
 msgctxt "field:account.asset,update_moves:"
 msgid "Update Moves"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset,value:"
 msgid "Value"
-msgstr ""
+msgstr "值"
 
+#, fuzzy
 msgctxt "field:account.asset-update-account.move,asset:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "field:account.asset-update-account.move,move:"
 msgid "Move"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.create_moves.start,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.asset.line,accumulated_depreciation:"
 msgid "Accumulated Depreciation"
 msgstr ""
 
 msgctxt "field:account.asset.line,acquired_value:"
 msgid "Acquired Value"
 msgstr ""
 
 msgctxt "field:account.asset.line,actual_value:"
 msgid "Actual Value"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.line,asset:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "field:account.asset.line,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.line,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.asset.line,depreciable_basis:"
 msgid "Depreciable Basis"
 msgstr ""
 
 msgctxt "field:account.asset.line,depreciation:"
 msgid "Depreciation"
@@ -154,57 +162,62 @@
 msgid "Account Move"
 msgstr ""
 
 msgctxt "field:account.asset.print_depreciation_table.start,end_date:"
 msgid "End Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.print_depreciation_table.start,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "开始日期"
 
+#, fuzzy
 msgctxt "field:account.asset.revision,asset:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "field:account.asset.revision,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.asset.revision,description:"
 msgid "Description"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.revision,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.asset.revision,origin:"
 msgid "Origin"
 msgstr ""
 
 msgctxt "field:account.asset.revision,residual_value:"
 msgid "Residual Value"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.revision,value:"
 msgid "Asset Value"
-msgstr ""
+msgstr "值"
 
 msgctxt "field:account.asset.update.show_depreciation,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,counterpart_account:"
 msgid "Counterpart Account"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.asset.update.show_depreciation,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.asset.update.show_depreciation,depreciation_account:"
 msgid "Depreciation Account"
 msgstr ""
 
 msgctxt "field:account.asset.update.show_depreciation,latest_move_date:"
 msgid "Latest Move Date"
@@ -218,17 +231,18 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "field:account.configuration,asset_bymonthday:"
 msgid "Day of the Month"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.configuration,asset_frequency:"
 msgid "Asset Depreciation Frequency"
-msgstr ""
+msgstr "Print Depreciation Table"
 
 msgctxt "field:account.configuration,asset_sequence:"
 msgid "Asset Reference Sequence"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_date,asset_bymonth:"
 msgid "Month"
@@ -238,33 +252,35 @@
 msgid "Day of the Month"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_date,company:"
 msgid "Company"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.configuration.asset_frequency,asset_frequency:"
 msgid "Asset Depreciation Frequency"
-msgstr ""
+msgstr "Print Depreciation Table"
 
 msgctxt "field:account.configuration.asset_frequency,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_sequence,asset_sequence:"
 msgid "Asset Reference Sequence"
 msgstr ""
 
 msgctxt "field:account.configuration.asset_sequence,company:"
 msgid "Company"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.line,asset:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "field:account.invoice.line,is_assets_depreciable:"
 msgid "Is Assets depreciable"
 msgstr ""
 
 msgctxt "field:product.category,account_asset:"
 msgid "Account Asset"
@@ -344,17 +360,18 @@
 msgid "In months"
 msgstr ""
 
 msgctxt "help:product.template,depreciation_duration:"
 msgid "In months"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:account.asset,name:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "model:account.asset-update-account.move,name:"
 msgid "Asset - Update - Move"
 msgstr ""
 
 msgctxt "model:account.asset.create_moves.start,name:"
 msgid "Create Moves Start"
@@ -386,51 +403,53 @@
 
 msgctxt "model:account.configuration.asset_sequence,name:"
 msgid "Account Configuration Asset Sequence"
 msgstr ""
 
 msgctxt "model:account.journal,name:journal_asset"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "model:ir.action,name:act_asset_form"
 msgid "Assets"
-msgstr ""
+msgstr "Assets"
 
 msgctxt "model:ir.action,name:report_depreciation_table"
 msgid "Depreciation Table"
-msgstr ""
+msgstr "Depreciation Table"
 
 msgctxt "model:ir.action,name:wizard_create_moves"
 msgid "Create Assets Moves"
-msgstr ""
+msgstr "Create Assets Moves"
 
 msgctxt "model:ir.action,name:wizard_print_depreciation_table"
 msgid "Print Depreciation Table"
-msgstr ""
+msgstr "Print Depreciation Table"
 
 msgctxt "model:ir.action,name:wizard_update"
 msgid "Update Asset"
-msgstr ""
+msgstr "Update Asset"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "全部"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_closed"
 msgid "Closed"
-msgstr ""
+msgstr "关闭"
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_running"
 msgid "Running"
-msgstr ""
+msgstr "Running"
 
 msgctxt "model:ir.message,text:msg_asset_delete_draft"
 msgid "You cannot delete asset \"%(asset)s\" because it is not in \"draft\" state."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_asset_draft_lines"
 msgid "You cannot reset to draft asset \"%(asset)s\" because it has lines."
@@ -456,105 +475,112 @@
 
 msgctxt "model:ir.message,text:msg_purchase_product_missing_account_asset"
 msgid ""
 "To invoice purchase \"%(purchase)s\", you must set an account asset on "
 "product \"%(product)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,confirm:asset_close_button"
 msgid "Are you sure you want to close the asset?"
-msgstr ""
+msgstr "Are you sure to close the asset?"
 
 msgctxt "model:ir.model.button,string:asset_clear_lines_button"
 msgid "Clear Lines"
-msgstr ""
+msgstr "Clear Lines"
 
 msgctxt "model:ir.model.button,string:asset_close_button"
 msgid "Close"
-msgstr ""
+msgstr "Close"
 
 msgctxt "model:ir.model.button,string:asset_create_lines_button"
 msgid "Create Lines"
-msgstr ""
+msgstr "Create Lines"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:asset_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:asset_run_button"
 msgid "Run"
-msgstr ""
+msgstr "Run"
 
 msgctxt "model:ir.model.button,string:asset_update_button"
 msgid "Update Asset"
-msgstr ""
+msgstr "Update Asset"
 
 msgctxt "model:ir.rule.group,name:rule_group_asset_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_asset"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_asset"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "model:ir.ui.menu,name:menu_asset"
 msgid "Assets"
-msgstr ""
+msgstr "Assets"
 
 msgctxt "model:ir.ui.menu,name:menu_asset_form"
 msgid "Assets"
-msgstr ""
+msgstr "Assets"
 
 msgctxt "model:ir.ui.menu,name:menu_create_depreciation_table"
 msgid "Print Depreciation Table"
-msgstr ""
+msgstr "Print Depreciation Table"
 
 msgctxt "model:ir.ui.menu,name:menu_create_moves"
 msgid "Create Assets Moves"
-msgstr ""
+msgstr "Create Assets Moves"
 
+#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "("
-msgstr ""
+msgstr "("
 
+#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid ")"
-msgstr ""
+msgstr ")"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "+"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "-"
-msgstr ""
+msgstr "-"
 
+#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "/"
-msgstr ""
+msgstr "/"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Actual Value"
 msgstr ""
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Amortization"
 msgstr ""
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Amortization Table"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Assets"
-msgstr ""
+msgstr "Assets"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Closing Value"
 msgstr ""
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Company:"
@@ -596,25 +622,28 @@
 msgid "Monthly"
 msgstr ""
 
 msgctxt "selection:account.asset,frequency:"
 msgid "Yearly"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:account.asset,state:"
 msgid "Closed"
-msgstr ""
+msgstr "关闭"
 
+#, fuzzy
 msgctxt "selection:account.asset,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:account.asset,state:"
 msgid "Running"
-msgstr ""
+msgstr "Running"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "April"
 msgstr ""
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "August"
@@ -720,74 +749,87 @@
 msgid "First"
 msgstr ""
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonthday:"
 msgid "Last"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
+#, fuzzy
 msgctxt "view:account.asset.create_moves.start:"
 msgid "Create Assets Moves up to"
-msgstr ""
+msgstr "Create Assets Moves"
 
 msgctxt "view:account.asset:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "view:account.asset:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Asset"
-msgstr ""
+msgstr "Asset"
 
 msgctxt "view:account.configuration:"
 msgid "Asset Move"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Depreciation Frequency"
-msgstr ""
+msgstr "Depreciation Table"
 
+#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Sequence"
-msgstr ""
+msgstr "序列"
 
 msgctxt "view:product.template:"
 msgid "Depreciation"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.create_moves,start,create_moves:"
 msgid "OK"
-msgstr ""
+msgstr "确定"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.create_moves,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.print_depreciation_table,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.print_depreciation_table,start,print_:"
 msgid "Print"
-msgstr ""
+msgstr "打印"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.update,show_move,create_move:"
 msgid "OK"
-msgstr ""
+msgstr "确定"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.update,show_move,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.update,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:account.asset.update,start,update_asset:"
 msgid "OK"
-msgstr ""
+msgstr "确定"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_asset-7.0.0/locale/zh_CN.po` & `trytond_account_asset-7.2.0/locale/ro.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,397 +1,392 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,fixed_asset:"
 msgid "Fixed Asset"
-msgstr ""
+msgstr "Mijloc Fix"
 
 msgctxt "field:account.account.type.template,fixed_asset:"
 msgid "Fixed Asset"
-msgstr ""
+msgstr "Activ Fix"
 
 msgctxt "field:account.asset,account_journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.asset,comment:"
 msgid "Comment"
-msgstr ""
+msgstr "Cometariu"
 
 msgctxt "field:account.asset,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.asset,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Monedă"
 
-#, fuzzy
 msgctxt "field:account.asset,customer_invoice_line:"
 msgid "Customer Invoice Line"
-msgstr "供应商发票行项目"
+msgstr "Rând Factura Client"
 
-#, fuzzy
 msgctxt "field:account.asset,depreciated_amount:"
 msgid "Depreciated Amount"
-msgstr "Depreciation Table"
+msgstr "Suma Amortizata"
 
-#, fuzzy
 msgctxt "field:account.asset,depreciating_value:"
 msgid "Depreciating Value"
-msgstr "Depreciation Table"
+msgstr "Valoare de Depreciere"
 
 msgctxt "field:account.asset,depreciation_method:"
 msgid "Depreciation Method"
-msgstr ""
+msgstr "Metoda Amortizarii"
 
 msgctxt "field:account.asset,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data de Incheiere"
 
 msgctxt "field:account.asset,frequency:"
 msgid "Frequency"
-msgstr ""
+msgstr "Frecventa"
 
 msgctxt "field:account.asset,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
 msgctxt "field:account.asset,move:"
 msgid "Account Move"
-msgstr ""
+msgstr "Mişcare Cont"
 
 msgctxt "field:account.asset,number:"
 msgid "Number"
-msgstr ""
+msgstr "Numar"
 
 msgctxt "field:account.asset,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:account.asset,purchase_date:"
 msgid "Purchase Date"
-msgstr ""
+msgstr "Data Achizitiei"
 
 msgctxt "field:account.asset,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Cantitate"
 
 msgctxt "field:account.asset,residual_value:"
 msgid "Residual Value"
-msgstr ""
+msgstr "Valoare Reziduala"
 
+#, fuzzy
 msgctxt "field:account.asset,revisions:"
 msgid "Revisions"
-msgstr ""
+msgstr "Revizuiri"
 
 msgctxt "field:account.asset,start_date:"
 msgid "Start Date"
-msgstr "开始日期"
+msgstr "Data de Inceput"
 
 msgctxt "field:account.asset,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
 msgctxt "field:account.asset,supplier_invoice_line:"
 msgid "Supplier Invoice Line"
-msgstr "供应商发票行项目"
+msgstr "Rând Factură Furnizor"
 
 msgctxt "field:account.asset,unit:"
 msgid "Unit"
-msgstr "单位"
+msgstr "Unitate"
 
 msgctxt "field:account.asset,update_moves:"
 msgid "Update Moves"
-msgstr ""
+msgstr "Actualizare Miscari"
 
-#, fuzzy
 msgctxt "field:account.asset,value:"
 msgid "Value"
-msgstr "值"
+msgstr "Valoare"
 
-#, fuzzy
 msgctxt "field:account.asset-update-account.move,asset:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "field:account.asset-update-account.move,move:"
 msgid "Move"
-msgstr ""
+msgstr "Miscare"
 
-#, fuzzy
 msgctxt "field:account.asset.create_moves.start,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
+#, fuzzy
 msgctxt "field:account.asset.line,accumulated_depreciation:"
 msgid "Accumulated Depreciation"
-msgstr ""
+msgstr "Depreciere Acumulata"
 
 msgctxt "field:account.asset.line,acquired_value:"
 msgid "Acquired Value"
-msgstr ""
+msgstr "Valoare Dobandita"
 
 msgctxt "field:account.asset.line,actual_value:"
 msgid "Actual Value"
-msgstr ""
+msgstr "Valoare Reala"
 
-#, fuzzy
 msgctxt "field:account.asset.line,asset:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "field:account.asset.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:account.asset.line,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:account.asset.line,depreciable_basis:"
 msgid "Depreciable Basis"
-msgstr ""
+msgstr "Baza Amortizabila"
 
 msgctxt "field:account.asset.line,depreciation:"
 msgid "Depreciation"
-msgstr ""
+msgstr "Amortizare"
 
 msgctxt "field:account.asset.line,move:"
 msgid "Account Move"
-msgstr ""
+msgstr "Mişcare Cont"
 
 msgctxt "field:account.asset.print_depreciation_table.start,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data Sfarsit"
 
-#, fuzzy
 msgctxt "field:account.asset.print_depreciation_table.start,start_date:"
 msgid "Start Date"
-msgstr "开始日期"
+msgstr "Data Inceput"
 
-#, fuzzy
 msgctxt "field:account.asset.revision,asset:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "field:account.asset.revision,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:account.asset.revision,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.asset.revision,end_date:"
 msgid "End Date"
-msgstr "日期格式"
+msgstr "Data Sfarsit"
 
 msgctxt "field:account.asset.revision,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:account.asset.revision,residual_value:"
 msgid "Residual Value"
-msgstr ""
+msgstr "Valoare Reziduala"
 
-#, fuzzy
 msgctxt "field:account.asset.revision,value:"
 msgid "Asset Value"
-msgstr "值"
+msgstr "Valoare Activ"
 
 msgctxt "field:account.asset.update.show_depreciation,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
+#, fuzzy
 msgctxt "field:account.asset.update.show_depreciation,counterpart_account:"
 msgid "Counterpart Account"
-msgstr ""
+msgstr "Cont Omolog"
 
-#, fuzzy
 msgctxt "field:account.asset.update.show_depreciation,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:account.asset.update.show_depreciation,depreciation_account:"
 msgid "Depreciation Account"
-msgstr ""
+msgstr "Cont de Amortizare"
 
 msgctxt "field:account.asset.update.show_depreciation,latest_move_date:"
 msgid "Latest Move Date"
-msgstr ""
+msgstr "Data Ultimei Mutari"
 
+#, fuzzy
 msgctxt "field:account.asset.update.show_depreciation,next_depreciation_date:"
 msgid "Next Depreciation Date"
-msgstr ""
+msgstr "Data Urmatoarei Amortizari"
 
 msgctxt "field:account.configuration,asset_bymonth:"
 msgid "Month"
-msgstr ""
+msgstr "Luna"
 
 msgctxt "field:account.configuration,asset_bymonthday:"
 msgid "Day of the Month"
-msgstr ""
+msgstr "Zi a Lunii"
 
-#, fuzzy
 msgctxt "field:account.configuration,asset_frequency:"
 msgid "Asset Depreciation Frequency"
-msgstr "Print Depreciation Table"
+msgstr "Frecventa Amortizarii Activelor"
 
 msgctxt "field:account.configuration,asset_sequence:"
 msgid "Asset Reference Sequence"
-msgstr ""
+msgstr "Secventa de Referinta a Activelor"
 
 msgctxt "field:account.configuration.asset_date,asset_bymonth:"
 msgid "Month"
-msgstr ""
+msgstr "Luna"
 
 msgctxt "field:account.configuration.asset_date,asset_bymonthday:"
 msgid "Day of the Month"
-msgstr ""
+msgstr "Zi a Lunii"
 
 msgctxt "field:account.configuration.asset_date,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.configuration.asset_frequency,asset_frequency:"
 msgid "Asset Depreciation Frequency"
-msgstr "Print Depreciation Table"
+msgstr "Frecventa Amortizarii Activelor"
 
 msgctxt "field:account.configuration.asset_frequency,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.configuration.asset_sequence,asset_sequence:"
 msgid "Asset Reference Sequence"
-msgstr ""
+msgstr "Secventa de Referinta a Activelor"
 
 msgctxt "field:account.configuration.asset_sequence,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.invoice.line,asset:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "field:account.invoice.line,is_assets_depreciable:"
 msgid "Is Assets depreciable"
 msgstr ""
 
 msgctxt "field:product.category,account_asset:"
 msgid "Account Asset"
-msgstr ""
+msgstr "Activ al Contului"
 
 msgctxt "field:product.category,account_depreciation:"
 msgid "Account Depreciation"
-msgstr ""
+msgstr "Amortizarea Contului"
 
 msgctxt "field:product.category.account,account_asset:"
 msgid "Account Asset"
-msgstr ""
+msgstr "Activ al Contului"
 
 msgctxt "field:product.category.account,account_depreciation:"
 msgid "Account Depreciation"
-msgstr ""
+msgstr "Amortizarea Contului"
 
 msgctxt "field:product.product,depreciable:"
 msgid "Depreciable"
-msgstr ""
+msgstr "Amortizabil"
 
 msgctxt "field:product.product,depreciation_duration:"
 msgid "Depreciation Duration"
-msgstr ""
+msgstr "Durata Amortizarii"
 
 msgctxt "field:product.template,depreciable:"
 msgid "Depreciable"
-msgstr ""
+msgstr "Amortizabil"
 
 msgctxt "field:product.template,depreciation_duration:"
 msgid "Depreciation Duration"
-msgstr ""
+msgstr "Durata Amortizarii"
 
 msgctxt "help:account.asset,depreciated_amount:"
 msgid "The amount already depreciated at the start date."
-msgstr ""
+msgstr "Suma deja amortizata la data de inceput."
 
 msgctxt "help:account.asset,depreciating_value:"
 msgid "The value of the asset at the start date."
-msgstr ""
+msgstr "Valoarea activului la data de inceput."
 
 msgctxt "help:account.asset,value:"
 msgid "The value of the asset when purchased."
-msgstr ""
+msgstr "Valoarea activului la momentul achizitiei."
 
 msgctxt "help:account.asset.update.show_depreciation,date:"
 msgid ""
 "The date must be between the last update/depreciation date and the next "
 "depreciation date."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:account.configuration,asset_bymonth:"
 msgid "The month to create the depreciation moves."
-msgstr ""
+msgstr "Luna in care se creeaza miscari de amortizare."
 
+#, fuzzy
 msgctxt "help:account.configuration,asset_bymonthday:"
 msgid "The day of the month to create the depreciation moves."
-msgstr ""
+msgstr "Ziua din luna in care se creeaza miscari de amortizare."
 
 msgctxt "help:account.configuration,asset_frequency:"
 msgid "The default depreciation frequency for new assets."
-msgstr ""
+msgstr "Frecvența implicită de amortizare pentru active noi."
 
+#, fuzzy
 msgctxt "help:account.configuration.asset_date,asset_bymonth:"
 msgid "The month to create the depreciation moves."
-msgstr ""
+msgstr "Luna in care se creeaza miscari de amortizare."
 
+#, fuzzy
 msgctxt "help:account.configuration.asset_date,asset_bymonthday:"
 msgid "The day of the month to create the depreciation moves."
-msgstr ""
+msgstr "Ziua din luna in care se creeaza miscari de amortizare."
 
 msgctxt "help:account.configuration.asset_frequency,asset_frequency:"
 msgid "The default depreciation frequency for new assets."
-msgstr ""
+msgstr "Frecvența implicită de amortizare pentru active noi."
 
 msgctxt "help:product.product,depreciation_duration:"
 msgid "In months"
-msgstr ""
+msgstr "In Luni"
 
+#, fuzzy
 msgctxt "help:product.template,depreciation_duration:"
 msgid "In months"
-msgstr ""
+msgstr "In Luni"
 
 #, fuzzy
 msgctxt "model:account.asset,name:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
+#, fuzzy
 msgctxt "model:account.asset-update-account.move,name:"
 msgid "Asset - Update - Move"
-msgstr ""
+msgstr "Activ - Actualizare - Miscare"
 
 msgctxt "model:account.asset.create_moves.start,name:"
 msgid "Create Moves Start"
 msgstr ""
 
 msgctxt "model:account.asset.line,name:"
 msgid "Asset Line"
-msgstr ""
+msgstr "Rând Active"
 
 msgctxt "model:account.asset.print_depreciation_table.start,name:"
 msgid "Asset Depreciation Table Start"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:account.asset.revision,name:"
 msgid "Asset Revision"
-msgstr ""
+msgstr "Revizuire Active"
 
 msgctxt "model:account.asset.update.show_depreciation,name:"
 msgid "Update Asset Show Depreciation"
 msgstr ""
 
 msgctxt "model:account.configuration.asset_date,name:"
 msgid "Account Configuration Asset Date"
@@ -403,433 +398,424 @@
 
 msgctxt "model:account.configuration.asset_sequence,name:"
 msgid "Account Configuration Asset Sequence"
 msgstr ""
 
 msgctxt "model:account.journal,name:journal_asset"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "model:ir.action,name:act_asset_form"
 msgid "Assets"
-msgstr "Assets"
+msgstr "Active"
 
 msgctxt "model:ir.action,name:report_depreciation_table"
 msgid "Depreciation Table"
-msgstr "Depreciation Table"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_create_moves"
 msgid "Create Assets Moves"
-msgstr "Create Assets Moves"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_print_depreciation_table"
 msgid "Print Depreciation Table"
-msgstr "Print Depreciation Table"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_update"
 msgid "Update Asset"
-msgstr "Update Asset"
+msgstr "Actualizare Activ"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_closed"
 msgid "Closed"
-msgstr "关闭"
+msgstr "Închis"
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_running"
 msgid "Running"
-msgstr "Running"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_asset_delete_draft"
 msgid "You cannot delete asset \"%(asset)s\" because it is not in \"draft\" state."
-msgstr ""
+msgstr "Nu puteți șterge activul \"%(asset)s\" deoarece nu este în stare \"Ciornă\"."
 
 msgctxt "model:ir.message,text:msg_asset_draft_lines"
 msgid "You cannot reset to draft asset \"%(asset)s\" because it has lines."
 msgstr ""
+"Nu puteți reseta activul \"%(asset)s\" la starea de ciornă deoarece are "
+"rânduri."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_asset_invoice_line_unique"
 msgid "Invoice line can be used only once on asset."
-msgstr ""
+msgstr "Linia de factură poate fi folosită o singură dată pe activ."
 
 msgctxt "model:ir.message,text:msg_asset_running_close_period"
 msgid ""
 "You cannot close period \"%(period)s\" because some assets \"%(assets)s\" "
 "still have lines without move."
 msgstr ""
+"Nu puteți închide perioada \"%(period)s\" deoarece unele active "
+"\"%(assets)s\" mai au rânduri fără mișcare."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invoice_line_asset_unique"
 msgid "Asset can be used only once on invoice line."
-msgstr ""
+msgstr "Activul poate fi folosit o singură dată pe linia de factură."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_no_assets"
 msgid "There is no started asset."
-msgstr ""
+msgstr "Nu există niciun activ început."
 
 msgctxt "model:ir.message,text:msg_purchase_product_missing_account_asset"
 msgid ""
 "To invoice purchase \"%(purchase)s\", you must set an account asset on "
 "product \"%(product)s\"."
 msgstr ""
+"Pentru a factura achiziția \"%(purchase)s\", trebuie să setați un activ de "
+"cont pe produsul \"%(product)s\"."
 
 #, fuzzy
 msgctxt "model:ir.model.button,confirm:asset_close_button"
 msgid "Are you sure you want to close the asset?"
-msgstr "Are you sure to close the asset?"
+msgstr "Sunteți sigur că doriți să închideți activul?"
 
 msgctxt "model:ir.model.button,string:asset_clear_lines_button"
 msgid "Clear Lines"
-msgstr "Clear Lines"
+msgstr "Goliți rândurile"
 
 msgctxt "model:ir.model.button,string:asset_close_button"
 msgid "Close"
-msgstr "Close"
+msgstr "Inchide"
 
 msgctxt "model:ir.model.button,string:asset_create_lines_button"
 msgid "Create Lines"
-msgstr "Create Lines"
+msgstr "Creează rânduri"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:asset_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
 msgctxt "model:ir.model.button,string:asset_run_button"
 msgid "Run"
-msgstr "Run"
+msgstr "Ruleaza"
 
 msgctxt "model:ir.model.button,string:asset_update_button"
 msgid "Update Asset"
-msgstr "Update Asset"
+msgstr "Actualizare Activ"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_asset_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator in Companii"
 
 msgctxt "model:ir.sequence,name:sequence_asset"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_asset"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "model:ir.ui.menu,name:menu_asset"
 msgid "Assets"
-msgstr "Assets"
+msgstr "Active"
 
 msgctxt "model:ir.ui.menu,name:menu_asset_form"
 msgid "Assets"
-msgstr "Assets"
+msgstr "Active"
 
 msgctxt "model:ir.ui.menu,name:menu_create_depreciation_table"
 msgid "Print Depreciation Table"
-msgstr "Print Depreciation Table"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_create_moves"
 msgid "Create Assets Moves"
-msgstr "Create Assets Moves"
+msgstr "Creeaza Mutari de Active"
 
-#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "("
 msgstr "("
 
-#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid ")"
 msgstr ")"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "+"
-msgstr ""
+msgstr "+"
 
-#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "-"
 msgstr "-"
 
-#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "/"
 msgstr "/"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Actual Value"
-msgstr ""
+msgstr "Valoare Reala"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Amortization"
-msgstr ""
+msgstr "Amortizare"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Amortization Table"
-msgstr ""
+msgstr "Tabel Amortizare"
 
-#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Assets"
-msgstr "Assets"
+msgstr "Active"
 
+#, fuzzy
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Closing Value"
-msgstr ""
+msgstr "Valoare de Inchidere"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Company:"
-msgstr ""
+msgstr "Companie:"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Fixed"
-msgstr ""
+msgstr "Fix"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "From:"
-msgstr ""
+msgstr "De la:"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Print Date:"
-msgstr ""
+msgstr "Data Tiparirii:"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "To:"
-msgstr ""
+msgstr "Catre:"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "Total -"
-msgstr ""
+msgstr "Total -"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "User:"
-msgstr ""
+msgstr "Utilizator:"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "at"
-msgstr ""
+msgstr "la"
 
 msgctxt "selection:account.asset,depreciation_method:"
 msgid "Linear"
-msgstr ""
+msgstr "Liniar"
 
 msgctxt "selection:account.asset,frequency:"
 msgid "Monthly"
-msgstr ""
+msgstr "Lunar"
 
 msgctxt "selection:account.asset,frequency:"
 msgid "Yearly"
-msgstr ""
+msgstr "Anual"
 
-#, fuzzy
 msgctxt "selection:account.asset,state:"
 msgid "Closed"
-msgstr "关闭"
+msgstr "Închis"
 
-#, fuzzy
 msgctxt "selection:account.asset,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
-#, fuzzy
 msgctxt "selection:account.asset,state:"
 msgid "Running"
-msgstr "Running"
+msgstr "In Derulare"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "April"
-msgstr ""
+msgstr "Aprilie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "August"
-msgstr ""
+msgstr "August"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "December"
-msgstr ""
+msgstr "Decembrie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "February"
-msgstr ""
+msgstr "Februarie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "January"
-msgstr ""
+msgstr "Ianuarie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "July"
-msgstr ""
+msgstr "Iulie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "June"
-msgstr ""
+msgstr "Iunie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "March"
-msgstr ""
+msgstr "Martie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "May"
-msgstr ""
+msgstr "Mai"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "November"
-msgstr ""
+msgstr "Noiembrie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "October"
-msgstr ""
+msgstr "Octombrie"
 
 msgctxt "selection:account.configuration,asset_bymonth:"
 msgid "September"
-msgstr ""
+msgstr "Septembrie"
 
 msgctxt "selection:account.configuration,asset_bymonthday:"
 msgid "First"
-msgstr ""
+msgstr "Primul"
 
 msgctxt "selection:account.configuration,asset_bymonthday:"
 msgid "Last"
-msgstr ""
+msgstr "Ultimul"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "April"
-msgstr ""
+msgstr "Aprilie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "August"
-msgstr ""
+msgstr "August"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "December"
-msgstr ""
+msgstr "Decembrie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "February"
-msgstr ""
+msgstr "Februarie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "January"
-msgstr ""
+msgstr "Ianuarie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "July"
-msgstr ""
+msgstr "Iulie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "June"
-msgstr ""
+msgstr "Iunie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "March"
-msgstr ""
+msgstr "Martie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "May"
-msgstr ""
+msgstr "Mai"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "November"
-msgstr ""
+msgstr "Noiembrie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "October"
-msgstr ""
+msgstr "Octombrie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonth:"
 msgid "September"
-msgstr ""
+msgstr "Septembrie"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonthday:"
 msgid "First"
-msgstr ""
+msgstr "Primul"
 
 msgctxt "selection:account.configuration.asset_date,asset_bymonthday:"
 msgid "Last"
-msgstr ""
+msgstr "Ultimul"
 
-#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 #, fuzzy
 msgctxt "view:account.asset.create_moves.start:"
 msgid "Create Assets Moves up to"
-msgstr "Create Assets Moves"
+msgstr "Creeaza Miscari de Active pana la"
 
 msgctxt "view:account.asset:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
 msgctxt "view:account.asset:"
 msgid "Other Info"
-msgstr ""
+msgstr "Alte Informatii"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Asset"
-msgstr "Asset"
+msgstr "Activ"
 
 msgctxt "view:account.configuration:"
 msgid "Asset Move"
-msgstr ""
+msgstr "Mişcare Activ"
 
 #, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Depreciation Frequency"
-msgstr "Depreciation Table"
+msgstr "Frecventa Amortizare"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Sequence"
-msgstr "序列"
+msgstr "Secventa"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Depreciation"
-msgstr ""
+msgstr "Amortizare"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.create_moves,start,create_moves:"
 msgid "OK"
-msgstr "确定"
+msgstr "OK"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.create_moves,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.print_depreciation_table,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.print_depreciation_table,start,print_:"
 msgid "Print"
-msgstr "打印"
+msgstr "Tipărire"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.update,show_move,create_move:"
 msgid "OK"
-msgstr "确定"
+msgstr "OK"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.update,show_move,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.update,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.asset.update,start,update_asset:"
 msgid "OK"
-msgstr "确定"
+msgstr "OK"
```

### Comparing `trytond_account_asset-7.0.0/message.xml` & `trytond_account_asset-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart.xml` & `trytond_account_asset-7.2.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_bg.xml` & `trytond_account_asset-7.2.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_ca.xml` & `trytond_account_asset-7.2.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_de.xml` & `trytond_account_asset-7.2.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_en.xml` & `trytond_account_asset-7.2.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_es.xml` & `trytond_account_asset-7.2.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_fr.xml` & `trytond_account_asset-7.2.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_nl.xml` & `trytond_account_asset-7.2.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_pt.xml` & `trytond_account_asset-7.2.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_ru.xml` & `trytond_account_asset-7.2.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/minimal_chart_sl.xml` & `trytond_account_asset-7.2.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/product.py` & `trytond_account_asset-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/product.xml` & `trytond_account_asset-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/purchase.py` & `trytond_account_asset-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/setup.py` & `trytond_account_asset-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/tests/scenario_account_asset.rst` & `trytond_account_asset-7.2.0/tests/scenario_account_asset.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ======================
 Account Asset Scenario
 ======================
 
 Imports::
 
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
+    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> from trytond.modules.account_asset.tests.tools \
-    ...     import add_asset_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_asset.tests.tools import add_asset_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('account_asset')
 
 Create company::
 
@@ -90,48 +90,43 @@
     >>> supplier_invoice = Invoice(type='in')
     >>> supplier_invoice.party = supplier
     >>> invoice_line = InvoiceLine()
     >>> supplier_invoice.lines.append(invoice_line)
     >>> invoice_line.product = asset_product
     >>> invoice_line.quantity = 1
     >>> invoice_line.unit_price = Decimal('1000')
-    >>> invoice_line.account == asset_account
-    True
+    >>> assertEqual(invoice_line.account, asset_account)
     >>> supplier_invoice.invoice_date = fiscalyear.start_date
     >>> supplier_invoice.click('post')
     >>> supplier_invoice.state
     'posted'
     >>> invoice_line, = supplier_invoice.lines
-    >>> (asset_account.debit, asset_account.credit) == \
-    ...     (Decimal('1000'), Decimal('0'))
-    True
+    >>> (asset_account.debit, asset_account.credit)
+    (Decimal('1000.00'), Decimal('0.00'))
 
 Depreciate the asset::
 
     >>> Asset = Model.get('account.asset')
     >>> asset = Asset()
     >>> asset.product = asset_product
     >>> asset.supplier_invoice_line = invoice_line
     >>> asset.value
     Decimal('1000.00')
-    >>> asset.start_date == supplier_invoice.invoice_date
-    True
-    >>> asset.end_date == (supplier_invoice.invoice_date +
-    ...     relativedelta(years=2, days=-1))
-    True
+    >>> assertEqual(asset.start_date, supplier_invoice.invoice_date)
+    >>> assertEqual(asset.end_date,
+    ...     (supplier_invoice.invoice_date + relativedelta(years=2, days=-1)))
     >>> asset.quantity
     1.0
-    >>> asset.unit == unit
-    True
+    >>> assertEqual(asset.unit, unit)
     >>> asset.residual_value = Decimal('100')
     >>> asset.click('create_lines')
     >>> len(asset.lines)
     24
-    >>> [l.depreciation for l in asset.lines] == [Decimal('37.5')] * 24
-    True
+    >>> {l.depreciation for l in asset.lines}
+    {Decimal('37.50')}
     >>> asset.lines[0].actual_value
     Decimal('962.50')
     >>> asset.lines[0].accumulated_depreciation
     Decimal('37.50')
     >>> asset.lines[11].actual_value
     Decimal('550.00')
     >>> asset.lines[11].accumulated_depreciation
@@ -141,15 +136,15 @@
     >>> asset.lines[-1].accumulated_depreciation
     Decimal('900.00')
     >>> asset.click('run')
 
 Trying to close the period to check error::
 
     >>> period = supplier_invoice.move.period
-    >>> period.click('close') # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> period.click('close')
     Traceback (most recent call last):
         ...
     AccessError: ...
 
 Create Moves for 3 months::
 
     >>> create_moves = Wizard('account.asset.create_moves')
@@ -170,38 +165,38 @@
     >>> update = Wizard('account.asset.update', [asset])
     >>> update.form.value = Decimal('1100.00')
     >>> update.execute('update_asset')
     >>> update.form.amount
     Decimal('100.00')
     >>> update.form.date = (supplier_invoice.invoice_date
     ...     + relativedelta(months=2))
-    >>> update.form.latest_move_date == (supplier_invoice.invoice_date
-    ...     + relativedelta(months=3, days=-1))
-    True
-    >>> update.form.next_depreciation_date == (supplier_invoice.invoice_date
-    ...     + relativedelta(months=4, days=-1))
-    True
-    >>> update.execute('create_move')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> assertEqual(update.form.latest_move_date, (supplier_invoice.invoice_date
+    ...     + relativedelta(months=3, days=-1)))
+    >>> assertEqual(update.form.next_depreciation_date, (supplier_invoice.invoice_date
+    ...     + relativedelta(months=4, days=-1)))
+    >>> update.execute('create_move')
     Traceback (most recent call last):
         ...
     ValueError: ...
 
     >>> update.form.date = (supplier_invoice.invoice_date
     ...     + relativedelta(months=3))
     >>> update.execute('create_move')
     >>> asset.reload()
     >>> asset.value
     Decimal('1100.00')
     >>> revision, = asset.revisions
     >>> revision.value
     Decimal('1100.00')
-    >>> [l.depreciation for l in asset.lines[:3]]
-    [Decimal('37.50'), Decimal('37.50'), Decimal('37.50')]
-    >>> [l.depreciation for l in asset.lines[3:-1]] == [Decimal('42.26')] * 20
-    True
+    >>> len(asset.lines)
+    24
+    >>> {l.depreciation for l in asset.lines[:3]}
+    {Decimal('37.50')}
+    >>> {l.depreciation for l in asset.lines[3:-1]}
+    {Decimal('42.26')}
     >>> asset.lines[-1].depreciation
     Decimal('42.30')
     >>> depreciation_account.reload()
     >>> depreciation_account.debit
     Decimal('100.00')
     >>> depreciation_account.credit
     Decimal('112.50')
@@ -234,22 +229,20 @@
     >>> customer_invoice.party = customer
     >>> invoice_line = InvoiceLine()
     >>> customer_invoice.lines.append(invoice_line)
     >>> invoice_line.product = asset_product
     >>> invoice_line.asset = asset
     >>> invoice_line.quantity = 1
     >>> invoice_line.unit_price = Decimal('600')
-    >>> invoice_line.account == revenue
-    True
+    >>> assertEqual(invoice_line.account, revenue)
     >>> customer_invoice.click('post')
     >>> customer_invoice.state
     'posted'
     >>> asset.reload()
-    >>> asset.customer_invoice_line == customer_invoice.lines[0]
-    True
+    >>> assertEqual(asset.customer_invoice_line, customer_invoice.lines[0])
     >>> revenue.debit
     Decimal('860.72')
     >>> revenue.credit
     Decimal('600.00')
     >>> asset_account.reload()
     >>> asset_account.debit
     Decimal('1000.00')
```

### Comparing `trytond_account_asset-7.0.0/tests/scenario_account_asset_depreciated.rst` & `trytond_account_asset-7.2.0/tests/scenario_account_asset_depreciated.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ==================================
 Account Asset Depreciated Scenario
 ==================================
 
 Imports::
 
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
+    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_asset.tests.tools import add_asset_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> from trytond.modules.account_asset.tests.tools \
-    ...     import add_asset_accounts
 
 Activate modules::
 
     >>> config = activate_modules('account_asset')
 
 Create company::
 
@@ -73,27 +73,27 @@
     >>> Asset = Model.get('account.asset')
     >>> asset = Asset()
     >>> asset.product = asset_product
     >>> asset.value = Decimal('1500.00')
     >>> asset.depreciated_amount = Decimal('500.00')
     >>> asset.start_date = fiscalyear.start_date
     >>> asset.purchase_date = asset.start_date
-    >>> asset.end_date = (asset.start_date +
-    ...     relativedelta(years=2, days=-1))
+    >>> asset.end_date = (asset.start_date
+    ...     + relativedelta(years=2, days=-1))
     >>> asset.quantity = 1
     >>> asset.residual_value = Decimal('100')
     >>> asset.click('create_lines')
     >>> len(asset.lines)
     24
-    >>> [l.depreciation for l in asset.lines] == [Decimal('37.5')] * 24
-    True
-    >>> [l.acquired_value for l in asset.lines] == [Decimal('1500.00')] * 24
-    True
-    >>> [l.depreciable_basis for l in asset.lines] == [Decimal('900.00')] * 24
-    True
+    >>> {l.depreciation for l in asset.lines}
+    {Decimal('37.50')}
+    >>> {l.acquired_value for l in asset.lines}
+    {Decimal('1500.00')}
+    >>> {l.depreciable_basis for l in asset.lines}
+    {Decimal('900.00')}
     >>> asset.lines[0].actual_value
     Decimal('962.50')
     >>> asset.lines[0].accumulated_depreciation
     Decimal('537.50')
     >>> asset.lines[11].actual_value
     Decimal('550.00')
     >>> asset.lines[11].accumulated_depreciation
```

### Comparing `trytond_account_asset-7.0.0/tests/scenario_purchase_asset.rst` & `trytond_account_asset-7.2.0/tests/scenario_purchase_asset.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 =======================
 Purchase Asset Scenario
 =======================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
-    >>> from trytond.modules.account_asset.tests.tools \
-    ...     import add_asset_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_asset.tests.tools import add_asset_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['account_asset', 'purchase'])
 
 Create company::
 
@@ -98,11 +97,9 @@
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('5.0000')
     >>> purchase.click('quote')
     >>> purchase.click('confirm')
     >>> purchase.click('process')
     >>> invoice, = purchase.invoices
     >>> asset_line, service_line = invoice.lines
-    >>> asset_line.account == asset_account
-    True
-    >>> service_line.account == expense
-    True
+    >>> assertEqual(asset_line.account, asset_account)
+    >>> assertEqual(service_line.account, expense)
```

### Comparing `trytond_account_asset-7.0.0/tests/test_module.py` & `trytond_account_asset-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/tests/tools.py` & `trytond_account_asset-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/tox.ini` & `trytond_account_asset-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/trytond_account_asset.egg-info/PKG-INFO` & `trytond_account_asset-7.2.0/trytond_account_asset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-asset
-Version: 7.0.0
+Name: trytond_account_asset
+Version: 7.2.0
 Summary: Tryton module for assets management
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
@@ -50,22 +50,22 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Account Asset Module
 ####################
 
 The account_asset module adds the depreciation of fixed assets.
 
 Asset
```

### Comparing `trytond_account_asset-7.0.0/trytond_account_asset.egg-info/SOURCES.txt` & `trytond_account_asset-7.2.0/trytond_account_asset.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_account_asset-7.0.0/view/asset_form.xml` & `trytond_account_asset-7.2.0/view/asset_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/view/asset_line_form.xml` & `trytond_account_asset-7.2.0/view/asset_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/view/asset_tree.xml` & `trytond_account_asset-7.2.0/view/asset_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/view/asset_update_show_depreciation_form.xml` & `trytond_account_asset-7.2.0/view/asset_update_show_depreciation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/view/asset_update_start_form.xml` & `trytond_account_asset-7.2.0/view/asset_update_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/view/configuration_form.xml` & `trytond_account_asset-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.0.0/view/template_form.xml` & `trytond_account_asset-7.2.0/view/template_form.xml`

 * *Files identical despite different names*

