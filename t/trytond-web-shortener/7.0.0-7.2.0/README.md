# Comparing `tmp/trytond_web_shortener-7.0.0.tar.gz` & `tmp/trytond_web_shortener-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shortener-7.0.0.tar", last modified: Mon Oct 30 17:45:38 2023, max compression
+gzip compressed data, was "trytond_web_shortener-7.2.0.tar", last modified: Mon Apr 29 15:54:31 2024, max compression
```

## Comparing `trytond_web_shortener-7.0.0.tar` & `trytond_web_shortener-7.2.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:38.613289 trytond_web_shortener-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-22 17:23:30.000000 trytond_web_shortener-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      970 2023-10-30 17:16:41.000000 trytond_web_shortener-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:16:40.000000 trytond_web_shortener-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3452 2023-10-30 17:45:38.613289 trytond_web_shortener-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:38.609956 trytond_web_shortener-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-10-22 17:23:30.000000 trytond_web_shortener-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:30.000000 trytond_web_shortener-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:38.609956 trytond_web_shortener-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      930 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      944 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      948 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      941 2023-10-30 16:47:45.000000 trytond_web_shortener-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-10-28 12:11:27.000000 trytond_web_shortener-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:45:38.613289 trytond_web_shortener-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4358 2023-10-27 17:38:49.000000 trytond_web_shortener-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:38.609956 trytond_web_shortener-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      851 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_web_shortener-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:16:35.000000 trytond_web_shortener-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:38.609956 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3452 2023-10-30 17:45:38.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1442 2023-10-30 17:45:38.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:45:38.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:45:38.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       37 2023-10-30 17:45:38.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:45:38.000000 trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:38.609956 trytond_web_shortener-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/view/shortened_url_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/view/shortened_url_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4250 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-04-15 07:12:15.000000 trytond_web_shortener-7.0.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:31.250661 trytond_web_shortener-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1071 2024-04-29 15:30:16.000000 trytond_web_shortener-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:30:16.000000 trytond_web_shortener-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3452 2024-04-29 15:54:31.250661 trytond_web_shortener-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:31.247328 trytond_web_shortener-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_web_shortener-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:39.000000 trytond_web_shortener-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:31.247328 trytond_web_shortener-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      930 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      944 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      948 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      941 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-04-27 16:43:28.000000 trytond_web_shortener-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:31.250661 trytond_web_shortener-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4358 2024-03-17 11:01:36.000000 trytond_web_shortener-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:31.250661 trytond_web_shortener-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      851 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:39.000000 trytond_web_shortener-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:30:12.000000 trytond_web_shortener-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:31.250661 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3452 2024-04-29 15:54:30.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1424 2024-04-29 15:54:31.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:30.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:54:30.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       37 2024-04-29 15:54:30.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:30.000000 trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:31.250661 trytond_web_shortener-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/view/shortened_url_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:15.000000 trytond_web_shortener-7.2.0/view/shortened_url_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-02-26 09:40:58.000000 trytond_web_shortener-7.2.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2024-04-27 16:30:39.000000 trytond_web_shortener-7.2.0/web.xml
```

### Comparing `trytond_web_shortener-7.0.0/CHANGELOG` & `trytond_web_shortener-7.2.0/CHANGELOG`

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

### Comparing `trytond_web_shortener-7.0.0/COPYRIGHT` & `trytond_web_shortener-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2018-2023 B2CK
-Copyright (C) 2019-2023 Cédric Krier
+Copyright (C) 2018-2024 B2CK
+Copyright (C) 2019-2024 Cédric Krier
 Copyright (C) 2018-2019 Nicolas Êvrard
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_web_shortener-7.0.0/LICENSE` & `trytond_web_shortener-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/PKG-INFO` & `trytond_web_shortener-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_web_shortener
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to plug a URL to an action
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
@@ -48,15 +48,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Web Shortener Module
 ####################
 
 The web_shortener module allows URLs to be shortened. It counts the number of
 times the URL is accessed and optionally triggers action.
```

### Comparing `trytond_web_shortener-7.0.0/README.rst` & `trytond_web_shortener-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/doc/conf.py` & `trytond_web_shortener-7.2.0/doc/conf.py`

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

### Comparing `trytond_web_shortener-7.0.0/doc/index.rst` & `trytond_web_shortener-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/bg.po` & `trytond_web_shortener-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/ca.po` & `trytond_web_shortener-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/cs.po` & `trytond_web_shortener-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/de.po` & `trytond_web_shortener-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/es.po` & `trytond_web_shortener-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/es_419.po` & `trytond_web_shortener-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/et.po` & `trytond_web_shortener-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/fa.po` & `trytond_web_shortener-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/fi.po` & `trytond_web_shortener-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/fr.po` & `trytond_web_shortener-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/hu.po` & `trytond_web_shortener-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/id.po` & `trytond_web_shortener-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/it.po` & `trytond_web_shortener-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/lo.po` & `trytond_web_shortener-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/lt.po` & `trytond_web_shortener-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/nl.po` & `trytond_web_shortener-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/pl.po` & `trytond_web_shortener-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/pt.po` & `trytond_web_shortener-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/ro.po` & `trytond_web_shortener-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/ru.po` & `trytond_web_shortener-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/sl.po` & `trytond_web_shortener-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/tr.po` & `trytond_web_shortener-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/uk.po` & `trytond_web_shortener-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/locale/zh_CN.po` & `trytond_web_shortener-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/routes.py` & `trytond_web_shortener-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/setup.py` & `trytond_web_shortener-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/tests/test_module.py` & `trytond_web_shortener-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/tox.ini` & `trytond_web_shortener-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/PKG-INFO` & `trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-web-shortener
-Version: 7.0.0
+Name: trytond_web_shortener
+Version: 7.2.0
 Summary: Tryton module to plug a URL to an action
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
@@ -48,15 +48,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Web Shortener Module
 ####################
 
 The web_shortener module allows URLs to be shortened. It counts the number of
 times the URL is accessed and optionally triggers action.
```

### Comparing `trytond_web_shortener-7.0.0/trytond_web_shortener.egg-info/SOURCES.txt` & `trytond_web_shortener-7.2.0/trytond_web_shortener.egg-info/SOURCES.txt`

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
 routes.py
```

### Comparing `trytond_web_shortener-7.0.0/web.py` & `trytond_web_shortener-7.2.0/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shortener-7.0.0/web.xml` & `trytond_web_shortener-7.2.0/web.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_web_shortener-7.0.0/web.xml` & `trytond_web_shortener-7.2.0/web.xml`

```diff
@@ -23,22 +23,22 @@
     <record model="ir.action.act_window.view" id="act_shortened_url_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="shortened_url_view_form"/>
       <field name="act_window" ref="act_shortened_url"/>
     </record>
     <menuitem parent="ir.menu_models" action="act_shortened_url" sequence="50" id="menu_shortened_url_form"/>
     <record model="ir.model.access" id="access_shortened_url">
-      <field name="model" search="[('model', '=', 'web.shortened_url')]"/>
+      <field name="model">web.shortened_url</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shortened_url_group_admin">
-      <field name="model" search="[('model', '=', 'web.shortened_url')]"/>
+      <field name="model">web.shortened_url</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

