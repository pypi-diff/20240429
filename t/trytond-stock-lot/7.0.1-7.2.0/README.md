# Comparing `tmp/trytond_stock_lot-7.0.1.tar.gz` & `tmp/trytond_stock_lot-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot-7.0.1.tar", last modified: Mon Jan  1 12:06:38 2024, max compression
+gzip compressed data, was "trytond_stock_lot-7.2.0.tar", last modified: Mon Apr 29 15:51:22 2024, max compression
```

## Comparing `trytond_stock_lot-7.0.1.tar` & `trytond_stock_lot-7.2.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:06:38.517977 trytond_stock_lot-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-01-01 12:06:35.000000 trytond_stock_lot-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-01-01 12:06:35.000000 trytond_stock_lot-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-01-01 12:06:38.517977 trytond_stock_lot-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:06:38.511310 trytond_stock_lot-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2810 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      849 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:06:38.514644 trytond_stock_lot-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    11570 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12147 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10348 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12506 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12207 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10088 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10723 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12519 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10339 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12250 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11130 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10131 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10581 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11136 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10402 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12245 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10572 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11427 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9983 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11457 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11272 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10339 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9851 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11713 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4666 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-01 12:06:38.517977 trytond_stock_lot-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4364 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29601 2023-12-27 10:42:47.000000 trytond_stock_lot-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20436 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:06:38.514644 trytond_stock_lot-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3492 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/scenario_stock_lot_assign_try.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/scenario_stock_lot_move_add.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1631 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/scenario_stock_lot_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2588 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/scenario_stock_lot_shipment_in.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4548 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/scenario_stock_lot_shipment_out.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3920 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/scenario_stock_lot_shipment_out_internal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12487 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      168 2023-10-30 17:55:12.000000 trytond_stock_lot-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:06:38.517977 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-01-01 12:06:38.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2904 2024-01-01 12:06:38.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-01 12:06:38.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-01-01 12:06:38.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:14.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      105 2024-01-01 12:06:38.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-01 12:06:38.000000 trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:06:38.517977 trytond_stock_lot-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/inventory_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/inventory_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/lot_by_location_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/lot_by_warehouse_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/lot_trace_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/lot_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/lots_by_locations_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/period_cache_lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/period_cache_lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/stock_move_add_lots_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/stock_move_add_lots_start_lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-10-30 17:06:38.000000 trytond_stock_lot-7.0.1/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:22.712259 trytond_stock_lot-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2024-04-29 15:27:54.000000 trytond_stock_lot-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:27:54.000000 trytond_stock_lot-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-04-29 15:51:22.712259 trytond_stock_lot-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:22.705592 trytond_stock_lot-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:33.000000 trytond_stock_lot-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      849 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:22.705592 trytond_stock_lot-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11800 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12339 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10542 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12686 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12401 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10244 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10911 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12709 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10533 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12446 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11312 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10317 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10765 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11352 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10596 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12431 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10768 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11627 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10139 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11687 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11462 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10533 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10007 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11899 2024-04-29 13:17:17.000000 trytond_stock_lot-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4666 2024-04-23 22:09:20.000000 trytond_stock_lot-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:22.712259 trytond_stock_lot-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4423 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31049 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20380 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:22.708926 trytond_stock_lot-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3461 2024-04-22 12:14:36.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_assign_try.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_move_add.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_move_add.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2024-04-22 12:14:36.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2548 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_shipment_in.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4550 2024-04-22 12:14:36.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_shipment_out.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3964 2024-04-22 12:14:36.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_shipment_out_internal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2200 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/tests/scenario_stock_lot_trace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12516 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:33.000000 trytond_stock_lot-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-29 15:27:49.000000 trytond_stock_lot-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:22.708926 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-04-29 15:51:22.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2997 2024-04-29 15:51:22.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:22.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:51:22.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-04-29 15:51:22.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:22.000000 trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:22.708926 trytond_stock_lot-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/view/inventory_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/inventory_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/view/lot_by_location_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2024-01-27 09:58:52.000000 trytond_stock_lot-7.2.0/view/lot_by_warehouse_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-04-27 16:30:39.000000 trytond_stock_lot-7.2.0/view/lot_trace_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/lot_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/lots_by_locations_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/view/period_cache_lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:21.000000 trytond_stock_lot-7.2.0/view/period_cache_lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      718 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/stock_move_add_lots_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/stock_move_add_lots_start_lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-04-15 07:12:15.000000 trytond_stock_lot-7.2.0/view/template_form.xml
```

### Comparing `trytond_stock_lot-7.0.1/CHANGELOG` & `trytond_stock_lot-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-Version 7.0.1 - 2024-01-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
+* Add locations to lot trace
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Check customer lot quantities for drop shipment
 * Check outgoing lot quantities for internal shipment
