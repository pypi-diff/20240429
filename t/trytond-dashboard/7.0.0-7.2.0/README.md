# Comparing `tmp/trytond_dashboard-7.0.0.tar.gz` & `tmp/trytond_dashboard-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_dashboard-7.0.0.tar", last modified: Mon Oct 30 17:29:36 2023, max compression
+gzip compressed data, was "trytond_dashboard-7.2.0.tar", last modified: Mon Apr 29 15:40:09 2024, max compression
```

## Comparing `trytond_dashboard-7.0.0.tar` & `trytond_dashboard-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:36.688701 trytond_dashboard-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-22 17:23:03.000000 trytond_dashboard-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2540 2023-10-30 17:06:14.000000 trytond_dashboard-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:06:14.000000 trytond_dashboard-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-10-30 17:29:36.688701 trytond_dashboard-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/dashboard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1013 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/dashboard.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:36.685368 trytond_dashboard-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2810 2023-10-22 17:23:03.000000 trytond_dashboard-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:03.000000 trytond_dashboard-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     4742 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:36.685368 trytond_dashboard-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1054 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1169 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1221 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1191 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1054 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1172 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1468 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1148 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1178 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-10-30 16:47:45.000000 trytond_dashboard-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1054 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1401 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1117 2023-10-28 12:11:22.000000 trytond_dashboard-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      912 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:29:36.688701 trytond_dashboard-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4134 2023-10-27 17:38:49.000000 trytond_dashboard-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:36.685368 trytond_dashboard-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-04-15 07:12:15.000000 trytond_dashboard-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_dashboard-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       93 2023-10-30 17:06:11.000000 trytond_dashboard-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:36.685368 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-10-30 17:29:36.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1658 2023-10-30 17:29:36.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:36.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-10-30 17:29:36.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       39 2023-10-30 17:29:36.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:29:36.000000 trytond_dashboard-7.0.0/trytond_dashboard.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:36.685368 trytond_dashboard-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/view/action_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/view/action_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/view/dashboard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-01-16 14:00:20.000000 trytond_dashboard-7.0.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:09.883190 trytond_dashboard-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2641 2024-04-29 15:19:31.000000 trytond_dashboard-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:19:31.000000 trytond_dashboard-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-04-29 15:40:09.883190 trytond_dashboard-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/dashboard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1013 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/dashboard.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:09.879856 trytond_dashboard-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-27 16:30:39.000000 trytond_dashboard-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:09.000000 trytond_dashboard-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     4742 2024-04-07 14:40:08.000000 trytond_dashboard-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1071 2024-04-27 16:30:39.000000 trytond_dashboard-7.2.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:09.879856 trytond_dashboard-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1357 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1054 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1169 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1221 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1191 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1054 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1172 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1468 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1148 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1178 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1259 2024-04-29 13:17:17.000000 trytond_dashboard-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1054 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1401 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1117 2024-04-27 16:43:24.000000 trytond_dashboard-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      912 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:09.883190 trytond_dashboard-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4134 2024-03-17 11:01:36.000000 trytond_dashboard-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:09.879856 trytond_dashboard-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-04-15 07:12:15.000000 trytond_dashboard-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:09.000000 trytond_dashboard-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       93 2024-04-29 15:19:27.000000 trytond_dashboard-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:09.883190 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-04-29 15:40:09.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1640 2024-04-29 15:40:09.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:09.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:40:09.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       39 2024-04-29 15:40:09.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:09.000000 trytond_dashboard-7.2.0/trytond_dashboard.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:09.883190 trytond_dashboard-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/view/action_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/view/action_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/view/dashboard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-01-16 14:00:20.000000 trytond_dashboard-7.2.0/view/user_form_preferences.xml
```

### Comparing `trytond_dashboard-7.0.0/CHANGELOG` & `trytond_dashboard-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_dashboard-7.0.0/COPYRIGHT` & `trytond_dashboard-7.2.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2023 Cédric Krier.
+Copyright (C) 2009-2024 Cédric Krier.
 Copyright (C) 2009-2013 Bertrand Chenal.
-Copyright (C) 2009-2023 B2CK SPRL.
+Copyright (C) 2009-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_dashboard-7.0.0/LICENSE` & `trytond_dashboard-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/PKG-INFO` & `trytond_dashboard-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_dashboard
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for dashboard
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
@@ -48,13 +48,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 
 Dashboard Module
 ################
 
 The dashboard module allows user to configure his dashboard.
