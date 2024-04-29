# Comparing `tmp/trytond_product_measurements-7.0.0.tar.gz` & `tmp/trytond_product_measurements-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_measurements-7.0.0.tar", last modified: Mon Oct 30 17:33:06 2023, max compression
+gzip compressed data, was "trytond_product_measurements-7.2.0.tar", last modified: Mon Apr 29 15:43:27 2024, max compression
```

## Comparing `trytond_product_measurements-7.0.0.tar` & `trytond_product_measurements-7.2.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:06.939704 trytond_product_measurements-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:23:10.000000 trytond_product_measurements-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-10-30 17:09:10.000000 trytond_product_measurements-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:09:10.000000 trytond_product_measurements-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_measurements-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_measurements-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2023-10-30 17:33:06.939704 trytond_product_measurements-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-01-16 14:00:20.000000 trytond_product_measurements-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_product_measurements-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:06.936371 trytond_product_measurements-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:23:10.000000 trytond_product_measurements-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-01-16 14:00:20.000000 trytond_product_measurements-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:10.000000 trytond_product_measurements-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:06.936371 trytond_product_measurements-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4101 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4543 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4470 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4549 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4125 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4577 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3989 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3714 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3831 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4326 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4521 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3839 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3959 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3861 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3969 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3603 2023-10-30 16:47:45.000000 trytond_product_measurements-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4542 2023-10-24 07:56:52.000000 trytond_product_measurements-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_product_measurements-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:33:06.939704 trytond_product_measurements-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4334 2023-10-27 17:38:49.000000 trytond_product_measurements-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:06.936371 trytond_product_measurements-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_measurements-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_product_measurements-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_measurements-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:09:06.000000 trytond_product_measurements-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:06.939704 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2023-10-30 17:33:06.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1417 2023-10-30 17:33:06.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:33:06.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:33:06.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-10-30 17:33:06.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:33:06.000000 trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:33:06.936371 trytond_product_measurements-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1080 2023-10-24 07:56:52.000000 trytond_product_measurements-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2183 2024-04-29 15:22:04.000000 trytond_product_measurements-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:22:04.000000 trytond_product_measurements-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.584685 trytond_product_measurements-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_product_measurements-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:16.000000 trytond_product_measurements-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4101 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4543 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4470 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4549 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4125 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4577 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3989 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3714 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3831 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4326 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4521 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3858 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4653 2024-04-29 13:17:17.000000 trytond_product_measurements-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3959 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3861 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3969 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3603 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4542 2024-02-04 18:51:26.000000 trytond_product_measurements-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4334 2024-03-17 11:01:36.000000 trytond_product_measurements-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:16.000000 trytond_product_measurements-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:22:00.000000 trytond_product_measurements-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1080 2024-02-04 18:51:26.000000 trytond_product_measurements-7.2.0/view/template_form.xml
```

### Comparing `trytond_product_measurements-7.0.0/CHANGELOG` & `trytond_product_measurements-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_product_measurements-7.0.0/COPYRIGHT` & `trytond_product_measurements-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2023 Cédric Krier.
+Copyright (C) 2011-2024 Cédric Krier.
 Copyright (C) 2011-2012 Bertrand Chenal.
 Copyright (C) 2011-2023 Nicolas Évrard.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_measurements-7.0.0/LICENSE` & `trytond_product_measurements-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/PKG-INFO` & `trytond_product_measurements-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_measurements
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add measurements to product
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
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Measurements
 ####################
 
 The Product Measurements module adds this following measurements to Product:
 
 - Length
```

### Comparing `trytond_product_measurements-7.0.0/doc/conf.py` & `trytond_product_measurements-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_measurements-7.0.0/locale/bg.po` & `trytond_product_measurements-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/ca.po` & `trytond_product_measurements-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/cs.po` & `trytond_product_measurements-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/de.po` & `trytond_product_measurements-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/es.po` & `trytond_product_measurements-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/es_419.po` & `trytond_product_measurements-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/et.po` & `trytond_product_measurements-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/fa.po` & `trytond_product_measurements-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/fi.po` & `trytond_product_measurements-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/fr.po` & `trytond_product_measurements-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/hu.po` & `trytond_product_measurements-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/id.po` & `trytond_product_measurements-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/it.po` & `trytond_product_measurements-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/lo.po` & `trytond_product_measurements-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/lt.po` & `trytond_product_measurements-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/nl.po` & `trytond_product_measurements-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/pl.po` & `trytond_product_measurements-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/pt.po` & `trytond_product_measurements-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/ro.po` & `trytond_product_measurements-7.2.0/locale/tr.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,height:"
 msgid "Height"