```

### Comparing `trytond_stock_lot-7.0.1/LICENSE` & `trytond_stock_lot-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/PKG-INFO` & `trytond_stock_lot-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for lot of products
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
@@ -49,19 +49,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_split<7.3,>=7.2; extra == "test"
 
 Stock Lot Module
 ################
 
 The stock lot module defines lot of products.
 
 Lot
```

### Comparing `trytond_stock_lot-7.0.1/__init__.py` & `trytond_stock_lot-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/doc/conf.py` & `trytond_stock_lot-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_lot-7.0.1/ir.xml` & `trytond_stock_lot-7.2.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/locale/bg.po` & `trytond_stock_lot-7.2.0/locale/bg.po`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Местоположение"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Партида"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -93,14 +98,19 @@
 msgid "Quantity"
 msgstr "Количество"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Местоположение"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/ca.po` & `trytond_stock_lot-7.2.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "Document"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr "Traçabilitat descendent"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Ubicació"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "Producte"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "Quantitat"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr "Albarà"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Ubicació"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr "Unitat"
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr "Traçabilitat ascendent"
```

### Comparing `trytond_stock_lot-7.0.1/locale/cs.po` & `trytond_stock_lot-7.2.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Production"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -86,14 +91,19 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Production"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/de.po` & `trytond_stock_lot-7.2.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "Dokument"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr "Retrograde Rückverfolgung"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Ort"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Charge"
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "Artikel"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "Menge"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr "Lieferung"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Ort"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr "Einheit"
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr "Progressive Rückverfolgung"
```

### Comparing `trytond_stock_lot-7.0.1/locale/es.po` & `trytond_stock_lot-7.2.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "Documento"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr "Trazabilidad descendente"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Ubicación"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lote"
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "Producto"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "Cantidad"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr "Albarán"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Ubicación"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr "Unidad"
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr "Trazabilidad ascendente"
```

### Comparing `trytond_stock_lot-7.0.1/locale/es_419.po` & `trytond_stock_lot-7.2.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 msgid "Document"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr ""
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr ""
@@ -85,14 +89,18 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr ""
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/et.po` & `trytond_stock_lot-7.2.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Asukoht"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Partii"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -89,14 +94,19 @@
 msgid "Quantity"
 msgstr "Kogus"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Asukoht"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/fa.po` & `trytond_stock_lot-7.2.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "مکان"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "قطعه"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -89,14 +94,19 @@
 msgid "Quantity"
 msgstr "مقدار/تعداد"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "مکان"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/fi.po` & `trytond_stock_lot-7.2.0/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Production"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -86,14 +91,19 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Production"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/fr.po` & `trytond_stock_lot-7.2.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "Document"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr "Traces descendantes"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Emplacement"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "Produit"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "Quantité"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr "Expédition"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Emplacement"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr "Unité"
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr "Traces ascendantes"
```

### Comparing `trytond_stock_lot-7.0.1/locale/hu.po` & `trytond_stock_lot-7.2.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Hely"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Charge"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -90,14 +95,19 @@
 msgid "Quantity"
 msgstr "Mennyiség"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Hely"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/id.po` & `trytond_stock_lot-7.2.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "Dokumen"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Lokasi"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "Produk"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "Kuantitas"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Lokasi"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/it.po` & `trytond_stock_lot-7.2.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 msgid "Document"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Luogo"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lotto"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -87,14 +92,19 @@
 msgid "Quantity"
 msgstr "Quantità"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Luogo"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/lo.po` & `trytond_stock_lot-7.2.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "ບ່ອນຢູ່"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -91,14 +96,19 @@
 msgid "Quantity"
 msgstr "ຈຳນວນ"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "ບ່ອນຢູ່"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/lt.po` & `trytond_stock_lot-7.2.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Production"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lo"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -87,14 +92,19 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Production"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/nl.po` & `trytond_stock_lot-7.2.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "Document"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr "Neerwaartse tracering"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Plaats"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Batch"
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "Product"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "Hoeveelheid"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr "Zending"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Plaats"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr "Eenheid"
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr "Opwaartse tracering"
```

### Comparing `trytond_stock_lot-7.0.1/locale/pl.po` & `trytond_stock_lot-7.2.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Lokalizacja"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -88,14 +93,19 @@
 msgid "Quantity"
 msgstr "Ilość"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Lokalizacja"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/pt.po` & `trytond_stock_lot-7.2.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Localização"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lote"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -89,14 +94,19 @@
 msgid "Quantity"
 msgstr "Quantidade"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Localização"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/ro.po` & `trytond_stock_lot-7.2.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 msgid "Document"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr ""
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -84,14 +88,18 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr ""
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/ru.po` & `trytond_stock_lot-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Местоположение"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -92,14 +97,19 @@
 msgid "Quantity"
 msgstr "Кол-во"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Местоположение"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/sl.po` & `trytond_stock_lot-7.2.0/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Lokacija"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Serija"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -89,14 +94,19 @@
 msgid "Quantity"
 msgstr "Količina"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Lokacija"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/tr.po` & `trytond_stock_lot-7.2.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "Production"
