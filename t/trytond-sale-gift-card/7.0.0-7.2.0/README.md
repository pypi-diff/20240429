# Comparing `tmp/trytond_sale_gift_card-7.0.0.tar.gz` & `tmp/trytond_sale_gift_card-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_gift_card-7.0.0.tar", last modified: Mon Oct 30 17:37:55 2023, max compression
+gzip compressed data, was "trytond_sale_gift_card-7.2.0.tar", last modified: Mon Apr 29 15:47:56 2024, max compression
```

## Comparing `trytond_sale_gift_card-7.0.0.tar` & `trytond_sale_gift_card-7.2.0.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:55.117745 trytond_sale_gift_card-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:17.000000 trytond_sale_gift_card-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      753 2023-10-30 17:12:01.000000 trytond_sale_gift_card-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:12:00.000000 trytond_sale_gift_card-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2844 2023-10-30 17:37:55.114412 trytond_sale_gift_card-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3420 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:55.114412 trytond_sale_gift_card-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:17.000000 trytond_sale_gift_card-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:17.000000 trytond_sale_gift_card-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1042 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)      553 2023-10-07 15:40:36.000000 trytond_sale_gift_card-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30315 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/gift_card.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:55.107745 trytond_sale_gift_card-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7467 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7601 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7486 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7370 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5993 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5952 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7160 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5953 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2023-10-30 16:47:45.000000 trytond_sale_gift_card-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-10-24 07:56:52.000000 trytond_sale_gift_card-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2459 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    18835 2023-10-07 17:14:58.000000 trytond_sale_gift_card-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7886 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:37:55.117745 trytond_sale_gift_card-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4595 2023-10-27 17:38:49.000000 trytond_sale_gift_card-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2009 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:55.111078 trytond_sale_gift_card-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5456 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/tests/scenario_sale_gift_card.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3729 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/tests/scenario_sale_gift_card_goods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6144 2023-08-13 15:26:13.000000 trytond_sale_gift_card-7.0.0/tests/scenario_sale_point_gift_card.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_gift_card-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-10-30 17:11:57.000000 trytond_sale_gift_card-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:55.114412 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2844 2023-10-30 17:37:54.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2587 2023-10-30 17:37:55.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:37:54.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:37:54.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:37:54.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:37:54.000000 trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:37:55.111078 trytond_sale_gift_card-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      509 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/account_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/gift_card_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/gift_card_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/sale_point_sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/sale_point_sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/sale_point_sale_pay_gift_card_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2024-04-29 15:25:12.000000 trytond_sale_gift_card-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:25:12.000000 trytond_sale_gift_card-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2844 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3420 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.700980 trytond_sale_gift_card-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:25.000000 trytond_sale_gift_card-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1042 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      553 2024-02-04 18:51:26.000000 trytond_sale_gift_card-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30315 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/gift_card.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.704314 trytond_sale_gift_card-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7467 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7601 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7486 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7370 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5993 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5952 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7160 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5953 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2024-02-04 18:51:26.000000 trytond_sale_gift_card-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2459 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    18775 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7817 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4595 2024-03-17 11:01:36.000000 trytond_sale_gift_card-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2009 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.704314 trytond_sale_gift_card-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5320 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3655 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card_goods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6138 2024-04-22 12:14:36.000000 trytond_sale_gift_card-7.2.0/tests/scenario_sale_point_gift_card.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:25.000000 trytond_sale_gift_card-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-29 15:25:07.000000 trytond_sale_gift_card-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2844 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2569 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      509 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/account_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/gift_card_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/gift_card_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_point_sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_point_sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_point_sale_pay_gift_card_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/template_form.xml
```

### Comparing `trytond_sale_gift_card-7.0.0/CHANGELOG` & `trytond_sale_gift_card-7.2.0/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_sale_gift_card-7.0.0/COPYRIGHT` & `trytond_sale_gift_card-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2023 B2CK
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 B2CK
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_gift_card-7.0.0/LICENSE` & `trytond_sale_gift_card-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/PKG-INFO` & `trytond_sale_gift_card-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_gift_card
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to manage gift cards
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
@@ -47,25 +47,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
 
 #####################
 Sale Gift Card Module
 #####################
 
 The *Sale Gift Card Module* manages the selling and redeeming of gift cards.