-msgstr "Înălţime"
+msgstr "Yükseklik"
 
 #, fuzzy
 msgctxt "field:product.product,height_uom:"
 msgid "Height UoM"
-msgstr "Înălțime UM"
+msgstr "Yükseklik Ölçü Birimi"
 
 msgctxt "field:product.product,length:"
 msgid "Length"
-msgstr "Lungime"
+msgstr "Uzunluk"
 
 #, fuzzy
 msgctxt "field:product.product,length_uom:"
 msgid "Length UoM"
-msgstr "Lungime UM"
+msgstr "Uzunluk Ölçü Birimi"
 
 msgctxt "field:product.product,volume:"
 msgid "Volume"
-msgstr "Volum"
+msgstr "Hacim"
 
 #, fuzzy
 msgctxt "field:product.product,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volum UM"
+msgstr "Hacim Ölçü Birimi"
 
 msgctxt "field:product.product,weight:"
 msgid "Weight"
-msgstr "Greutate"
+msgstr "Ağırlık"
 
 #, fuzzy
 msgctxt "field:product.product,weight_uom:"
 msgid "Weight UoM"
-msgstr "UM Greutate"
+msgstr "Ağırlık Ölçü Birimi"
 
 msgctxt "field:product.product,width:"
 msgid "Width"
-msgstr "Lăţime"
+msgstr "Genişlik"
 
 #, fuzzy
 msgctxt "field:product.product,width_uom:"
 msgid "Width UoM"
-msgstr "UM Latime"
+msgstr "Genişlik Ölçü Birimi"
 
 msgctxt "field:product.template,height:"
 msgid "Height"
-msgstr "Înălţime"
+msgstr "Yükseklik"
 
 #, fuzzy
 msgctxt "field:product.template,height_uom:"
 msgid "Height UoM"
-msgstr "UM Înălțime"
+msgstr "Yükseklik Ölçü Birimi"
 
 msgctxt "field:product.template,length:"
 msgid "Length"
-msgstr "Lungime"
+msgstr "Uzunluk"
 
 #, fuzzy
 msgctxt "field:product.template,length_uom:"
 msgid "Length UoM"
-msgstr "UM Lungime"
+msgstr "Uzunluk Ölçü Birimi"
 
 msgctxt "field:product.template,volume:"
 msgid "Volume"
-msgstr "Volum"
+msgstr "Hacim"
 
 #, fuzzy
 msgctxt "field:product.template,volume_uom:"
 msgid "Volume UoM"
-msgstr "UM Volum"
+msgstr "Hacim Ölçü Birimi"
 
 msgctxt "field:product.template,weight:"
 msgid "Weight"
-msgstr "Greutate"
+msgstr "Ağırlık"
 
 #, fuzzy
 msgctxt "field:product.template,weight_uom:"
 msgid "Weight UoM"
-msgstr "UM Greutate"
+msgstr "Ağırlık Ölçü Birimi"
 
 msgctxt "field:product.template,width:"
 msgid "Width"
-msgstr "Lăţime"
+msgstr "Genişlik"
 
 #, fuzzy
 msgctxt "field:product.template,width_uom:"
 msgid "Width UoM"
-msgstr "UM Latime"
+msgstr "Genişlik Ölçü Birimi"
 
 msgctxt "help:product.product,height:"
 msgid "Height for 1 default unit of measure."
 msgstr ""
 
 msgctxt "help:product.product,height_uom:"
 msgid "The Unit of Measure for the height."
@@ -170,12 +170,12 @@
 
 msgctxt "help:product.template,width_uom:"
 msgid "The Unit of Measure for the width."
 msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Measurements"