+
+#, fuzzy
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "Lot"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
@@ -86,14 +91,19 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "Production"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/uk.po` & `trytond_stock_lot-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 msgid "Document"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr ""
 
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr ""
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr ""
@@ -83,14 +87,18 @@
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr ""
 
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr ""
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-7.0.1/locale/zh_CN.po` & `trytond_stock_lot-7.2.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 msgid "Document"
 msgstr "文档"
 
 msgctxt "field:stock.lot.trace,downward_traces:"
 msgid "Downward Traces"
 msgstr "向下追踪"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,from_location:"
+msgid "From Location"
+msgstr "库位"
+
 msgctxt "field:stock.lot.trace,lot:"
 msgid "Lot"
 msgstr "批次"
 
 msgctxt "field:stock.lot.trace,product:"
 msgid "Product"
 msgstr "产品"
@@ -83,14 +88,19 @@
 msgid "Quantity"
 msgstr "数量"
 
 msgctxt "field:stock.lot.trace,shipment:"
 msgid "Shipment"
 msgstr "收发货"
 
+#, fuzzy
+msgctxt "field:stock.lot.trace,to_location:"
+msgid "To Location"
+msgstr "库位"
+
 msgctxt "field:stock.lot.trace,unit:"
 msgid "Unit"
 msgstr "单位"
 
 msgctxt "field:stock.lot.trace,upward_traces:"
 msgid "Upward Traces"
 msgstr "向上追踪"
```

### Comparing `trytond_stock_lot-7.0.1/message.xml` & `trytond_stock_lot-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/product.py` & `trytond_stock_lot-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/product.xml` & `trytond_stock_lot-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/setup.py` & `trytond_stock_lot-7.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond_stock_split'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module for lot of products',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
```

### Comparing `trytond_stock_lot-7.0.1/stock.py` & `trytond_stock_lot-7.2.0/stock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 from collections import defaultdict
 from copy import copy
 from functools import wraps
 
-from sql import Column
+from sql import Column, Null
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, Model, ModelSQL, ModelView, fields)
 from trytond.model.exceptions import (
     AccessError, RequiredValidationError, ValidationError)
@@ -183,14 +183,17 @@
         'product.product', "Product",
         context={
             'company': Eval('company', -1),
             },
         depends=['company'])
     lot = fields.Many2One('stock.lot', "Lot")
 
+    from_location = fields.Many2One('stock.location', "From Location")
+    to_location = fields.Many2One('stock.location', "To Location")
+
     quantity = fields.Float("Quantity", digits='unit')
     unit = fields.Many2One('product.uom', "Unit")
 
     company = fields.Many2One('company.company', "Company")
     date = fields.Date("Date")
     shipment = fields.Reference("Shipment", 'get_shipments')
     document = fields.Function(
@@ -204,36 +207,38 @@
         fields.Many2Many(
             'stock.lot.trace', None, None, "Downward Traces"),
         'get_downward_traces')
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
-        cls._order.insert(0, ('date', 'ASC'))
+        cls._order.insert(0, ('date', None))
 
     @classmethod
     def table_query(cls):
         pool = Pool()
         Move = pool.get('stock.move')
         move = Move.__table__()
         return (
             move.select(
                 *cls._columns(move),
-                where=move.state == 'done'))
+                where=(move.lot != Null) & (move.state == 'done')))
 
     @classmethod
     def _columns(cls, move):
         return [
             move.id.as_('id'),
             move.create_uid.as_('create_uid'),
             move.create_date.as_('create_date'),
             move.write_uid.as_('write_uid'),
             move.write_date.as_('write_date'),
             move.product.as_('product'),
             move.lot.as_('lot'),
+            move.from_location.as_('from_location'),
+            move.to_location.as_('to_location'),
             move.quantity.as_('quantity'),
             move.unit.as_('unit'),
             move.company.as_('company'),
             move.effective_date.as_('date'),
             move.shipment.as_('shipment'),
             ]
 
@@ -256,31 +261,43 @@
 
     @classmethod
     def _is_trace_move(cls, move):
         return move.state == 'done'
 
     @classmethod
     def _trace_move_order_key(cls, move):
