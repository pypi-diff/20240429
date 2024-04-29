# Comparing `tmp/trytond_carrier_carriage-7.0.0.tar.gz` & `tmp/trytond_carrier_carriage-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_carriage-7.0.0.tar", last modified: Mon Oct 30 17:27:51 2023, max compression
+gzip compressed data, was "trytond_carrier_carriage-7.2.0.tar", last modified: Mon Apr 29 15:38:42 2024, max compression
```

## Comparing `trytond_carrier_carriage-7.0.0.tar` & `trytond_carrier_carriage-7.2.0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:51.208198 trytond_carrier_carriage-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:23:00.000000 trytond_carrier_carriage-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:05:15.000000 trytond_carrier_carriage-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:05:15.000000 trytond_carrier_carriage-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2994 2023-10-30 17:27:51.208198 trytond_carrier_carriage-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      974 2023-10-24 07:56:52.000000 trytond_carrier_carriage-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:51.204865 trytond_carrier_carriage-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:23:00.000000 trytond_carrier_carriage-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1775 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:00.000000 trytond_carrier_carriage-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-06-10 11:39:56.000000 trytond_carrier_carriage-7.0.0/incoterm.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5296 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/incoterm.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:51.201532 trytond_carrier_carriage-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7050 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7545 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7151 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7107 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5887 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6950 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-30 16:47:45.000000 trytond_carrier_carriage-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8490 2023-10-27 17:38:49.000000 trytond_carrier_carriage-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:27:51.208198 trytond_carrier_carriage-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4834 2023-10-27 17:38:49.000000 trytond_carrier_carriage-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7851 2023-10-27 17:38:49.000000 trytond_carrier_carriage-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3075 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:51.201532 trytond_carrier_carriage-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4796 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/tests/scenario_carrier_carriage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_carrier_carriage-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-10-30 17:05:11.000000 trytond_carrier_carriage-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:51.204865 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2994 2023-10-30 17:27:50.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2213 2023-10-30 17:27:51.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:27:50.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:27:50.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-10-30 17:27:50.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:27:50.000000 trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:51.204865 trytond_carrier_carriage-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      580 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/sale_carriage_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/sale_carriage_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      746 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/shipment_carriage_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/shipment_carriage_form_sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/shipment_carriage_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/shipment_carriage_list_sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.0.0/view/shipment_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:42.332146 trytond_carrier_carriage-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:18:25.000000 trytond_carrier_carriage-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:18:24.000000 trytond_carrier_carriage-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2985 2024-04-29 15:38:42.332146 trytond_carrier_carriage-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      974 2024-02-04 18:51:26.000000 trytond_carrier_carriage-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:42.325480 trytond_carrier_carriage-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_carrier_carriage-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1775 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:06.000000 trytond_carrier_carriage-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2024-01-27 09:58:52.000000 trytond_carrier_carriage-7.2.0/incoterm.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5296 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/incoterm.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:42.328813 trytond_carrier_carriage-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7050 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7545 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7151 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7107 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5887 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6950 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:22.000000 trytond_carrier_carriage-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8490 2024-04-26 08:56:10.000000 trytond_carrier_carriage-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:42.332146 trytond_carrier_carriage-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4825 2024-04-27 16:30:39.000000 trytond_carrier_carriage-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7847 2024-04-27 16:30:39.000000 trytond_carrier_carriage-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3029 2024-04-27 16:30:39.000000 trytond_carrier_carriage-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:42.328813 trytond_carrier_carriage-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4773 2024-04-27 16:30:39.000000 trytond_carrier_carriage-7.2.0/tests/scenario_carrier_carriage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:06.000000 trytond_carrier_carriage-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-29 15:18:20.000000 trytond_carrier_carriage-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:42.328813 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2985 2024-04-29 15:38:41.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2195 2024-04-29 15:38:42.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:41.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:38:41.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2024-04-29 15:38:41.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:41.000000 trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:42.328813 trytond_carrier_carriage-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      580 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/sale_carriage_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/sale_carriage_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      746 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/shipment_carriage_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/shipment_carriage_form_sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/shipment_carriage_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/shipment_carriage_list_sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_carrier_carriage-7.2.0/view/shipment_form.xml
```

### Comparing `trytond_carrier_carriage-7.0.0/COPYRIGHT` & `trytond_carrier_carriage-7.2.0/COPYRIGHT`

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

### Comparing `trytond_carrier_carriage-7.0.0/LICENSE` & `trytond_carrier_carriage-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/PKG-INFO` & `trytond_carrier_carriage-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_carriage
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to support multiple carrier
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-carrier-carriage
+Project-URL: Documentation, https://docs.tryton.org/modules-carrier-carriage
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier carriage shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,24 +47,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_incoterm<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_incoterm<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 #######################
 Carrier Carriage Module
 #######################
 
 The *Carrier Carriage Module* extends the support of carrier by adding carriers
 before and after the main carrier.
