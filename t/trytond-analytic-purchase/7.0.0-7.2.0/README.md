# Comparing `tmp/trytond_analytic_purchase-7.0.0.tar.gz` & `tmp/trytond_analytic_purchase-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_purchase-7.0.0.tar", last modified: Mon Oct 30 17:26:51 2023, max compression
+gzip compressed data, was "trytond_analytic_purchase-7.2.0.tar", last modified: Mon Apr 29 15:37:58 2024, max compression
```

## Comparing `trytond_analytic_purchase-7.0.0.tar` & `trytond_analytic_purchase-7.2.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:51.501247 trytond_analytic_purchase-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-22 17:22:59.000000 trytond_analytic_purchase-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2642 2023-10-30 17:04:42.000000 trytond_analytic_purchase-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:04:42.000000 trytond_analytic_purchase-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_purchase-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2715 2023-10-30 17:26:51.497913 trytond_analytic_purchase-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:51.497913 trytond_analytic_purchase-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-22 17:22:59.000000 trytond_analytic_purchase-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:59.000000 trytond_analytic_purchase-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:51.494580 trytond_analytic_purchase-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-28 12:11:21.000000 trytond_analytic_purchase-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2175 2023-10-07 15:40:36.000000 trytond_analytic_purchase-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-01-16 14:00:20.000000 trytond_analytic_purchase-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:26:51.501247 trytond_analytic_purchase-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4460 2023-10-27 17:38:49.000000 trytond_analytic_purchase-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:51.497913 trytond_analytic_purchase-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4641 2023-10-24 07:56:52.000000 trytond_analytic_purchase-7.0.0/tests/scenario_analytic_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_analytic_purchase-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-10-30 17:04:38.000000 trytond_analytic_purchase-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:51.497913 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2715 2023-10-30 17:26:50.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1534 2023-10-30 17:26:51.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:26:50.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-10-30 17:26:50.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-10-30 17:26:50.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:26:50.000000 trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:26:51.497913 trytond_analytic_purchase-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_analytic_purchase-7.0.0/view/purchase_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:58.179967 trytond_analytic_purchase-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2024-04-29 15:17:49.000000 trytond_analytic_purchase-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:17:49.000000 trytond_analytic_purchase-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_purchase-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2715 2024-04-29 15:37:58.179967 trytond_analytic_purchase-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:58.176634 trytond_analytic_purchase-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_analytic_purchase-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:04.000000 trytond_analytic_purchase-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:58.176634 trytond_analytic_purchase-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-29 13:17:17.000000 trytond_analytic_purchase-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-27 16:43:22.000000 trytond_analytic_purchase-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2175 2024-02-04 18:51:26.000000 trytond_analytic_purchase-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-01-16 14:00:20.000000 trytond_analytic_purchase-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:58.179967 trytond_analytic_purchase-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4460 2024-03-17 11:01:36.000000 trytond_analytic_purchase-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:58.176634 trytond_analytic_purchase-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4591 2024-04-22 12:14:36.000000 trytond_analytic_purchase-7.2.0/tests/scenario_analytic_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_purchase-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:04.000000 trytond_analytic_purchase-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-29 15:17:45.000000 trytond_analytic_purchase-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:58.179967 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2715 2024-04-29 15:37:57.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1516 2024-04-29 15:37:58.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:57.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:37:57.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-04-29 15:37:57.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:57.000000 trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:58.179967 trytond_analytic_purchase-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_analytic_purchase-7.2.0/view/purchase_line_form.xml
```

### Comparing `trytond_analytic_purchase-7.0.0/CHANGELOG` & `trytond_analytic_purchase-7.2.0/CHANGELOG`

 * *Files 13% similar despite different names*

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

### Comparing `trytond_analytic_purchase-7.0.0/LICENSE` & `trytond_analytic_purchase-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_purchase-7.0.0/PKG-INFO` & `trytond_analytic_purchase-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_purchase
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add analytic accounting on purchase
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_analytic_account<7.1,>=7.0
-Requires-Dist: trytond_analytic_invoice<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_analytic_account<7.3,>=7.2
+Requires-Dist: trytond_analytic_invoice<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Analytic Purchase Module
 ########################
 
 The analytic purchase module allows to set analytic accounts on purchase line.
```

### Comparing `trytond_analytic_purchase-7.0.0/doc/conf.py` & `trytond_analytic_purchase-7.2.0/doc/conf.py`

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

### Comparing `trytond_analytic_purchase-7.0.0/purchase.py` & `trytond_analytic_purchase-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_purchase-7.0.0/setup.py` & `trytond_analytic_purchase-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_purchase-7.0.0/tests/scenario_analytic_purchase.rst` & `trytond_analytic_purchase-7.2.0/tests/scenario_analytic_purchase.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ==========================
 Analytic Purchase Scenario
 ==========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
 Activate modules::
 
     >>> config = activate_modules('analytic_purchase')
 
 Create company::
 
@@ -98,16 +97,15 @@
     >>> Purchase = Model.get('purchase.purchase')
     >>> purchase = Purchase()
     >>> purchase.party = supplier
     >>> purchase.payment_term = payment_term
     >>> purchase.invoice_method = 'order'
     >>> purchase_line = purchase.lines.new()
     >>> entry, = purchase_line.analytic_accounts
-    >>> entry.root == root
-    True
+    >>> assertEqual(entry.root, root)
     >>> entry.account = analytic_account
     >>> purchase_line.product = product
     >>> purchase_line.quantity = 5
     >>> purchase_line.unit_price = Decimal('5.0000')
     >>> purchase.click('quote')
     >>> purchase.click('confirm')
     >>> purchase.state
@@ -115,16 +113,15 @@
 
 Check invoice analytic accounts::
 
     >>> Invoice = Model.get('account.invoice')
     >>> invoice = Invoice(purchase.invoices[0].id)
     >>> invoice_line, = invoice.lines
     >>> entry, = invoice_line.analytic_accounts
-    >>> entry.account == analytic_account
-    True
+    >>> assertEqual(entry.account, analytic_account)
 
 Purchase with an empty analytic account::
 
     >>> set_user(purchase_user)
     >>> Purchase = Model.get('purchase.purchase')
     >>> purchase = Purchase()
     >>> purchase.party = supplier
```

### Comparing `trytond_analytic_purchase-7.0.0/tox.ini` & `trytond_analytic_purchase-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/PKG-INFO` & `trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-analytic-purchase
-Version: 7.0.0
+Name: trytond_analytic_purchase
+Version: 7.2.0
 Summary: Tryton module to add analytic accounting on purchase
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_analytic_account<7.1,>=7.0
-Requires-Dist: trytond_analytic_invoice<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_analytic_account<7.3,>=7.2
+Requires-Dist: trytond_analytic_invoice<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Analytic Purchase Module
 ########################
 
 The analytic purchase module allows to set analytic accounts on purchase line.
```

### Comparing `trytond_analytic_purchase-7.0.0/trytond_analytic_purchase.egg-info/SOURCES.txt` & `trytond_analytic_purchase-7.2.0/trytond_analytic_purchase.egg-info/SOURCES.txt`

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
 purchase.py
```