-        return (move.effective_date,)
+        return (move.effective_date, move.id)
 
     def get_upward_traces(self, name):
         return list(map(int, sorted(filter(
                         self._is_trace_move, self._get_upward_traces()),
                     key=self._trace_move_order_key)))
 
     def _get_upward_traces(self):
-        return set()
+        pool = Pool()
+        Move = pool.get('stock.move')
+        return set(Move.search([
+                    ('lot', '=', self.lot.id),
+                    ('from_location', '=', self.to_location),
+                    ('effective_date', '>=', self.date),
+                    ]))
 
     def get_downward_traces(self, name):
         return list(map(int, sorted(filter(
                         self._is_trace_move, self._get_downward_traces()),
-                    key=self._trace_move_order_key)))
+                    key=self._trace_move_order_key, reverse=True)))
 
     def _get_downward_traces(self):
-        return set()
+        pool = Pool()
+        Move = pool.get('stock.move')
+        return set(Move.search([
+                    ('lot', '=', self.lot.id),
+                    ('to_location', '=', self.from_location),
+                    ('effective_date', '<=', self.date),
+                    ]))
 
 
 class LotByLocationContext(ModelView):
     'Lot by Location'
     __name__ = 'stock.lots_by_location.context'
     forecast_date = fields.Date(
         'At Date', help=('Allow to compute expected '
@@ -460,28 +477,32 @@
     @ModelView.button
     def do(cls, moves):
         super().do(moves)
         for move in moves:
             move.check_lot()
 
     @classmethod
-    def assign_try(cls, moves, with_childs=True, grouping=('product',)):
+    def assign_try(
+            cls, moves, with_childs=True, grouping=('product',), pblc=None):
         if 'lot' not in grouping:
             moves_with_lot, moves_without_lot = [], []
             for move in moves:
                 if move.lot:
                     moves_with_lot.append(move)
                 else:
                     moves_without_lot.append(move)
             success = super().assign_try(
-                moves_with_lot, with_childs, grouping=grouping + ('lot',))
+                moves_with_lot, with_childs=with_childs,
+                grouping=grouping + ('lot',), pblc=pblc)
             success &= super().assign_try(
-                moves_without_lot, with_childs, grouping=grouping)
+                moves_without_lot, with_childs=with_childs,
+                grouping=grouping, pblc=pblc)
         else:
-            success = super().assign_try(moves, with_childs, grouping)
+            success = super().assign_try(
+                moves, with_childs=with_childs, grouping=grouping, pblc=pblc)
         return success
 
 
 class MoveAddLots(Wizard):
     "Add Lots"
     __name__ = 'stock.move.add.lots'
     start = StateView('stock.move.add.lots.start',
@@ -516,28 +537,40 @@
                     lot_quantity=lang.format_number(lot_quantity, digits),
                     move_quantity=lang.format_number(move_quantity, digits)))
         lots = []
         for line in self.start.lots:
             lot = line.get_lot(self.record)
             lots.append(lot)
         Lot.save(lots)
-        if quantity_remaining:
-            self.record.quantity = quantity_remaining
-            self.record.save()
-        for i, (line, lot) in enumerate(zip(self.start.lots, lots)):
-            if not i and not quantity_remaining:
-                self.record.quantity = line.quantity
-                self.record.lot = lot
+        if hasattr(self.model, 'split'):
+            move = self.record
+            for line, lot in zip(self.start.lots, lots):
+                splits = move.split(line.quantity, self.record.unit, count=1)
+                splits.remove(move)
+                move.lot = lot
+                move.save()
+                if splits:
+                    move, = splits
+                else:
+                    break
+        else:
+            if quantity_remaining:
+                self.record.quantity = quantity_remaining
                 self.record.save()
-            else:
-                with Transaction().set_context(_stock_move_split=True):
-                    self.model.copy([self.record], {
-                            'quantity': line.quantity,
-                            'lot': lot.id,
-                            })
+            for i, (line, lot) in enumerate(zip(self.start.lots, lots)):
+                if not i and not quantity_remaining:
+                    self.record.quantity = line.quantity
+                    self.record.lot = lot
+                    self.record.save()
+                else:
+                    with Transaction().set_context(_stock_move_split=True):
+                        self.model.copy([self.record], {
+                                'quantity': line.quantity,
+                                'lot': lot.id,
+                                })
         return 'end'
 
 
 class MoveAddLotsStart(ModelView):
     "Add Lots"
     __name__ = 'stock.move.add.lots.start'