```

### Comparing `trytond_carrier_carriage-7.0.0/__init__.py` & `trytond_carrier_carriage-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/doc/conf.py` & `trytond_carrier_carriage-7.2.0/doc/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_carrier_carriage-7.0.0/doc/design.rst` & `trytond_carrier_carriage-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/incoterm.py` & `trytond_carrier_carriage-7.2.0/incoterm.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/incoterm.xml` & `trytond_carrier_carriage-7.2.0/incoterm.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/bg.po` & `trytond_carrier_carriage-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/ca.po` & `trytond_carrier_carriage-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/cs.po` & `trytond_carrier_carriage-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/de.po` & `trytond_carrier_carriage-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/es.po` & `trytond_carrier_carriage-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/es_419.po` & `trytond_carrier_carriage-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/et.po` & `trytond_carrier_carriage-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/fa.po` & `trytond_carrier_carriage-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/fi.po` & `trytond_carrier_carriage-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/fr.po` & `trytond_carrier_carriage-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/hu.po` & `trytond_carrier_carriage-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/id.po` & `trytond_carrier_carriage-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/it.po` & `trytond_carrier_carriage-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/lo.po` & `trytond_carrier_carriage-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/lt.po` & `trytond_carrier_carriage-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/nl.po` & `trytond_carrier_carriage-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/pl.po` & `trytond_carrier_carriage-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/pt.po` & `trytond_carrier_carriage-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/ro.po` & `trytond_carrier_carriage-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/ru.po` & `trytond_carrier_carriage-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/sl.po` & `trytond_carrier_carriage-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/tr.po` & `trytond_carrier_carriage-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/uk.po` & `trytond_carrier_carriage-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/locale/zh_CN.po` & `trytond_carrier_carriage-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/sale.py` & `trytond_carrier_carriage-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/sale.xml` & `trytond_carrier_carriage-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/setup.py` & `trytond_carrier_carriage-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-carrier-carriage'),
+            'https://docs.tryton.org/modules-carrier-carriage'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton carrier carriage shipment cost',
     package_dir={'trytond.modules.carrier_carriage': '.'},
     packages=(
         ['trytond.modules.carrier_carriage']
```

### Comparing `trytond_carrier_carriage-7.0.0/stock.py` & `trytond_carrier_carriage-7.2.0/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,30 +178,30 @@
 
 
 class _ShipmentOutMixin(_ShipmentMixin):
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, shipments):
+    def do(cls, shipments):
         pool = Pool()
         Carriage = pool.get('stock.shipment.carriage')
         has_cost_sale = hasattr(Carriage, 'cost_sale')
         carriages = []
         for shipment in shipments:
             for carriage in shipment.carriages:
                 carriage.cost = carriage.cost_used
                 carriage.cost_currency = carriage.cost_currency_used
                 if has_cost_sale:
                     carriage.cost_sale = carriage.cost_sale_used
                     carriage.cost_sale_currency = (
                         carriage.cost_sale_currency_used)
                 carriages.append(carriage)
         Carriage.save(carriages)
