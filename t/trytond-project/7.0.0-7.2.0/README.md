# Comparing `tmp/trytond_project-7.0.0.tar.gz` & `tmp/trytond_project-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project-7.0.0.tar", last modified: Mon Oct 30 17:34:23 2023, max compression
+gzip compressed data, was "trytond_project-7.2.0.tar", last modified: Mon Apr 29 15:44:40 2024, max compression
```

## Comparing `trytond_project-7.0.0.tar` & `trytond_project-7.2.0.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.500069 trytond_project-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-22 17:23:12.000000 trytond_project-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3537 2023-10-30 17:10:00.000000 trytond_project-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:10:00.000000 trytond_project-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2023-10-30 17:34:23.500069 trytond_project-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_project-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.496736 trytond_project-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-22 17:23:12.000000 trytond_project-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3201 2023-04-15 07:12:15.000000 trytond_project-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_project-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:12.000000 trytond_project-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-15 07:12:15.000000 trytond_project-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_project-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.496736 trytond_project-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_project-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-01-16 14:00:21.000000 trytond_project-7.0.0/icons/tryton-project.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_project-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.496736 trytond_project-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7126 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7477 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6169 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7909 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7467 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6240 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6437 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7513 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6143 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7520 2023-10-30 16:47:45.000000 trytond_project-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6409 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5965 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6337 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6676 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6218 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7426 2023-10-30 16:47:45.000000 trytond_project-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6385 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7106 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-10-30 16:47:45.000000 trytond_project-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7382 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7289 2023-10-30 16:47:45.000000 trytond_project-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6157 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5961 2023-10-28 12:11:24.000000 trytond_project-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2023-10-30 16:47:45.000000 trytond_project-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_project-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-04-15 07:12:15.000000 trytond_project-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-04-15 07:12:15.000000 trytond_project-7.0.0/project.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:34:23.500069 trytond_project-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4528 2023-10-27 17:38:49.000000 trytond_project-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.496736 trytond_project-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2201 2023-04-15 07:12:15.000000 trytond_project-7.0.0/tests/scenario_project_status.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7386 2023-04-15 07:12:15.000000 trytond_project-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1288 2023-04-15 07:12:15.000000 trytond_project-7.0.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1117 2023-04-15 07:12:15.000000 trytond_project-7.0.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_project-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-10-30 17:09:56.000000 trytond_project-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.500069 trytond_project-7.0.0/trytond_project.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2023-10-30 17:34:23.000000 trytond_project-7.0.0/trytond_project.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2064 2023-10-30 17:34:23.000000 trytond_project-7.0.0/trytond_project.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:34:23.000000 trytond_project-7.0.0/trytond_project.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-10-30 17:34:23.000000 trytond_project-7.0.0/trytond_project.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_project-7.0.0/trytond_project.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-10-30 17:34:23.000000 trytond_project-7.0.0/trytond_project.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:34:23.000000 trytond_project-7.0.0/trytond_project.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:23.496736 trytond_project-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_list_children.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_status_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_status_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_project-7.0.0/view/work_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16077 2023-10-07 15:40:36.000000 trytond_project-7.0.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12059 2023-04-15 07:12:15.000000 trytond_project-7.0.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.802770 trytond_project-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-29 15:23:02.000000 trytond_project-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:23:02.000000 trytond_project-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-04-29 15:44:40.802770 trytond_project-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_project-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_project-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3201 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:19.000000 trytond_project-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-15 07:12:15.000000 trytond_project-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_project-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_project-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-01-16 14:00:21.000000 trytond_project-7.2.0/icons/tryton-project.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_project-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7126 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7477 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6169 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7909 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7467 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6240 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6437 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7513 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6143 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7520 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6409 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5965 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6337 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6676 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6218 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7426 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6385 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7106 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7236 2024-04-29 13:17:17.000000 trytond_project-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7382 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6157 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-27 16:43:25.000000 trytond_project-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_project-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-04-15 07:12:15.000000 trytond_project-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-04-15 07:12:15.000000 trytond_project-7.2.0/project.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:40.802770 trytond_project-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4519 2024-04-27 16:30:39.000000 trytond_project-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.799437 trytond_project-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2024-04-22 12:14:36.000000 trytond_project-7.2.0/tests/scenario_project_status.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7386 2023-04-15 07:12:15.000000 trytond_project-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1288 2023-04-15 07:12:15.000000 trytond_project-7.2.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1117 2023-04-15 07:12:15.000000 trytond_project-7.2.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:19.000000 trytond_project-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2024-04-29 15:22:58.000000 trytond_project-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.802770 trytond_project-7.2.0/trytond_project.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2046 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_project-7.2.0/trytond_project.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:40.000000 trytond_project-7.2.0/trytond_project.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:40.802770 trytond_project-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_list_children.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_status_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_status_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_project-7.2.0/view/work_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16077 2024-01-27 09:58:52.000000 trytond_project-7.2.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11944 2024-04-27 16:30:39.000000 trytond_project-7.2.0/work.xml
```

### Comparing `trytond_project-7.0.0/CHANGELOG` & `trytond_project-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_project-7.0.0/COPYRIGHT` & `trytond_project-7.2.0/COPYRIGHT`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2008-2023 Cédric Krier.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 Cédric Krier.
+Copyright (C) 2008-2024 B2CK SPRL.
 Copyright (C) 2009-2013 Bertrand Chenal.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_project-7.0.0/LICENSE` & `trytond_project-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/PKG-INFO` & `trytond_project-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_project
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with projects
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-project/
+Project-URL: Documentation, https://docs.tryton.org/modules-project/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,21 +49,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_company_work_time<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_company_work_time<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##############
 Project Module
 ##############
 
 The *Project Module* contains the basic concepts that are needed for managing
 simple projects.
```