```

### Comparing `trytond_stock_lot-7.0.1/stock.xml` & `trytond_stock_lot-7.2.0/stock.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_stock_lot-7.0.1/stock.xml` & `trytond_stock_lot-7.2.0/stock.xml`

```diff
@@ -50,37 +50,37 @@
     </record>
     <record model="ir.action.keyword" id="act_lot_form_product_relate_keyword2">
       <field name="keyword">form_relate</field>
       <field name="model">product.template,-1</field>
       <field name="action" ref="act_lot_form_product_relate"/>
     </record>
     <record model="ir.model.access" id="access_lot">
-      <field name="model" search="[('model', '=', 'stock.lot')]"/>
+      <field name="model">stock.lot</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_lot_group_stock">
-      <field name="model" search="[('model', '=', 'stock.lot')]"/>
+      <field name="model">stock.lot</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="lot_upward_traces_button">
+      <field name="model">stock.lot</field>
       <field name="name">upward_traces</field>
       <field name="string">Upward Traces</field>
-      <field name="model" search="[('model', '=', 'stock.lot')]"/>
     </record>
     <record model="ir.model.button" id="lot_downward_traces_button">
+      <field name="model">stock.lot</field>
       <field name="name">downward_traces</field>
       <field name="string">Downward Traces</field>
-      <field name="model" search="[('model', '=', 'stock.lot')]"/>
     </record>
     <record model="ir.ui.view" id="lot_trace_view_tree_upward">
       <field name="model">stock.lot.trace</field>
       <field name="type">tree</field>
       <field name="field_childs">upward_traces</field>
       <field name="name">lot_trace_tree</field>
     </record>
@@ -90,14 +90,15 @@
       <field name="field_childs">downward_traces</field>
       <field name="name">lot_trace_tree</field>
     </record>
     <record model="ir.action.act_window" id="act_lot_trace_upward_relate">
       <field name="name">Upward Traces</field>
       <field name="res_model">stock.lot.trace</field>
       <field name="domain" eval="[('lot', 'in', Eval('active_ids', []))]" pyson="1"/>
+      <field name="order" eval="[('date', 'ASC'), ('id', 'ASC')]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_lot_trace_upward_relate_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="lot_trace_view_tree_upward"/>
       <field name="act_window" ref="act_lot_trace_upward_relate"/>
     </record>
     <record model="ir.action.keyword" id="act_lot_trace_upward_relate_keyword1">
@@ -105,43 +106,44 @@
       <field name="model">stock.lot,-1</field>
       <field name="action" ref="act_lot_trace_upward_relate"/>
     </record>
     <record model="ir.action.act_window" id="act_lot_trace_downward_relate">
       <field name="name">Downward Traces</field>
       <field name="res_model">stock.lot.trace</field>
       <field name="domain" eval="[('lot', 'in', Eval('active_ids', []))]" pyson="1"/>
+      <field name="order" eval="[('date', 'DESC'), ('id', 'DESC')]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_lot_trace_downward_relate_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="lot_trace_view_tree_downward"/>
       <field name="act_window" ref="act_lot_trace_downward_relate"/>
     </record>
     <record model="ir.action.keyword" id="act_lot_trace_downward_relate_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">stock.lot,-1</field>
       <field name="action" ref="act_lot_trace_downward_relate"/>
     </record>
     <record model="ir.rule.group" id="rule_group_lot_trace_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'stock.lot.trace')]"/>
+      <field name="model">stock.lot.trace</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_lot_trace_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_lot_trace_companies"/>
     </record>
     <record model="ir.model.access" id="access_lot_trace">
-      <field name="model" search="[('model', '=', 'stock.lot.trace')]"/>
+      <field name="model">stock.lot.trace</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_lot_trace_group_stock">
-      <field name="model" search="[('model', '=', 'stock.lot.trace')]"/>
+      <field name="model">stock.lot.trace</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="lots_by_location_context_view_form">
@@ -151,22 +153,22 @@
     </record>
     <record model="ir.ui.view" id="lots_by_locations_view_list">
       <field name="model">stock.lots_by_locations</field>
       <field name="type">tree</field>
       <field name="name">lots_by_locations_list</field>
     </record>
     <record model="ir.model.access" id="access_lots_by_locations">
-      <field name="model" search="[('model', '=', 'stock.lots_by_locations')]"/>
+      <field name="model">stock.lots_by_locations</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_lots_by_locations_group_stock">
-      <field name="model" search="[('model', '=', 'stock.lots_by_locations')]"/>
+      <field name="model">stock.lots_by_locations</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.act_window" id="act_lots_by_locations_relate">
@@ -269,17 +271,17 @@
     </record>
     <record model="ir.ui.view" id="move_view_list_shipment">
       <field name="model">stock.move</field>
       <field name="inherit" ref="stock.move_view_list_shipment"/>
       <field name="name">move_tree</field>
     </record>
     <record model="ir.model.button" id="move_add_lots_wizard_button">
