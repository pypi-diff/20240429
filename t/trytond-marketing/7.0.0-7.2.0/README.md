# Comparing `tmp/trytond_marketing-7.0.0.tar.gz` & `tmp/trytond_marketing-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing-7.0.0.tar", last modified: Mon Oct 30 17:30:55 2023, max compression
+gzip compressed data, was "trytond_marketing-7.2.0.tar", last modified: Mon Apr 29 15:41:22 2024, max compression
```

## Comparing `trytond_marketing-7.0.0.tar` & `trytond_marketing-7.2.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-22 17:23:06.000000 trytond_marketing-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      970 2023-10-30 17:07:04.000000 trytond_marketing-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:07:04.000000 trytond_marketing-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2398 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2810 2023-10-22 17:23:06.000000 trytond_marketing-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:06.000000 trytond_marketing-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/icons/tryton-marketing.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      234 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2023-10-30 16:47:45.000000 trytond_marketing-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-28 12:11:23.000000 trytond_marketing-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1092 2023-10-16 16:37:26.000000 trytond_marketing-7.0.0/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4325 2023-10-27 17:38:49.000000 trytond_marketing-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_marketing-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_marketing-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:07:00.000000 trytond_marketing-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:55.755745 trytond_marketing-7.0.0/trytond_marketing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2398 2023-10-30 17:30:55.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1342 2023-10-30 17:30:55.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:55.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:30:55.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       26 2023-10-30 17:30:55.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:30:55.000000 trytond_marketing-7.0.0/trytond_marketing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:22.411293 trytond_marketing-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1071 2024-04-29 15:20:27.000000 trytond_marketing-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:20:27.000000 trytond_marketing-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2398 2024-04-29 15:41:22.411293 trytond_marketing-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:22.407959 trytond_marketing-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-27 16:30:39.000000 trytond_marketing-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:11.000000 trytond_marketing-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:22.407959 trytond_marketing-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/icons/tryton-marketing.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:22.411293 trytond_marketing-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      234 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-27 16:43:24.000000 trytond_marketing-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1092 2023-10-16 16:37:26.000000 trytond_marketing-7.2.0/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:22.411293 trytond_marketing-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4325 2024-03-17 11:01:36.000000 trytond_marketing-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:22.411293 trytond_marketing-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_marketing-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:11.000000 trytond_marketing-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:20:22.000000 trytond_marketing-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:22.411293 trytond_marketing-7.2.0/trytond_marketing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2398 2024-04-29 15:41:21.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1324 2024-04-29 15:41:22.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:21.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:41:21.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       26 2024-04-29 15:41:21.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:21.000000 trytond_marketing-7.2.0/trytond_marketing.egg-info/top_level.txt
```

### Comparing `trytond_marketing-7.0.0/CHANGELOG` & `trytond_marketing-7.2.0/CHANGELOG`

 * *Files 15% similar despite different names*

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

### Comparing `trytond_marketing-7.0.0/LICENSE` & `trytond_marketing-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing-7.0.0/PKG-INFO` & `trytond_marketing-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_marketing
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to group marketing features
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
@@ -47,14 +47,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Marketing Module
 ################
 
 The marketing module defines the fundamentals for marketing modules.
```

### Comparing `trytond_marketing-7.0.0/doc/conf.py` & `trytond_marketing-7.2.0/doc/conf.py`

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

### Comparing `trytond_marketing-7.0.0/icons/LICENSE` & `trytond_marketing-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing-7.0.0/marketing.xml` & `trytond_marketing-7.2.0/marketing.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing-7.0.0/setup.py` & `trytond_marketing-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing-7.0.0/tox.ini` & `trytond_marketing-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing-7.0.0/trytond_marketing.egg-info/PKG-INFO` & `trytond_marketing-7.2.0/trytond_marketing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-marketing
-Version: 7.0.0
+Name: trytond_marketing
+Version: 7.2.0
 Summary: Tryton module to group marketing features
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
@@ -47,14 +47,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Marketing Module
 ################
 
 The marketing module defines the fundamentals for marketing modules.
```

### Comparing `trytond_marketing-7.0.0/trytond_marketing.egg-info/SOURCES.txt` & `trytond_marketing-7.2.0/trytond_marketing.egg-info/SOURCES.txt`

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
 marketing.xml
```

