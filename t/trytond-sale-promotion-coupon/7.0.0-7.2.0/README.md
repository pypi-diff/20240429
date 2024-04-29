# Comparing `tmp/trytond_sale_promotion_coupon-7.0.0.tar.gz` & `tmp/trytond_sale_promotion_coupon-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_promotion_coupon-7.0.0.tar", last modified: Mon Oct 30 17:39:32 2023, max compression
+gzip compressed data, was "trytond_sale_promotion_coupon-7.2.0.tar", last modified: Mon Apr 29 15:49:17 2024, max compression
```

## Comparing `trytond_sale_promotion_coupon-7.0.0.tar` & `trytond_sale_promotion_coupon-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:32.941545 trytond_sale_promotion_coupon-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:23:20.000000 trytond_sale_promotion_coupon-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-10-30 17:12:59.000000 trytond_sale_promotion_coupon-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:12:58.000000 trytond_sale_promotion_coupon-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2980 2023-10-30 17:39:32.938212 trytond_sale_promotion_coupon-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      611 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:32.938212 trytond_sale_promotion_coupon-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:23:20.000000 trytond_sale_promotion_coupon-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:20.000000 trytond_sale_promotion_coupon-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:32.934878 trytond_sale_promotion_coupon-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2074 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2216 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2302 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2112 2023-10-30 16:47:45.000000 trytond_sale_promotion_coupon-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2006 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1741 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1731 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2059 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-10-28 12:11:25.000000 trytond_sale_promotion_coupon-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7769 2023-08-13 15:26:13.000000 trytond_sale_promotion_coupon-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1690 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:39:32.941545 trytond_sale_promotion_coupon-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4371 2023-10-27 17:38:49.000000 trytond_sale_promotion_coupon-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:32.934878 trytond_sale_promotion_coupon-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/tests/scenario_sale_promotion_coupon.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_promotion_coupon-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      113 2023-10-30 17:12:55.000000 trytond_sale_promotion_coupon-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:32.938212 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2980 2023-10-30 17:39:32.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1846 2023-10-30 17:39:32.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:39:32.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:39:32.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2023-10-30 17:39:32.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:39:32.000000 trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:32.938212 trytond_sale_promotion_coupon-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/view/coupon_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/view/coupon_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/view/coupon_number_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/view/coupon_number_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.0.0/view/promotion_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.0.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:17.622197 trytond_sale_promotion_coupon-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1288 2024-04-29 15:26:18.000000 trytond_sale_promotion_coupon-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:26:17.000000 trytond_sale_promotion_coupon-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-29 15:49:17.618864 trytond_sale_promotion_coupon-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      611 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:17.615531 trytond_sale_promotion_coupon-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_sale_promotion_coupon-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:28.000000 trytond_sale_promotion_coupon-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:17.618864 trytond_sale_promotion_coupon-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2074 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2216 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2302 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2112 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2006 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1741 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1731 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2059 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2024-04-27 16:43:26.000000 trytond_sale_promotion_coupon-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7769 2024-03-25 16:05:35.000000 trytond_sale_promotion_coupon-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1690 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:17.622197 trytond_sale_promotion_coupon-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4371 2024-03-17 11:01:36.000000 trytond_sale_promotion_coupon-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:17.618864 trytond_sale_promotion_coupon-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3553 2024-04-22 12:14:36.000000 trytond_sale_promotion_coupon-7.2.0/tests/scenario_sale_promotion_coupon.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:28.000000 trytond_sale_promotion_coupon-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      113 2024-04-29 15:26:13.000000 trytond_sale_promotion_coupon-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:17.618864 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-29 15:49:17.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1828 2024-04-29 15:49:17.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:17.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:49:17.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      126 2024-04-29 15:49:17.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:17.000000 trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:17.618864 trytond_sale_promotion_coupon-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/view/coupon_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/view/coupon_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/view/coupon_number_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/view/coupon_number_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_sale_promotion_coupon-7.2.0/view/promotion_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-01-16 14:00:21.000000 trytond_sale_promotion_coupon-7.2.0/view/sale_form.xml
```

### Comparing `trytond_sale_promotion_coupon-7.0.0/CHANGELOG` & `trytond_sale_promotion_coupon-7.2.0/CHANGELOG`

 * *Files 11% similar despite different names*

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

### Comparing `trytond_sale_promotion_coupon-7.0.0/COPYRIGHT` & `trytond_sale_promotion_coupon-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_promotion_coupon-7.0.0/LICENSE` & `trytond_sale_promotion_coupon-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/PKG-INFO` & `trytond_sale_promotion_coupon-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_promotion_coupon
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for sale promotion coupon
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
@@ -45,20 +45,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_promotion<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_promotion<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Promotion Coupon Module
 ############################
 
 The sale_promotion_coupon module adds coupon to the promotions.
 
 A promotion with coupons will be applied only if a linked coupon has been added