### Comparing `trytond_project-7.0.0/__init__.py` & `trytond_project-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/doc/conf.py` & `trytond_project-7.2.0/doc/conf.py`

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

### Comparing `trytond_project-7.0.0/doc/design.rst` & `trytond_project-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/doc/usage.rst` & `trytond_project-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/icons/LICENSE` & `trytond_project-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/ir.py` & `trytond_project-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/bg.po` & `trytond_project-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/ca.po` & `trytond_project-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/cs.po` & `trytond_project-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/de.po` & `trytond_project-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/es.po` & `trytond_project-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/es_419.po` & `trytond_project-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/et.po` & `trytond_project-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/fa.po` & `trytond_project-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/fi.po` & `trytond_project-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/fr.po` & `trytond_project-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/hu.po` & `trytond_project-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/id.po` & `trytond_project-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/it.po` & `trytond_project-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/lo.po` & `trytond_project-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/lt.po` & `trytond_project-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/nl.po` & `trytond_project-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/pl.po` & `trytond_project-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/pt.po` & `trytond_project-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/ro.po` & `trytond_project-7.2.0/locale/uk.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,children:"
 msgid "Children"
-msgstr "Copii"
+msgstr ""
 
 msgctxt "field:project.work,comment:"
 msgid "Comment"
-msgstr "Comentariu"
+msgstr ""
 
 msgctxt "field:project.work,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:project.work,effort_duration:"
 msgid "Effort"
-msgstr "Efort"
+msgstr ""
 
 msgctxt "field:project.work,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr ""
 
 msgctxt "field:project.work,parent:"
 msgid "Parent"
-msgstr "Părinte"
+msgstr ""
 
 msgctxt "field:project.work,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:project.work,party_address:"
 msgid "Contact Address"
 msgstr ""
 
 msgctxt "field:project.work,path:"
 msgid "Path"
@@ -136,27 +136,27 @@
 
 msgctxt "help:project.work.status,types:"
 msgid "The type of works which can use this status."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_child_work"
 msgid "Tasks"
-msgstr "Sarcini"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_project_form"
 msgid "Projects"
-msgstr "Proiecte"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_project_tree"
 msgid "Projects"
-msgstr "Proiecte"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_task_form"
 msgid "Tasks"
-msgstr "Sarcini"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_timesheet_line_form_work"
 msgid "Timesheet Lines"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works Efforts"
@@ -192,39 +192,39 @@
 
 msgctxt "model:ir.message,text:msg_work_parent_progress"
 msgid "To re-open work \"%(work)s\" you must re-open also its parent \"%(parent)s\"."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Налаштування"
 
 msgctxt "model:ir.ui.menu,name:menu_project"
 msgid "Projects"
-msgstr "Proiecte"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_project_form"
 msgid "Projects"
-msgstr "Proiecte"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_project_tree"
 msgid "Projects"
-msgstr "Proiecte"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Raportare"
+msgstr "Звітність"
 
 msgctxt "model:ir.ui.menu,name:menu_task_form"
 msgid "Tasks"
-msgstr "Sarcini"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works Efforts"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_work_status"
 msgid "Work Status"
@@ -256,15 +256,15 @@
 
 msgctxt "selection:project.work,type:"
 msgid "Project"
 msgstr ""
 
 msgctxt "selection:project.work,type:"
 msgid "Task"
-msgstr "Sarcina"
+msgstr ""
 
 msgctxt "view:project.work.status:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:project.work:"
 msgid "%"