-        super().done(shipments)
+        super().do(shipments)
 
 
 class ShipmentOut(_ShipmentOutMixin, metaclass=PoolMeta):
     __name__ = 'stock.shipment.out'
 
 
 class ShipmentOutReturn(_ShipmentOutMixin, metaclass=PoolMeta):
```

### Comparing `trytond_carrier_carriage-7.0.0/stock.xml` & `trytond_carrier_carriage-7.2.0/stock.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_carrier_carriage-7.0.0/stock.xml` & `trytond_carrier_carriage-7.2.0/stock.xml`

```diff
@@ -10,22 +10,22 @@
     </record>
     <record model="ir.ui.view" id="shipment_carriage_view_list">
       <field name="model">stock.shipment.carriage</field>
       <field name="type">tree</field>
       <field name="name">shipment_carriage_list</field>
     </record>
     <record model="ir.model.access" id="access_shipment_carriage">
-      <field name="model" search="[('model', '=', 'stock.shipment.carriage')]"/>
+      <field name="model">stock.shipment.carriage</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shipment_carriage_group_stock">
-      <field name="model" search="[('model', '=', 'stock.shipment.carriage')]"/>
+      <field name="model">stock.shipment.carriage</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="shipment_out_view_form">
```

### Comparing `trytond_carrier_carriage-7.0.0/tests/scenario_carrier_carriage.rst` & `trytond_carrier_carriage-7.2.0/tests/scenario_carrier_carriage.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 Carrier Carriage Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['carrier_carriage', 'sale_shipment_cost'])
 
     >>> Carrier = Model.get('carrier')
     >>> Party = Model.get('party.party')
@@ -123,35 +121,33 @@
     >>> sale.click('process')
     >>> sale.state
     'processing'
 
 Check shipment::
 
     >>> shipment, = sale.shipments
-    >>> shipment.carrier == carrier1
-    True
+    >>> assertEqual(shipment.carrier, carrier1)
     >>> shipment.cost_used
     Decimal('2.0000')
     >>> shipment.cost_sale_used
     Decimal('3.0000')
 
     >>> carriage, = shipment.before_carriages
-    >>> carriage.carrier == carrier2
-    True
+    >>> assertEqual(carriage.carrier, carrier2)
     >>> carriage.cost_used
     Decimal('1.0000')
     >>> carriage.cost_sale_used
     Decimal('2.0000')
 
 Send products::
 
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> shipment.cost_invoice_line.amount
     Decimal('3.00')
     >>> carriage, = shipment.before_carriages
     >>> carriage.cost_invoice_line.amount
```

### Comparing `trytond_carrier_carriage-7.0.0/tox.ini` & `trytond_carrier_carriage-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/PKG-INFO` & `trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-carrier-carriage
-Version: 7.0.0
+Name: trytond_carrier_carriage
+Version: 7.2.0
 Summary: Tryton module to support multiple carrier
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-carrier-carriage
+Project-URL: Documentation, https://docs.tryton.org/modules-carrier-carriage
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier carriage shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,24 +47,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_incoterm<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_incoterm<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 #######################
 Carrier Carriage Module
 #######################
 
 The *Carrier Carriage Module* extends the support of carrier by adding carriers
 before and after the main carrier.
```

### Comparing `trytond_carrier_carriage-7.0.0/trytond_carrier_carriage.egg-info/SOURCES.txt` & `trytond_carrier_carriage-7.2.0/trytond_carrier_carriage.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_carrier_carriage-7.0.0/view/sale_carriage_form.xml` & `trytond_carrier_carriage-7.2.0/view/sale_carriage_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_carriage-7.0.0/view/shipment_carriage_form.xml` & `trytond_carrier_carriage-7.2.0/view/shipment_carriage_form.xml`

 * *Files identical despite different names*