+      <field name="model">stock.move</field>
       <field name="name">add_lots_wizard</field>
       <field name="string">Add Lots</field>
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_move_add_lots">
       <field name="name">Add Lots</field>
       <field name="wiz_name">stock.move.add.lots</field>
       <field name="model">stock.move</field>
     </record>
     <record model="ir.ui.view" id="move_add_lots_start_view_form">
@@ -289,45 +291,45 @@
     </record>
     <record model="ir.ui.view" id="move_add_lots_start_lot_view_list">
       <field name="model">stock.move.add.lots.start.lot</field>
       <field name="type">tree</field>
       <field name="name">stock_move_add_lots_start_lot_list</field>
     </record>
     <record model="ir.model.button" id="move_add_lots_start_duplicate_lot_button">
+      <field name="model">stock.move.add.lots.start</field>
       <field name="name">duplicate_lot</field>
       <field name="string">Duplicate Lot</field>
-      <field name="model" search="[('model', '=', 'stock.move.add.lots.start')]"/>
     </record>
     <record model="ir.ui.view" id="period_cache_lot_view_form">
       <field name="model">stock.period.cache.lot</field>
       <field name="type">form</field>
       <field name="name">period_cache_lot_form</field>
     </record>
     <record model="ir.ui.view" id="period_cache_lot_view_list">
       <field name="model">stock.period.cache.lot</field>
       <field name="type">tree</field>
       <field name="name">period_cache_lot_list</field>
     </record>
     <record model="ir.model.access" id="access_period_cache_lot">
-      <field name="model" search="[('model', '=', 'stock.period.cache.lot')]"/>
+      <field name="model">stock.period.cache.lot</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_period_cache_lot_stock">
-      <field name="model" search="[('model', '=', 'stock.period.cache.lot')]"/>
+      <field name="model">stock.period.cache.lot</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_period_cache_lot_admin">
-      <field name="model" search="[('model', '=', 'stock.period.cache.lot')]"/>
+      <field name="model">stock.period.cache.lot</field>
       <field name="group" ref="stock.group_stock_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="inventory_line_view_form">
```

### Comparing `trytond_stock_lot-7.0.1/tests/scenario_stock_lot_assign_try.rst` & `trytond_stock_lot-7.2.0/tests/scenario_stock_lot_assign_try.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 =================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import config, Model, Wizard
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot')
     >>> Inventory = Model.get('stock.inventory')
```

### Comparing `trytond_stock_lot-7.0.1/tests/scenario_stock_lot_move_add.rst` & `trytond_stock_lot-7.2.0/tests/scenario_stock_lot_move_add.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 ===========================
 Stock Lot Move Add Scenario
 ===========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
-    >>> config = activate_modules('stock_lot')
+    >>> modules = ['stock_lot']
+    >>> if globals().get('stock_split', False):
+    ...     modules.append('stock_split')
+    >>> config = activate_modules(modules)
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create product::
@@ -56,20 +59,18 @@
     >>> Lot = Model.get('stock.lot')
     >>> lot2 = Lot(number='02', product=product)
     >>> lot2.save()
 
 Add few lots::
 
     >>> add_lots = move.click('add_lots_wizard')
-    >>> add_lots.form.product== product
-    True
+    >>> assertEqual(add_lots.form.product, product)
     >>> add_lots.form.quantity
     10.0
-    >>> add_lots.form.unit == unit
-    True
+    >>> assertEqual(add_lots.form.unit, unit)
     >>> add_lots.form.quantity_remaining
     10.0
 
     >>> lot = add_lots.form.lots.new()
     >>> lot.quantity
     10.0
     >>> lot.number = '01'
@@ -86,16 +87,15 @@
 
     >>> move, = Move.find([('lot.number', '=', '01')])
     >>> move.quantity
     2.0
     >>> move, = Move.find([('lot.number', '=', '02')])
     >>> move.quantity
     1.0
-    >>> move.lot == lot2
-    True
+    >>> assertEqual(move.lot, lot2)
     >>> move, = Move.find([('lot', '=', None)])
     >>> move.quantity
     7.0
 
 Add lot to remaining::
 
     >>> add_lots = move.click('add_lots_wizard')
```

### Comparing `trytond_stock_lot-7.0.1/tests/scenario_stock_lot_number.rst` & `trytond_stock_lot-7.2.0/tests/scenario_stock_lot_number.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 =========================
 Stock Lot Number Scenario
 =========================
 
 Imports::
 
-    >>> from decimal import Decimal
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot')
 
 Create lot sequence::
 
@@ -31,16 +30,15 @@
 Create product::
 
     >>> ProductUom = Model.get('product.uom')
     >>> ProductTemplate = Model.get('product.template')
     >>> unit, = ProductUom.find([('name', '=', 'Unit')])
 
     >>> template = ProductTemplate()