```

### Comparing `trytond_project-7.0.0/locale/ru.po` & `trytond_project-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/sl.po` & `trytond_project-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/tr.po` & `trytond_project-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/locale/zh_CN.po` & `trytond_project-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/message.xml` & `trytond_project-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/party.py` & `trytond_project-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/project.xml` & `trytond_project-7.2.0/project.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/setup.py` & `trytond_project-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-project/',
+        "Documentation": 'https://docs.tryton.org/modules-project/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton project',
     package_dir={'trytond.modules.project': '.'},
     packages=(
         ['trytond.modules.project']
```

### Comparing `trytond_project-7.0.0/tests/scenario_project_status.rst` & `trytond_project-7.2.0/tests/scenario_project_status.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 =======================
 Project Status Scenario
 =======================
 
 Imports::
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate project::
 
     >>> config = activate_modules('project')
 
 Create a company::
 
@@ -26,19 +26,17 @@
     >>> done, = WorkStatus.find([('name', '=', "Done")])
 
 Create a project with a task::
 
     >>> Work = Model.get('project.work')
 
     >>> project = Work(type='project', name="Project")
-    >>> project.status == open
-    True
+    >>> assertEqual(project.status, open)
     >>> task = project.children.new(name="Task")
-    >>> task.status == open
-    True
+    >>> assertEqual(task.status, open)
 
     >>> project.save()
     >>> task, = project.children
 
 Open the project::
 
     >>> project.status = in_progress
@@ -47,36 +45,36 @@
     >>> project.save()
 
 Try to complete project without task::
 
     >>> project.status = done
     >>> project.progress
     1.0
-    >>> project.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> project.save()
     Traceback (most recent call last):
         ...
     WorkProgressValidationError: ...
 
     >>> task, = project.children
     >>> task.progress = 1
     >>> project.save()
 
 Try to re-open task without project::
 
     >>> task = Work(task.id)
     >>> task.progress = 0.5
-    >>> task.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> task.save()
     Traceback (most recent call last):
         ...
     WorkProgressValidationError: ...
 
 Change progress with updating status::
 
     >>> project.progress = 0.8
-    >>> project.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> project.save()
     Traceback (most recent call last):
         ...
     WorkProgressValidationError: ...
 
     >>> project.status = in_progress
     >>> project.save()
 
@@ -85,10 +83,9 @@
     >>> task = Work(task.id)
     >>> task.progress = 0.5
     >>> task.save()
 
 Copy the project::
 
     >>> project_copy, = project.duplicate()
-    >>> project_copy.status == open
-    True
+    >>> assertEqual(project_copy.status, open)
     >>> project_copy.progress
```

### Comparing `trytond_project-7.0.0/tests/test_module.py` & `trytond_project-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/timesheet.py` & `trytond_project-7.2.0/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/timesheet.xml` & `trytond_project-7.2.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/tox.ini` & `trytond_project-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/trytond_project.egg-info/PKG-INFO` & `trytond_project-7.2.0/trytond_project.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-project
-Version: 7.0.0
+Name: trytond_project
+Version: 7.2.0
 Summary: Tryton module with projects
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-project/
+Project-URL: Documentation, https://docs.tryton.org/modules-project/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,21 +49,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_company_work_time<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_company_work_time<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##############
 Project Module
 ##############
 
 The *Project Module* contains the basic concepts that are needed for managing
 simple projects.
```

### Comparing `trytond_project-7.0.0/trytond_project.egg-info/SOURCES.txt` & `trytond_project-7.2.0/trytond_project.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_project-7.0.0/view/work_form.xml` & `trytond_project-7.2.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/view/work_list.xml` & `trytond_project-7.2.0/view/work_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/view/work_status_form.xml` & `trytond_project-7.2.0/view/work_status_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/view/work_tree.xml` & `trytond_project-7.2.0/view/work_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/work.py` & `trytond_project-7.2.0/work.py`

 * *Files identical despite different names*

### Comparing `trytond_project-7.0.0/work.xml` & `trytond_project-7.2.0/work.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_project-7.0.0/work.xml` & `trytond_project-7.2.0/work.xml`

```diff
@@ -26,30 +26,30 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="work_status_view_form"/>
       <field name="act_window" ref="act_work_status"/>
     </record>
     <menuitem parent="menu_configuration" sequence="20" action="act_work_status" id="menu_work_status"/>
     <record model="ir.rule.group" id="rule_group_work_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'project.work')]"/>
+      <field name="model">project.work</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_work_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_work_companies"/>
     </record>
     <record model="ir.model.access" id="access_work_status">
-      <field name="model" search="[('model', '=', 'project.work.status')]"/>
+      <field name="model">project.work.status</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_status_admin">
-      <field name="model" search="[('model', '=', 'project.work.status')]"/>
+      <field name="model">project.work.status</field>
       <field name="group" ref="group_project_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="work_view_tree">
@@ -187,22 +187,22 @@
     </record>
     <record model="ir.action.act_window.view" id="act_open_project_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="work_view_form"/>
       <field name="act_window" ref="act_open_child_work"/>
     </record>
     <record model="ir.model.access" id="access_work">
-      <field name="model" search="[('model', '=', 'project.work')]"/>
+      <field name="model">project.work</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_admin">
-      <field name="model" search="[('model', '=', 'project.work')]"/>
+      <field name="model">project.work</field>
       <field name="group" ref="group_project_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

