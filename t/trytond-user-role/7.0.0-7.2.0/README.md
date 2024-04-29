# Comparing `tmp/trytond_user_role-7.0.0.tar.gz` & `tmp/trytond_user_role-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_user_role-7.0.0.tar", last modified: Mon Oct 30 17:44:59 2023, max compression
+gzip compressed data, was "trytond_user_role-7.2.0.tar", last modified: Mon Apr 29 15:53:58 2024, max compression
```

## Comparing `trytond_user_role-7.0.0.tar` & `trytond_user_role-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:59.106434 trytond_user_role-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-22 17:23:29.000000 trytond_user_role-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1003 2023-10-30 17:16:10.000000 trytond_user_role-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:16:09.000000 trytond_user_role-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2601 2023-10-30 17:44:59.106434 trytond_user_role-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:59.103101 trytond_user_role-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2810 2023-10-22 17:23:29.000000 trytond_user_role-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:29.000000 trytond_user_role-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:59.103101 trytond_user_role-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1391 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1249 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1131 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1213 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1220 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1096 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1231 2023-10-30 16:47:45.000000 trytond_user_role-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-10-28 12:11:27.000000 trytond_user_role-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3604 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3975 2023-10-07 15:40:36.000000 trytond_user_role-7.0.0/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:44:59.106434 trytond_user_role-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4356 2023-10-27 17:38:49.000000 trytond_user_role-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:59.103101 trytond_user_role-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1992 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/tests/scenario_user_role.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_user_role-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:16:06.000000 trytond_user_role-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:59.106434 trytond_user_role-7.0.0/trytond_user_role.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2601 2023-10-30 17:44:58.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-10-30 17:44:59.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:44:58.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:44:58.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-10-30 17:44:58.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:44:58.000000 trytond_user_role-7.0.0/trytond_user_role.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:59.103101 trytond_user_role-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/view/role_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/view/role_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/view/user_role_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_user_role-7.0.0/view/user_role_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:58.401520 trytond_user_role-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-29 15:29:51.000000 trytond_user_role-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:29:51.000000 trytond_user_role-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2601 2024-04-29 15:53:58.401520 trytond_user_role-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:58.394854 trytond_user_role-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-27 16:30:39.000000 trytond_user_role-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:38.000000 trytond_user_role-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:58.398187 trytond_user_role-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1207 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1217 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1391 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1249 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1131 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1213 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1220 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1204 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1096 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1231 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2024-04-27 16:43:28.000000 trytond_user_role-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3604 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3883 2024-04-27 16:30:39.000000 trytond_user_role-7.2.0/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:58.401520 trytond_user_role-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4356 2024-03-17 11:01:36.000000 trytond_user_role-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:58.398187 trytond_user_role-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-22 12:14:37.000000 trytond_user_role-7.2.0/tests/scenario_user_role.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:38.000000 trytond_user_role-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:29:46.000000 trytond_user_role-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:58.398187 trytond_user_role-7.2.0/trytond_user_role.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2601 2024-04-29 15:53:57.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1600 2024-04-29 15:53:58.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:57.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:53:57.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-04-29 15:53:57.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:57.000000 trytond_user_role-7.2.0/trytond_user_role.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:58.398187 trytond_user_role-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/view/role_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/view/role_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/view/user_role_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_user_role-7.2.0/view/user_role_list.xml
```

### Comparing `trytond_user_role-7.0.0/CHANGELOG` & `trytond_user_role-7.2.0/CHANGELOG`

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

### Comparing `trytond_user_role-7.0.0/COPYRIGHT` & `trytond_user_role-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_user_role-7.0.0/LICENSE` & `trytond_user_role-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/PKG-INFO` & `trytond_user_role-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_user_role
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to manage role on user
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
@@ -47,17 +47,17 @@
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
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 User Role Module
 ################
 
 The user_role module allows to assign roles to user instead of groups.
 A *Role* is defined by a set of groups. When a role is added to a user, it
 overrides the existing groups. A role can be added to a user for a period.