```

### Comparing `trytond_sale_gift_card-7.0.0/__init__.py` & `trytond_sale_gift_card-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/account.py` & `trytond_sale_gift_card-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/account.xml` & `trytond_sale_gift_card-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/doc/conf.py` & `trytond_sale_gift_card-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_gift_card-7.0.0/doc/design.rst` & `trytond_sale_gift_card-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/doc/usage.rst` & `trytond_sale_gift_card-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/email.html` & `trytond_sale_gift_card-7.2.0/email.html`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/exceptions.py` & `trytond_sale_gift_card-7.2.0/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/gift_card.fodt` & `trytond_sale_gift_card-7.2.0/gift_card.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/bg.po` & `trytond_sale_gift_card-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/ca.po` & `trytond_sale_gift_card-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/cs.po` & `trytond_sale_gift_card-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/de.po` & `trytond_sale_gift_card-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/es.po` & `trytond_sale_gift_card-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/es_419.po` & `trytond_sale_gift_card-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/et.po` & `trytond_sale_gift_card-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/fa.po` & `trytond_sale_gift_card-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/fi.po` & `trytond_sale_gift_card-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/fr.po` & `trytond_sale_gift_card-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/hu.po` & `trytond_sale_gift_card-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/id.po` & `trytond_sale_gift_card-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/it.po` & `trytond_sale_gift_card-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/lo.po` & `trytond_sale_gift_card-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/lt.po` & `trytond_sale_gift_card-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/nl.po` & `trytond_sale_gift_card-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/pl.po` & `trytond_sale_gift_card-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/pt.po` & `trytond_sale_gift_card-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/ro.po` & `trytond_sale_gift_card-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/ru.po` & `trytond_sale_gift_card-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/sl.po` & `trytond_sale_gift_card-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/tr.po` & `trytond_sale_gift_card-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/uk.po` & `trytond_sale_gift_card-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/locale/zh_CN.po` & `trytond_sale_gift_card-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/message.xml` & `trytond_sale_gift_card-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/product.py` & `trytond_sale_gift_card-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/sale.py` & `trytond_sale_gift_card-7.2.0/sale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from email.header import Header
 
 from sql import Null
 from sql.functions import CharLength
 from sql.operators import Equal
 
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import Exclude, ModelSQL, ModelView, Workflow, fields
 from trytond.modules.company.model import CompanyValueMixin
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, Id
 from trytond.report import Report, get_email
-from trytond.sendmail import sendmail_transactional
+from trytond.sendmail import send_message_transactional
 from trytond.tools.email_ import (
     EmailNotValidError, set_from_header, validate_email)
 from trytond.transaction import Transaction
 from trytond.wizard import Button, StateTransition, StateView
 
 from .exceptions import GiftCardLineValidationError
 
@@ -194,16 +193,16 @@
             languages = gift_card._languages
             if not languages:
                 languages.append(Lang.get())
             msg, title = get_email(
                 'sale.gift_card.email', gift_card, languages)
             set_from_header(msg, from_cfg, from_ or from_cfg)
             msg['To'] = email
-            msg['Subject'] = Header(title, 'utf-8')
-            sendmail_transactional(from_cfg, [email], msg, strict=True)
+            msg['Subject'] = title
+            send_message_transactional(msg, strict=True)
 
 
 class GiftCardReport(Report):
     __name__ = 'sale.gift_card'
 
     @classmethod
     def _get_records(cls, ids, model, data):
```

### Comparing `trytond_sale_gift_card-7.0.0/sale.xml` & `trytond_sale_gift_card-7.2.0/sale.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale_gift_card-7.0.0/sale.xml` & `trytond_sale_gift_card-7.2.0/sale.xml`

```diff
@@ -63,31 +63,31 @@
     <record model="ir.action.act_window.domain" id="act_gift_card_form_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="act_window" ref="act_gift_card_form"/>
     </record>
     <menuitem parent="sale.menu_sale" action="act_gift_card_form" sequence="50" id="menu_gift_card_form"/>
     <record model="ir.model.access" id="access_gift_card">
-      <field name="model" search="[('model', '=', 'sale.gift_card')]"/>
+      <field name="model">sale.gift_card</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_gift_card_admin">
-      <field name="model" search="[('model', '=', 'sale.gift_card')]"/>
+      <field name="model">sale.gift_card</field>
       <field name="group" ref="group_gift_card_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_gift_card_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.gift_card')]"/>
+      <field name="model">sale.gift_card</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_gift_card_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_gift_card_companies"/>
     </record>
     <record model="ir.action.report" id="report_gift_card_email">
```

### Comparing `trytond_sale_gift_card-7.0.0/setup.py` & `trytond_sale_gift_card-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/stock.py` & `trytond_sale_gift_card-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/tests/scenario_sale_gift_card.rst` & `trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 =======================
 Sale Gift Card Scenario
 =======================
 
 Imports::
 
-    >>> import re
     >>> from decimal import Decimal
+    >>> from unittest.mock import patch
+
     >>> from proteus import Model, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.sale_gift_card import sale
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
-Patch sendmail_transactional::
+Patch send_message_transactional::
 
-    >>> from unittest.mock import patch
-    >>> from trytond.modules.sale_gift_card import sale
     >>> smtp_calls = patch.object(
-    ...     sale, 'sendmail_transactional').start()
+    ...     sale, 'send_message_transactional').start()
 
 Activate modules::
 
     >>> config = activate_modules('sale_gift_card')
 
     >>> Account = Model.get('account.account')
     >>> AccountConfig = Model.get('account.configuration')
@@ -125,43 +123,38 @@
 
 Check gift cards::
 
     >>> cards = GiftCard.find([])
     >>> len(cards)
     2
     >>> card = cards[-1]