-    >>> template.lot_sequence == sequence
-    True
+    >>> assertEqual(template.lot_sequence, sequence)
     >>> template.name = 'Product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.save()
     >>> product, = template.products
 
 Create lot without number::
```

### Comparing `trytond_stock_lot-7.0.1/tests/scenario_stock_lot_shipment_in.rst` & `trytond_stock_lot-7.2.0/tests/scenario_stock_lot_shipment_in.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ==============================
 Stock Lot Shipment In Scenario
 ==============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot')
 
     >>> Location = Model.get('stock.location')
     >>> Lot = Model.get('stock.lot')
@@ -75,23 +75,22 @@
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
 
 Change lot and try to finish::
 
     >>> incoming_move, = shipment.inventory_moves
-    >>> incoming_move.lot == lot1
-    True
+    >>> assertEqual(incoming_move.lot, lot1)
     >>> incoming_move.lot = lot2
-    >>> shipment.click('done')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('do')
     Traceback (most recent call last):
         ...
     ShipmentCheckQuantityWarning: ...
     >>> incoming_move.reload()
     >>> incoming_move.lot = lot1
     >>> incoming_move.save()
 
 Finish the shipment::
 
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
```

### Comparing `trytond_stock_lot-7.0.1/tests/scenario_stock_lot_shipment_out.rst` & `trytond_stock_lot-7.2.0/tests/scenario_stock_lot_shipment_out.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Lot Shipment Out Scenario
 ===============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import config, Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot')
 
@@ -58,15 +58,15 @@
     >>> shipment_out = ShipmentOut()
     >>> shipment_out.planned_date = today
     >>> shipment_out.customer = customer
     >>> shipment_out.warehouse = warehouse_loc
     >>> shipment_out.company = company
     >>> move = shipment_out.outgoing_moves.new()
     >>> move.product = product
-    >>> move.unit =unit
+    >>> move.unit = unit
     >>> move.quantity = 10
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> move.company = company
     >>> move.unit_price = Decimal('1')
     >>> move.currency = company.currency
     >>> shipment_out.save()
@@ -95,20 +95,20 @@
     'assigned'
     >>> len(shipment_out.outgoing_moves)
     1
 
 Check the inventory moves origin::
 
     >>> outgoing_move, = shipment_out.outgoing_moves
-    >>> all(m.origin == outgoing_move for m in shipment_out.inventory_moves)
-    True
+    >>> for move in shipment_out.inventory_moves:
+    ...     assertEqual(move.origin, outgoing_move)
 
 Try to pick without lot::
 
-    >>> shipment_out.click('pick')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment_out.click('pick')
     Traceback (most recent call last):
         ...
     RequiredValidationError: ...
 
 Set 2 lots::
 
     >>> Lot = Model.get('stock.lot')
@@ -133,16 +133,16 @@
     ...     quantity = lot_quantities.setdefault(number, 0)
     ...     lot_quantities[number] += move.quantity
     >>> sorted(lot_quantities.items())
     [('', 0.0), ('00001', 7.0), ('00002', 3.0)]
 
 Check the inventory moves have an outgoing move origin with the same lot::
 
-    >>> all(m.lot == m.origin.lot for m in shipment_out.inventory_moves)
-    True
+    >>> for move in shipment_out.inventory_moves:
+    ...     assertEqual(move.lot, move.origin.lot)
 
 Pack the shipment and return to pick::
 
     >>> shipment_out.click('pack')
     >>> shipment_out.state
     'packed'
     >>> len(shipment_out.outgoing_moves)
@@ -151,9 +151,9 @@
     >>> shipment_out.state
     'picked'
     >>> len(shipment_out.outgoing_moves)
     2
 
 Check the inventory moves still have an outgoing move origin with the same lot::
 
-    >>> all(m.lot == m.origin.lot for m in shipment_out.inventory_moves)
-    True
+    >>> for move in shipment_out.inventory_moves:
+    ...     assertEqual(move.lot, move.origin.lot)
```

### Comparing `trytond_stock_lot-7.0.1/tests/scenario_stock_lot_shipment_out_internal.rst` & `trytond_stock_lot-7.2.0/tests/scenario_stock_lot_shipment_out_internal.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertTrue
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
@@ -58,18 +57,16 @@
 
 Create Internal Shipment with lead time::
 
     >>> shipment = Shipment()
     >>> shipment.planned_date = tomorrow
     >>> shipment.from_location = warehouse1.storage_location
     >>> shipment.to_location = warehouse2.storage_location
