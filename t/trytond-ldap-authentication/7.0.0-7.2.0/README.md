# Comparing `tmp/trytond_ldap_authentication-7.0.0.tar.gz` & `tmp/trytond_ldap_authentication-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_ldap_authentication-7.0.0.tar", last modified: Mon Oct 30 17:30:48 2023, max compression
+gzip compressed data, was "trytond_ldap_authentication-7.2.0.tar", last modified: Mon Apr 29 15:41:15 2024, max compression
```

## Comparing `trytond_ldap_authentication-7.0.0.tar` & `trytond_ldap_authentication-7.2.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-22 17:23:05.000000 trytond_ldap_authentication-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2683 2023-10-30 17:06:59.000000 trytond_ldap_authentication-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      805 2023-10-30 17:06:59.000000 trytond_ldap_authentication-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_ldap_authentication-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-22 17:23:05.000000 trytond_ldap_authentication-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:05.000000 trytond_ldap_authentication-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      249 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-10-30 16:47:45.000000 trytond_ldap_authentication-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      249 2023-10-28 12:11:23.000000 trytond_ldap_authentication-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6276 2023-10-24 07:56:52.000000 trytond_ldap_authentication-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4490 2023-10-27 17:38:49.000000 trytond_ldap_authentication-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8164 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_ldap_authentication-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:06:56.000000 trytond_ldap_authentication-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:48.649044 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-10-30 17:30:48.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-10-30 17:30:48.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:48.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:30:48.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       39 2023-10-30 17:30:48.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:30:48.000000 trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:15.531473 trytond_ldap_authentication-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2784 2024-04-29 15:20:22.000000 trytond_ldap_authentication-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      805 2024-04-29 15:20:22.000000 trytond_ldap_authentication-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_ldap_authentication-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-04-29 15:41:15.531473 trytond_ldap_authentication-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:15.528139 trytond_ldap_authentication-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_ldap_authentication-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:11.000000 trytond_ldap_authentication-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:15.528139 trytond_ldap_authentication-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      274 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      249 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      249 2024-04-27 16:43:24.000000 trytond_ldap_authentication-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6276 2024-02-04 18:51:26.000000 trytond_ldap_authentication-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:15.531473 trytond_ldap_authentication-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4490 2024-03-17 11:01:36.000000 trytond_ldap_authentication-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:15.528139 trytond_ldap_authentication-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8164 2023-04-15 07:12:15.000000 trytond_ldap_authentication-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:11.000000 trytond_ldap_authentication-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:20:17.000000 trytond_ldap_authentication-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:15.531473 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-04-29 15:41:15.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1336 2024-04-29 15:41:15.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:15.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:41:15.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       39 2024-04-29 15:41:15.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:15.000000 trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/top_level.txt
```

### Comparing `trytond_ldap_authentication-7.0.0/CHANGELOG` & `trytond_ldap_authentication-7.2.0/CHANGELOG`

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

### Comparing `trytond_ldap_authentication-7.0.0/COPYRIGHT` & `trytond_ldap_authentication-7.2.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2006-2023 Cédric Krier.
+Copyright (C) 2006-2024 Cédric Krier.
 Copyright (C) 2009-2012 Bertrand Chenal.
-Copyright (C) 2009-2023 B2CK SPRL.
+Copyright (C) 2009-2024 B2CK SPRL.
 Copyright (C) 2008-2012 Udo Spallek.
 Copyright (C) 2008-2011 virtual things.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_ldap_authentication-7.0.0/LICENSE` & `trytond_ldap_authentication-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/PKG-INFO` & `trytond_ldap_authentication-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_ldap_authentication
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to authenticate users through LDAP
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
@@ -49,15 +49,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: ldap3>=2.0.7
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 LDAP Authentication Module
 ##########################
 
 The LDAP authentication module allows to authenticate users via a LDAP server.
```

### Comparing `trytond_ldap_authentication-7.0.0/README.rst` & `trytond_ldap_authentication-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/doc/conf.py` & `trytond_ldap_authentication-7.2.0/doc/conf.py`

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

### Comparing `trytond_ldap_authentication-7.0.0/doc/index.rst` & `trytond_ldap_authentication-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/res.py` & `trytond_ldap_authentication-7.2.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/setup.py` & `trytond_ldap_authentication-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/tests/test_module.py` & `trytond_ldap_authentication-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/tox.ini` & `trytond_ldap_authentication-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/PKG-INFO` & `trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-ldap-authentication
-Version: 7.0.0
+Name: trytond_ldap_authentication
+Version: 7.2.0
 Summary: Tryton module to authenticate users through LDAP
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
@@ -49,15 +49,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: ldap3>=2.0.7
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 LDAP Authentication Module
 ##########################
 
 The LDAP authentication module allows to authenticate users via a LDAP server.
```

### Comparing `trytond_ldap_authentication-7.0.0/trytond_ldap_authentication.egg-info/SOURCES.txt` & `trytond_ldap_authentication-7.2.0/trytond_ldap_authentication.egg-info/SOURCES.txt`

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
 message.xml
```