-    >>> card.product == gift_card
-    True
+    >>> assertEqual(card.product, gift_card)
     >>> card.value
     Decimal('50.00')
     >>> bool(card.origin)
     True
     >>> bool(card.spent_on)
     False
     >>> smtp_calls.call_count
     2
-    >>> from_, to, msg = smtp_calls.call_args[0]
-    >>> to
-    ['customer@example.com']
-    >>> msg = msg.get_payload(0).get_payload(decode=True).decode('utf-8')
-    >>> card.number in msg
+    >>> msg, = smtp_calls.call_args[0]
+    >>> card.number in msg.get_body().get_content()
     True
 
 Print gift cards::
 
     >>> gift_card_report = Report('sale.gift_card')
     >>> bool(gift_card_report.execute([sale]))
     True
 
 Check invoice::
 
     >>> invoice, = sale.invoices
     >>> line, = invoice.lines
-    >>> line.account == gift_card_revenue
-    True
+    >>> assertEqual(line.account, gift_card_revenue)
 
 Redeem a gift card to buy a product::
 
     >>> sale = Sale()
     >>> sale.party = customer2
     >>> line = sale.lines.new()
     >>> line.product = product
@@ -178,22 +171,20 @@
     >>> sale.click('confirm')
     >>> sale.state
     'processing'
 
 Check gift card::
 
     >>> card.reload()
-    >>> card.spent_on == sale
-    True
+    >>> assertEqual(card.spent_on, sale)
 
 Check the invoice::
 
     >>> invoice, = sale.invoices
     >>> len(invoice.lines)
     2
     >>> invoice.total_amount
     Decimal('50.00')
     >>> gift_card_line, = [l for l in invoice.lines if l.product == gift_card]
     >>> gift_card_line.quantity
     -1.0
-    >>> gift_card_line.account == gift_card_revenue
-    True
+    >>> assertEqual(gift_card_line.account, gift_card_revenue)
```

### Comparing `trytond_sale_gift_card-7.0.0/tests/scenario_sale_gift_card_goods.rst` & `trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card_goods.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 =============================
 Sale Gift Card Goods Scenario
 =============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_gift_card')
 
     >>> Account = Model.get('account.account')
     >>> AccountConfig = Model.get('account.configuration')
@@ -105,27 +104,26 @@
     >>> len(cards)
     0
 
 Check invoice::
 
     >>> invoice, = sale.invoices
     >>> line, = invoice.lines
-    >>> line.account == gift_card_revenue
-    True
+    >>> assertEqual(line.account, gift_card_revenue)
 
 Ship the gift card::
 
     >>> shipment, = sale.shipments
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('do')
     Traceback (most recent call last):
         ...
     MoveGiftCardValidationError: ...
     >>> move, = shipment.outgoing_moves
     >>> gift_card = move.gift_cards.new(product=gift_card)
     >>> gift_card.number = "1234"
     >>> gift_card.value
     Decimal('20.00')
     >>> move.save()
-    >>> shipment.click('done')
+    >>> shipment.click('do')
```

### Comparing `trytond_sale_gift_card-7.0.0/tests/scenario_sale_point_gift_card.rst` & `trytond_sale_gift_card-7.2.0/tests/scenario_sale_point_gift_card.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 Sale Point Gift Card Scenario
 =============================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model, Report
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(['sale_gift_card', 'sale_point'])
 
     >>> Account = Model.get('account.account')
     >>> AccountConfig = Model.get('account.configuration')
@@ -169,16 +168,15 @@
     'done'
 
 Check gift card::
 
     >>> gift_card, = GiftCard.find([])
     >>> gift_card.value
     Decimal('100.00')
-    >>> gift_card.currency == sale.currency
-    True
+    >>> assertEqual(gift_card.currency, sale.currency)
 
 Print gift card::
 
     >>> gift_card_report = Report('sale.gift_card')
     >>> bool(gift_card_report.execute([sale]))
     True
 
@@ -209,15 +207,14 @@
     'done'
     >>> sale.total
     Decimal('150.00')
 
 Check gift card::
 
     >>> gift_card.reload()
-    >>> gift_card.spent_on == sale
-    True
+    >>> assertEqual(gift_card.spent_on, sale)
 
 Post sale::
 
     >>> sale.click('post')
     >>> sale.state
     'posted'
```

### Comparing `trytond_sale_gift_card-7.0.0/tox.ini` & `trytond_sale_gift_card-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/PKG-INFO` & `trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-gift-card
-Version: 7.0.0
+Name: trytond_sale_gift_card
+Version: 7.2.0
 Summary: Tryton module to manage gift cards
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
@@ -47,25 +47,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
 
 #####################
 Sale Gift Card Module
 #####################
 
 The *Sale Gift Card Module* manages the selling and redeeming of gift cards.
```

### Comparing `trytond_sale_gift_card-7.0.0/trytond_sale_gift_card.egg-info/SOURCES.txt` & `trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_sale_gift_card-7.0.0/view/gift_card_form.xml` & `trytond_sale_gift_card-7.2.0/view/gift_card_form.xml`

 * *Files identical despite different names*