```

### Comparing `trytond_user_role-7.0.0/__init__.py` & `trytond_user_role-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/doc/conf.py` & `trytond_user_role-7.2.0/doc/conf.py`

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

### Comparing `trytond_user_role-7.0.0/locale/bg.po` & `trytond_user_role-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/ca.po` & `trytond_user_role-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/cs.po` & `trytond_user_role-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/de.po` & `trytond_user_role-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/es.po` & `trytond_user_role-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/es_419.po` & `trytond_user_role-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/et.po` & `trytond_user_role-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/fa.po` & `trytond_user_role-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/fi.po` & `trytond_user_role-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/fr.po` & `trytond_user_role-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/hu.po` & `trytond_user_role-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/id.po` & `trytond_user_role-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/it.po` & `trytond_user_role-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/lo.po` & `trytond_user_role-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/lt.po` & `trytond_user_role-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/nl.po` & `trytond_user_role-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/pl.po` & `trytond_user_role-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/pt.po` & `trytond_user_role-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/ro.po` & `trytond_user_role-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/ru.po` & `trytond_user_role-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/sl.po` & `trytond_user_role-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/tr.po` & `trytond_user_role-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/uk.po` & `trytond_user_role-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/locale/zh_CN.po` & `trytond_user_role-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/res.py` & `trytond_user_role-7.2.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/res.xml` & `trytond_user_role-7.2.0/res.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_user_role-7.0.0/res.xml` & `trytond_user_role-7.2.0/res.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_role_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="role_view_form"/>
       <field name="act_window" ref="act_role_form"/>
     </record>
     <menuitem parent="res.menu_res" action="act_role_form" sequence="50" id="menu_role_form"/>
     <record model="ir.model.access" id="access_role">
-      <field name="model" search="[('model', '=', 'res.role')]"/>
+      <field name="model">res.role</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_role_admin">
-      <field name="model" search="[('model', '=', 'res.role')]"/>
+      <field name="model">res.role</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="user_view_form">
@@ -55,22 +55,22 @@
     </record>
     <record model="ir.ui.view" id="user_role_list">
       <field name="model">res.user.role</field>
       <field name="type">tree</field>
       <field name="name">user_role_list</field>
     </record>
     <record model="ir.model.access" id="access_user_role">
-      <field name="model" search="[('model', '=', 'res.user.role')]"/>
+      <field name="model">res.user.role</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_user_role_admin">
-      <field name="model" search="[('model', '=', 'res.user.role')]"/>
+      <field name="model">res.user.role</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.cron" id="cron_sync_roles">
```

### Comparing `trytond_user_role-7.0.0/setup.py` & `trytond_user_role-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/tests/scenario_user_role.rst` & `trytond_user_role-7.2.0/tests/scenario_user_role.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ==================
 User Role Scenario
 ==================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+
+    >>> from proteus import Model
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('user_role')
 
 Create some groups::
 
@@ -41,16 +42,15 @@
 
     >>> user_role = user.roles.new()
     >>> user_role.role = role
     >>> user.save()
 
     >>> len(user.groups)
     2
-    >>> user.groups == [groups[0], groups[1]]
-    True
+    >>> assertEqual(user.groups, [groups[0], groups[1]])
 
 Start the role in the future::
 
     >>> user_role, = user.roles
     >>> user_role.from_date = dt.datetime.now() + dt.timedelta(days=1)
     >>> user_role.to_date = None
     >>> user.save()
```

### Comparing `trytond_user_role-7.0.0/tox.ini` & `trytond_user_role-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_user_role-7.0.0/trytond_user_role.egg-info/PKG-INFO` & `trytond_user_role-7.2.0/trytond_user_role.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-user-role
-Version: 7.0.0
+Name: trytond_user_role
+Version: 7.2.0
 Summary: Tryton module to manage role on user
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
@@ -47,17 +47,17 @@
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
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 User Role Module
 ################
 
 The user_role module allows to assign roles to user instead of groups.
 A *Role* is defined by a set of groups. When a role is added to a user, it
 overrides the existing groups. A role can be added to a user for a period.
```

### Comparing `trytond_user_role-7.0.0/trytond_user_role.egg-info/SOURCES.txt` & `trytond_user_role-7.2.0/trytond_user_role.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 ir.py
```

