# Comparing `tmp/trytond_google_maps-7.0.0.tar.gz` & `tmp/trytond_google_maps-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_google_maps-7.0.0.tar", last modified: Mon Oct 30 17:30:24 2023, max compression
+gzip compressed data, was "trytond_google_maps-7.2.0.tar", last modified: Mon Apr 29 15:40:54 2024, max compression
```

## Comparing `trytond_google_maps-7.0.0.tar` & `trytond_google_maps-7.2.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:24.842264 trytond_google_maps-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-10-22 17:23:05.000000 trytond_google_maps-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2604 2023-10-30 17:06:46.000000 trytond_google_maps-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:06:46.000000 trytond_google_maps-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_google_maps-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2580 2023-10-30 17:30:24.842264 trytond_google_maps-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      212 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/address.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:24.842264 trytond_google_maps-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2812 2023-10-22 17:23:05.000000 trytond_google_maps-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      212 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:05.000000 trytond_google_maps-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:24.838931 trytond_google_maps-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:23.000000 trytond_google_maps-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:30:24.842264 trytond_google_maps-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4253 2023-10-27 17:38:49.000000 trytond_google_maps-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:24.838931 trytond_google_maps-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1405 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_google_maps-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:06:42.000000 trytond_google_maps-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:24.842264 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2580 2023-10-30 17:30:24.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1352 2023-10-30 17:30:24.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:24.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-10-30 17:30:24.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-10-30 17:30:24.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:30:24.000000 trytond_google_maps-7.0.0/trytond_google_maps.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:24.842264 trytond_google_maps-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_google_maps-7.0.0/view/address_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:54.862013 trytond_google_maps-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2705 2024-04-29 15:20:07.000000 trytond_google_maps-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:20:06.000000 trytond_google_maps-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_google_maps-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2580 2024-04-29 15:40:54.862013 trytond_google_maps-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      212 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/address.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:54.858680 trytond_google_maps-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_google_maps-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      212 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:10.000000 trytond_google_maps-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:54.858680 trytond_google_maps-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:24.000000 trytond_google_maps-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:54.862013 trytond_google_maps-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4253 2024-03-17 11:01:36.000000 trytond_google_maps-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:54.858680 trytond_google_maps-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1405 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:10.000000 trytond_google_maps-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:20:02.000000 trytond_google_maps-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:54.862013 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2580 2024-04-29 15:40:54.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1334 2024-04-29 15:40:54.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:54.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:40:54.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       42 2024-04-29 15:40:54.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:54.000000 trytond_google_maps-7.2.0/trytond_google_maps.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:54.862013 trytond_google_maps-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_google_maps-7.2.0/view/address_form.xml
```

### Comparing `trytond_google_maps-7.0.0/CHANGELOG` & `trytond_google_maps-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

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

### Comparing `trytond_google_maps-7.0.0/COPYRIGHT` & `trytond_google_maps-7.2.0/COPYRIGHT`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2012 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_google_maps-7.0.0/LICENSE` & `trytond_google_maps-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-7.0.0/PKG-INFO` & `trytond_google_maps-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_google_maps
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to link addresses to Google Maps
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
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Google Maps Module
 ##################
 
 The Google Maps module add a new URL field on the party
 addresses. This link open the Google Maps page on the default browser
 with the map centered on the selected address.
```

### Comparing `trytond_google_maps-7.0.0/address.py` & `trytond_google_maps-7.2.0/address.py`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-7.0.0/address.xml` & `trytond_google_maps-7.2.0/address.xml`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-7.0.0/doc/conf.py` & `trytond_google_maps-7.2.0/doc/conf.py`

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

### Comparing `trytond_google_maps-7.0.0/setup.py` & `trytond_google_maps-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-7.0.0/tests/test_module.py` & `trytond_google_maps-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-7.0.0/tox.ini` & `trytond_google_maps-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-7.0.0/trytond_google_maps.egg-info/PKG-INFO` & `trytond_google_maps-7.2.0/trytond_google_maps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-google-maps
-Version: 7.0.0
+Name: trytond_google_maps
+Version: 7.2.0
 Summary: Tryton module to link addresses to Google Maps
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
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Google Maps Module
 ##################
 
 The Google Maps module add a new URL field on the party
 addresses. This link open the Google Maps page on the default browser
 with the map centered on the selected address.
```

### Comparing `trytond_google_maps-7.0.0/trytond_google_maps.egg-info/SOURCES.txt` & `trytond_google_maps-7.2.0/trytond_google_maps.egg-info/SOURCES.txt`

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
 address.py
```