```

### Comparing `trytond_sale_promotion_coupon-7.0.0/README.rst` & `trytond_sale_promotion_coupon-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/__init__.py` & `trytond_sale_promotion_coupon-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/doc/conf.py` & `trytond_sale_promotion_coupon-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_promotion_coupon-7.0.0/doc/index.rst` & `trytond_sale_promotion_coupon-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/bg.po` & `trytond_sale_promotion_coupon-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/ca.po` & `trytond_sale_promotion_coupon-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/cs.po` & `trytond_sale_promotion_coupon-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/de.po` & `trytond_sale_promotion_coupon-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/es.po` & `trytond_sale_promotion_coupon-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/es_419.po` & `trytond_sale_promotion_coupon-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/et.po` & `trytond_sale_promotion_coupon-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/fa.po` & `trytond_sale_promotion_coupon-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/fi.po` & `trytond_sale_promotion_coupon-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/fr.po` & `trytond_sale_promotion_coupon-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/hu.po` & `trytond_sale_promotion_coupon-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/id.po` & `trytond_sale_promotion_coupon-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/it.po` & `trytond_sale_promotion_coupon-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/lo.po` & `trytond_sale_promotion_coupon-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/lt.po` & `trytond_sale_promotion_coupon-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/nl.po` & `trytond_sale_promotion_coupon-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/pl.po` & `trytond_sale_promotion_coupon-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/pt.po` & `trytond_sale_promotion_coupon-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/ro.po` & `trytond_sale_promotion_coupon-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/ru.po` & `trytond_sale_promotion_coupon-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/sl.po` & `trytond_sale_promotion_coupon-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/tr.po` & `trytond_sale_promotion_coupon-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/uk.po` & `trytond_sale_promotion_coupon-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/locale/zh_CN.po` & `trytond_sale_promotion_coupon-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/sale.py` & `trytond_sale_promotion_coupon-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/sale.xml` & `trytond_sale_promotion_coupon-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/setup.py` & `trytond_sale_promotion_coupon-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/tests/scenario_sale_promotion_coupon.rst` & `trytond_sale_promotion_coupon-7.2.0/tests/scenario_sale_promotion_coupon.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ==============================
 Sale Promotion Coupon Scenario
 ==============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('sale_promotion_coupon')
 
 Create company::
 
@@ -51,15 +50,15 @@
     >>> template.name = 'Product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.salable = True
     >>> template.list_price = Decimal('20')
     >>> template.account_category = account_category
     >>> template.save()
-    >>> product,  = template.products
+    >>> product, = template.products
 
 Create Promotion with coupon::
 
     >>> Promotion = Model.get('sale.promotion')
     >>> promotion = Promotion(name="10%")
     >>> promotion.formula = '0.9 * unit_price'
     >>> coupon = promotion.coupons.new(name="Promo")
```

### Comparing `trytond_sale_promotion_coupon-7.0.0/tox.ini` & `trytond_sale_promotion_coupon-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/PKG-INFO` & `trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-promotion-coupon
-Version: 7.0.0
+Name: trytond_sale_promotion_coupon
+Version: 7.2.0
 Summary: Tryton module for sale promotion coupon
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
@@ -45,20 +45,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_promotion<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_promotion<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Promotion Coupon Module
 ############################
 
 The sale_promotion_coupon module adds coupon to the promotions.
 
 A promotion with coupons will be applied only if a linked coupon has been added
```

### Comparing `trytond_sale_promotion_coupon-7.0.0/trytond_sale_promotion_coupon.egg-info/SOURCES.txt` & `trytond_sale_promotion_coupon-7.2.0/trytond_sale_promotion_coupon.egg-info/SOURCES.txt`

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
 exceptions.py
```

