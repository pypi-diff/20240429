# Comparing `tmp/trytond_authentication_sms-7.0.0.tar.gz` & `tmp/trytond_authentication_sms-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_authentication_sms-7.0.0.tar", last modified: Mon Oct 30 17:27:24 2023, max compression
+gzip compressed data, was "trytond_authentication_sms-7.2.0.tar", last modified: Mon Apr 29 15:38:23 2024, max compression
```

## Comparing `trytond_authentication_sms-7.0.0.tar` & `trytond_authentication_sms-7.2.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:24.654738 trytond_authentication_sms-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:00.000000 trytond_authentication_sms-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1411 2023-10-30 17:05:01.000000 trytond_authentication_sms-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:05:01.000000 trytond_authentication_sms-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_authentication_sms-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3388 2023-10-30 17:27:24.654738 trytond_authentication_sms-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1112 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:24.651405 trytond_authentication_sms-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:00.000000 trytond_authentication_sms-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1112 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:00.000000 trytond_authentication_sms-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:24.651405 trytond_authentication_sms-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      828 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      818 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      810 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      821 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      991 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      818 2023-10-30 16:47:45.000000 trytond_authentication_sms-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      719 2023-10-28 12:11:21.000000 trytond_authentication_sms-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3787 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-01-16 14:00:20.000000 trytond_authentication_sms-7.0.0/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:27:24.654738 trytond_authentication_sms-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4374 2023-10-27 17:38:49.000000 trytond_authentication_sms-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:24.651405 trytond_authentication_sms-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3660 2023-06-10 11:39:56.000000 trytond_authentication_sms-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_authentication_sms-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:04:57.000000 trytond_authentication_sms-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:24.654738 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3388 2023-10-30 17:27:24.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-10-30 17:27:24.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:27:24.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:27:24.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       26 2023-10-30 17:27:24.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:27:24.000000 trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:27:24.651405 trytond_authentication_sms-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      193 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.0.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1512 2024-04-29 15:18:10.000000 trytond_authentication_sms-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:18:09.000000 trytond_authentication_sms-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_authentication_sms-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3388 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1112 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.305977 trytond_authentication_sms-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_authentication_sms-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1112 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:05.000000 trytond_authentication_sms-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.305977 trytond_authentication_sms-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      818 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      810 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      821 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      991 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      824 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2024-04-29 13:17:17.000000 trytond_authentication_sms-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      818 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      719 2024-04-27 16:43:22.000000 trytond_authentication_sms-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3787 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-01-16 14:00:20.000000 trytond_authentication_sms-7.2.0/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4374 2024-03-17 11:01:36.000000 trytond_authentication_sms-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.305977 trytond_authentication_sms-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3660 2024-01-27 09:58:52.000000 trytond_authentication_sms-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:05.000000 trytond_authentication_sms-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:18:05.000000 trytond_authentication_sms-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3388 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1451 2024-04-29 15:38:23.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       26 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:22.000000 trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:23.309310 trytond_authentication_sms-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      193 2023-04-15 07:12:15.000000 trytond_authentication_sms-7.2.0/view/user_form_preferences.xml
```

### Comparing `trytond_authentication_sms-7.0.0/CHANGELOG` & `trytond_authentication_sms-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_authentication_sms-7.0.0/COPYRIGHT` & `trytond_authentication_sms-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2016-2023 B2CK
-Copyright (C) 2016-2023 Cédric Krier
+Copyright (C) 2016-2024 B2CK
+Copyright (C) 2016-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_authentication_sms-7.0.0/LICENSE` & `trytond_authentication_sms-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/PKG-INFO` & `trytond_authentication_sms-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_authentication_sms
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to authenticate users via SMS
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
@@ -46,15 +46,15 @@
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
 
 Authentication SMS Module
 #########################
 
 The `SMS <https://en.wikipedia.org/wiki/Short_Message_Service>`_ authentication
 module allows users to authenticate via SMS.  It adds a new authentication
```

### Comparing `trytond_authentication_sms-7.0.0/README.rst` & `trytond_authentication_sms-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/doc/conf.py` & `trytond_authentication_sms-7.2.0/doc/conf.py`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_authentication_sms-7.0.0/doc/index.rst` & `trytond_authentication_sms-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/bg.po` & `trytond_authentication_sms-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/ca.po` & `trytond_authentication_sms-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/cs.po` & `trytond_authentication_sms-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/de.po` & `trytond_authentication_sms-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/es.po` & `trytond_authentication_sms-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/es_419.po` & `trytond_authentication_sms-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/et.po` & `trytond_authentication_sms-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/fa.po` & `trytond_authentication_sms-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/fi.po` & `trytond_authentication_sms-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/fr.po` & `trytond_authentication_sms-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/hu.po` & `trytond_authentication_sms-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/id.po` & `trytond_authentication_sms-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/it.po` & `trytond_authentication_sms-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/lo.po` & `trytond_authentication_sms-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/lt.po` & `trytond_authentication_sms-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/nl.po` & `trytond_authentication_sms-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/pl.po` & `trytond_authentication_sms-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/pt.po` & `trytond_authentication_sms-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/ro.po` & `trytond_authentication_sms-7.2.0/locale/tr.po`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:res.user,mobile:"
 msgid "Mobile"
 msgstr ""
 
 msgctxt "field:res.user.login.sms_code,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:res.user.login.sms_code,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "field:res.user.login.sms_code,user_id:"
 msgid "User ID"
```

### Comparing `trytond_authentication_sms-7.0.0/locale/ru.po` & `trytond_authentication_sms-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/sl.po` & `trytond_authentication_sms-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/tr.po` & `trytond_authentication_sms-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/locale/zh_CN.po` & `trytond_authentication_sms-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/res.py` & `trytond_authentication_sms-7.2.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/res.xml` & `trytond_authentication_sms-7.2.0/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/setup.py` & `trytond_authentication_sms-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/tests/test_module.py` & `trytond_authentication_sms-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/tox.ini` & `trytond_authentication_sms-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/PKG-INFO` & `trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-authentication-sms
-Version: 7.0.0
+Name: trytond_authentication_sms
+Version: 7.2.0
 Summary: Tryton module to authenticate users via SMS
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
@@ -46,15 +46,15 @@
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
 
 Authentication SMS Module
 #########################
 
 The `SMS <https://en.wikipedia.org/wiki/Short_Message_Service>`_ authentication
 module allows users to authenticate via SMS.  It adds a new authentication
```

### Comparing `trytond_authentication_sms-7.0.0/trytond_authentication_sms.egg-info/SOURCES.txt` & `trytond_authentication_sms-7.2.0/trytond_authentication_sms.egg-info/SOURCES.txt`

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
 message.xml
```