-    >>> bool(shipment.transit_location)
-    True
-    >>> shipment.planned_start_date == today
-    True
+    >>> assertTrue(shipment.transit_location)
+    >>> assertEqual(shipment.planned_start_date, today)
     >>> move = shipment.moves.new()
     >>> move.product = product
     >>> move.quantity = 3
     >>> move.from_location = shipment.from_location
     >>> move.to_location = shipment.to_location
     >>> shipment.save()
 
@@ -101,16 +98,16 @@
 
     >>> len(shipment.incoming_moves)
     1
 
 Check the inventory moves origin::
 
     >>> incoming_move, = shipment.incoming_moves
-    >>> all(m.origin == incoming_move for m in shipment.outgoing_moves)
-    True
+    >>> for move in shipment.outgoing_moves:
+    ...     assertEqual(move.origin, incoming_move)
 
 Set 2 lots::
 
     >>> for i, move in enumerate(shipment.outgoing_moves, start=1):
     ...     lot = Lot(number='%05i' % i, product=move.product)
     ...     lot.save()
     ...     move.lot = lot
@@ -132,9 +129,9 @@
     ...     quantity = lot_quantities.setdefault(number, 0)
     ...     lot_quantities[number] += move.quantity
     >>> sorted(lot_quantities.items())
     [('', 0.0), ('00001', 1.0), ('00002', 2.0)]
 
 Check the outgoing moves have an incoming move origin with the same lot::
 
-    >>> all(m.lot == m.origin.lot for m in shipment.outgoing_moves)
-    True
+    >>> for move in shipment.outgoing_moves:
+    ...     assertEqual(move.lot, move.origin.lot)
```

### Comparing `trytond_stock_lot-7.0.1/tests/test_module.py` & `trytond_stock_lot-7.2.0/tests/test_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 from trytond.transaction import Transaction
 
 
 class StockLotTestCase(CompanyTestMixin, ModuleTestCase):
     'Test Stock Lot module'
     module = 'stock_lot'
+    extras = ['stock_split']
 
     @with_transaction()
     def test_products_by_location(self):
         'Test products_by_location'
         pool = Pool()
         Uom = pool.get('product.uom')
         Template = pool.get('product.template')
```

### Comparing `trytond_stock_lot-7.0.1/tox.ini` & `trytond_stock_lot-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/PKG-INFO` & `trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-lot
-Version: 7.0.1
+Name: trytond_stock_lot
+Version: 7.2.0
 Summary: Tryton module for lot of products
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
@@ -49,19 +49,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_split<7.3,>=7.2; extra == "test"
 
 Stock Lot Module
 ################
 
 The stock lot module defines lot of products.
 
 Lot
```

### Comparing `trytond_stock_lot-7.0.1/trytond_stock_lot.egg-info/SOURCES.txt` & `trytond_stock_lot-7.2.0/trytond_stock_lot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 ir.xml
@@ -49,14 +48,15 @@
 ./tests/__init__.py
 ./tests/scenario_stock_lot_assign_try.rst
 ./tests/scenario_stock_lot_move_add.rst
 ./tests/scenario_stock_lot_number.rst
 ./tests/scenario_stock_lot_shipment_in.rst
 ./tests/scenario_stock_lot_shipment_out.rst
 ./tests/scenario_stock_lot_shipment_out_internal.rst
+./tests/scenario_stock_lot_trace.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/inventory_line_form.xml
 ./view/inventory_line_tree.xml
 ./view/lot_by_location_context_form.xml
 ./view/lot_by_warehouse_context_form.xml
 ./view/lot_form.xml
@@ -96,19 +96,21 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_stock_lot_assign_try.rst
+tests/scenario_stock_lot_move_add.json
 tests/scenario_stock_lot_move_add.rst
 tests/scenario_stock_lot_number.rst
 tests/scenario_stock_lot_shipment_in.rst
 tests/scenario_stock_lot_shipment_out.rst
 tests/scenario_stock_lot_shipment_out_internal.rst
+tests/scenario_stock_lot_trace.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_stock_lot.egg-info/PKG-INFO
 trytond_stock_lot.egg-info/SOURCES.txt
 trytond_stock_lot.egg-info/dependency_links.txt
 trytond_stock_lot.egg-info/entry_points.txt
 trytond_stock_lot.egg-info/not-zip-safe
```

### Comparing `trytond_stock_lot-7.0.1/view/lot_by_warehouse_context_form.xml` & `trytond_stock_lot-7.2.0/view/lot_by_warehouse_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/view/lot_form.xml` & `trytond_stock_lot-7.2.0/view/lot_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.0.1/view/stock_move_add_lots_start_form.xml` & `trytond_stock_lot-7.2.0/view/stock_move_add_lots_start_form.xml`

 * *Files identical despite different names*