```

### Comparing `trytond_dashboard-7.0.0/dashboard.py` & `trytond_dashboard-7.2.0/dashboard.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/dashboard.xml` & `trytond_dashboard-7.2.0/dashboard.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/doc/conf.py` & `trytond_dashboard-7.2.0/doc/conf.py`

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

### Comparing `trytond_dashboard-7.0.0/ir.py` & `trytond_dashboard-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/ir.xml` & `trytond_dashboard-7.2.0/ir.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_dashboard-7.0.0/ir.xml` & `trytond_dashboard-7.2.0/ir.xml`

```diff
@@ -1,20 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data>
     <record model="ir.ui.view" id="view_dashboard">
-      <field name="model"/>
+      <field name="model" eval="None"/>
       <field name="type">board</field>
       <field name="name">dashboard</field>
     </record>
     <record model="ir.action.act_window" id="act_dashboard">
       <field name="name">Dashboard</field>
-      <field name="res_model"/>
+      <field name="res_model" eval="None"/>
       <field name="type">ir.action.act_window</field>
     </record>
     <record model="ir.action.act_window.view" id="act_dashboard_view1">
       <field name="sequence" eval="1"/>
       <field name="view" ref="view_dashboard"/>
       <field name="act_window" ref="act_dashboard"/>
     </record>
```

### Comparing `trytond_dashboard-7.0.0/locale/bg.po` & `trytond_dashboard-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/ca.po` & `trytond_dashboard-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/cs.po` & `trytond_dashboard-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/de.po` & `trytond_dashboard-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/es.po` & `trytond_dashboard-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/es_419.po` & `trytond_dashboard-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/et.po` & `trytond_dashboard-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/fa.po` & `trytond_dashboard-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/fi.po` & `trytond_dashboard-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/fr.po` & `trytond_dashboard-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/hu.po` & `trytond_dashboard-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/id.po` & `trytond_dashboard-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/it.po` & `trytond_dashboard-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/lo.po` & `trytond_dashboard-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/lt.po` & `trytond_dashboard-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/nl.po` & `trytond_dashboard-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/pl.po` & `trytond_dashboard-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/pt.po` & `trytond_dashboard-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/ro.po` & `trytond_dashboard-7.2.0/locale/tr.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:dashboard.action,act_window:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:dashboard.action,user:"
 msgid "User"
-msgstr "Utilizator"
+msgstr ""
 
 msgctxt "field:res.user,dashboard_actions:"
 msgid "Dashboard Actions"
 msgstr ""
 
 msgctxt "field:res.user,dashboard_layout:"
 msgid "Dashboard Layout"
@@ -20,19 +20,19 @@
 
 msgctxt "model:dashboard.action,name:"
 msgid "Dashboard Action"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_dashboard"
 msgid "Dashboard"
-msgstr ""
+msgstr "Dashboard"
 
 msgctxt "model:ir.ui.menu,name:menu_dashboard"
 msgid "Dashboard"
-msgstr ""
+msgstr "Dashboard"
 
 msgctxt "selection:res.user,dashboard_layout:"
 msgid "Square"
 msgstr ""
 
 msgctxt "selection:res.user,dashboard_layout:"
 msgid "Stack Bottom"
@@ -46,10 +46,11 @@
 msgid "Stack Right"
 msgstr ""
 
 msgctxt "selection:res.user,dashboard_layout:"
 msgid "Stack Top"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:res.user:"
 msgid "Dashboard"
-msgstr ""
+msgstr "Dashboard"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_dashboard-7.0.0/locale/ru.po` & `trytond_dashboard-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/sl.po` & `trytond_dashboard-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/uk.po` & `trytond_dashboard-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/locale/zh_CN.po` & `trytond_dashboard-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/res.py` & `trytond_dashboard-7.2.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/res.xml` & `trytond_dashboard-7.2.0/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/setup.py` & `trytond_dashboard-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/tests/test_module.py` & `trytond_dashboard-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/tox.ini` & `trytond_dashboard-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/trytond_dashboard.egg-info/PKG-INFO` & `trytond_dashboard-7.2.0/trytond_dashboard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-dashboard
-Version: 7.0.0
+Name: trytond_dashboard
+Version: 7.2.0
 Summary: Tryton module for dashboard
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
@@ -48,13 +48,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 
 Dashboard Module
 ################
 
 The dashboard module allows user to configure his dashboard.
```

### Comparing `trytond_dashboard-7.0.0/trytond_dashboard.egg-info/SOURCES.txt` & `trytond_dashboard-7.2.0/trytond_dashboard.egg-info/SOURCES.txt`

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
 dashboard.py
```

### Comparing `trytond_dashboard-7.0.0/view/user_form.xml` & `trytond_dashboard-7.2.0/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-7.0.0/view/user_form_preferences.xml` & `trytond_dashboard-7.2.0/view/user_form_preferences.xml`

 * *Files identical despite different names*