-msgstr "Măsurători"
+msgstr "Ölçüler"
 
 msgctxt "view:product.template:"
 msgid "Measurements for 1 default UoM."
 msgstr ""
```

### Comparing `trytond_product_measurements-7.0.0/locale/ru.po` & `trytond_product_measurements-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/sl.po` & `trytond_product_measurements-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/locale/tr.po` & `trytond_product_measurements-7.2.0/locale/zh_CN.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,94 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,height:"
 msgid "Height"
-msgstr "Yükseklik"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,height_uom:"
 msgid "Height UoM"
-msgstr "Yükseklik Ölçü Birimi"
+msgstr ""
 
 msgctxt "field:product.product,length:"
 msgid "Length"
-msgstr "Uzunluk"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,length_uom:"
 msgid "Length UoM"
-msgstr "Uzunluk Ölçü Birimi"
+msgstr ""
 
 msgctxt "field:product.product,volume:"
 msgid "Volume"
-msgstr "Hacim"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,volume_uom:"
 msgid "Volume UoM"
-msgstr "Hacim Ölçü Birimi"
+msgstr ""
 
 msgctxt "field:product.product,weight:"
 msgid "Weight"
-msgstr "Ağırlık"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,weight_uom:"
 msgid "Weight UoM"
-msgstr "Ağırlık Ölçü Birimi"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,width:"
 msgid "Width"
-msgstr "Genişlik"
+msgstr "宽"
 
 #, fuzzy
 msgctxt "field:product.product,width_uom:"
 msgid "Width UoM"
-msgstr "Genişlik Ölçü Birimi"
+msgstr "宽"
 
 msgctxt "field:product.template,height:"
 msgid "Height"
-msgstr "Yükseklik"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,height_uom:"
 msgid "Height UoM"
-msgstr "Yükseklik Ölçü Birimi"
+msgstr ""
 
 msgctxt "field:product.template,length:"
 msgid "Length"
-msgstr "Uzunluk"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,length_uom:"
 msgid "Length UoM"
-msgstr "Uzunluk Ölçü Birimi"
+msgstr ""
 
 msgctxt "field:product.template,volume:"
 msgid "Volume"
-msgstr "Hacim"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,volume_uom:"
 msgid "Volume UoM"
-msgstr "Hacim Ölçü Birimi"
+msgstr ""
 
 msgctxt "field:product.template,weight:"
 msgid "Weight"
-msgstr "Ağırlık"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,weight_uom:"
 msgid "Weight UoM"
-msgstr "Ağırlık Ölçü Birimi"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,width:"
 msgid "Width"
-msgstr "Genişlik"
+msgstr "宽"
 
 #, fuzzy
 msgctxt "field:product.template,width_uom:"
 msgid "Width UoM"
-msgstr "Genişlik Ölçü Birimi"
+msgstr "宽"
 
 msgctxt "help:product.product,height:"
 msgid "Height for 1 default unit of measure."
 msgstr ""
 
 msgctxt "help:product.product,height_uom:"
 msgid "The Unit of Measure for the height."
@@ -170,12 +164,12 @@
 
 msgctxt "help:product.template,width_uom:"
 msgid "The Unit of Measure for the width."
 msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Measurements"
-msgstr "Ölçüler"
+msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Measurements for 1 default UoM."
 msgstr ""
```

### Comparing `trytond_product_measurements-7.0.0/locale/uk.po` & `trytond_product_measurements-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/product.py` & `trytond_product_measurements-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/setup.py` & `trytond_product_measurements-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/tox.ini` & `trytond_product_measurements-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/PKG-INFO` & `trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-measurements
-Version: 7.0.0
+Name: trytond_product_measurements
+Version: 7.2.0
 Summary: Tryton module to add measurements to product
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
@@ -48,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Product Measurements
 ####################
 
 The Product Measurements module adds this following measurements to Product:
 
 - Length
```

### Comparing `trytond_product_measurements-7.0.0/trytond_product_measurements.egg-info/SOURCES.txt` & `trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/SOURCES.txt`

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

### Comparing `trytond_product_measurements-7.0.0/view/template_form.xml` & `trytond_product_measurements-7.2.0/view/template_form.xml`

 * *Files identical despite different names*

