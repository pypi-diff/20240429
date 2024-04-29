# Comparing `tmp/trytond_project_plan-7.0.0.tar.gz` & `tmp/trytond_project_plan-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_plan-7.0.0.tar", last modified: Mon Oct 30 17:34:38 2023, max compression
+gzip compressed data, was "trytond_project_plan-7.2.0.tar", last modified: Mon Apr 29 15:44:54 2024, max compression
```

## Comparing `trytond_project_plan-7.0.0.tar` & `trytond_project_plan-7.2.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:38.130139 trytond_project_plan-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-10-22 17:23:12.000000 trytond_project_plan-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2023-10-30 17:10:09.000000 trytond_project_plan-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:10:09.000000 trytond_project_plan-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_plan-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3628 2023-10-30 17:34:38.130139 trytond_project_plan-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_project_plan-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1856 2023-08-13 15:26:13.000000 trytond_project_plan-7.0.0/allocation.py
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/allocation.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:38.130139 trytond_project_plan-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2813 2023-10-22 17:23:12.000000 trytond_project_plan-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:12.000000 trytond_project_plan-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:38.126806 trytond_project_plan-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3766 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3187 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3140 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3203 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3339 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2706 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2629 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2772 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3128 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2750 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3603 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3112 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3001 2023-10-28 12:11:24.000000 trytond_project_plan-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:34:38.130139 trytond_project_plan-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4273 2023-10-27 17:38:49.000000 trytond_project_plan-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:38.126806 trytond_project_plan-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_plan-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_project_plan-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_project_plan-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2023-10-30 17:10:05.000000 trytond_project_plan-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:38.130139 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3628 2023-10-30 17:34:37.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1507 2023-10-30 17:34:38.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:34:37.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-30 17:34:37.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-10-30 17:34:37.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:34:37.000000 trytond_project_plan-7.0.0/trytond_project_plan.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:38.126806 trytond_project_plan-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/view/allocation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/view/allocation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22865 2023-04-15 07:12:15.000000 trytond_project_plan-7.0.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)      965 2023-01-16 14:00:21.000000 trytond_project_plan-7.0.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2484 2024-04-29 15:23:13.000000 trytond_project_plan-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:23:13.000000 trytond_project_plan-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_plan-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3628 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_project_plan-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1856 2024-01-27 09:58:52.000000 trytond_project_plan-7.2.0/allocation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/allocation.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:54.542411 trytond_project_plan-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-27 16:30:39.000000 trytond_project_plan-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:19.000000 trytond_project_plan-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3766 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3187 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3140 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3203 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3339 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2706 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2629 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2772 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3128 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2750 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3212 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3603 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3112 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3001 2024-04-27 16:43:25.000000 trytond_project_plan-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4273 2024-03-17 11:01:36.000000 trytond_project_plan-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_plan-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_project_plan-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:19.000000 trytond_project_plan-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2024-04-29 15:23:09.000000 trytond_project_plan-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3628 2024-04-29 15:44:54.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1489 2024-04-29 15:44:54.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:54.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:44:54.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-29 15:44:54.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:54.000000 trytond_project_plan-7.2.0/trytond_project_plan.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:54.545744 trytond_project_plan-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/view/allocation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/view/allocation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22865 2023-04-15 07:12:15.000000 trytond_project_plan-7.2.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      965 2023-01-16 14:00:21.000000 trytond_project_plan-7.2.0/work.xml
```

### Comparing `trytond_project_plan-7.0.0/CHANGELOG` & `trytond_project_plan-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_project_plan-7.0.0/COPYRIGHT` & `trytond_project_plan-7.2.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2009-2013 Bertrand Chenal.
-Copyright (C) 2009-2023 Cédric Krier.
-Copyright (C) 2009-2023 B2CK SPRL.
+Copyright (C) 2009-2024 Cédric Krier.
+Copyright (C) 2009-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_project_plan-7.0.0/LICENSE` & `trytond_project_plan-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/PKG-INFO` & `trytond_project_plan-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_project_plan
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add planning capabilities on projects
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
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_project<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_project<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Project Plan Module
 ###################
 
 The Project Plan module adds planning features on top of the Project
 module.
```

### Comparing `trytond_project_plan-7.0.0/README.rst` & `trytond_project_plan-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/allocation.py` & `trytond_project_plan-7.2.0/allocation.py`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/allocation.xml` & `trytond_project_plan-7.2.0/allocation.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/doc/conf.py` & `trytond_project_plan-7.2.0/doc/conf.py`

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

### Comparing `trytond_project_plan-7.0.0/doc/index.rst` & `trytond_project_plan-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/bg.po` & `trytond_project_plan-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/ca.po` & `trytond_project_plan-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/cs.po` & `trytond_project_plan-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/de.po` & `trytond_project_plan-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/es.po` & `trytond_project_plan-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/es_419.po` & `trytond_project_plan-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/et.po` & `trytond_project_plan-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/fa.po` & `trytond_project_plan-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/fi.po` & `trytond_project_plan-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/fr.po` & `trytond_project_plan-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/hu.po` & `trytond_project_plan-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/id.po` & `trytond_project_plan-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/it.po` & `trytond_project_plan-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/lo.po` & `trytond_project_plan-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/lt.po` & `trytond_project_plan-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/nl.po` & `trytond_project_plan-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/pl.po` & `trytond_project_plan-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/pt.po` & `trytond_project_plan-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/ro.po` & `trytond_project_plan-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/ru.po` & `trytond_project_plan-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/sl.po` & `trytond_project_plan-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/tr.po` & `trytond_project_plan-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/uk.po` & `trytond_project_plan-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/locale/zh_CN.po` & `trytond_project_plan-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/setup.py` & `trytond_project_plan-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/tox.ini` & `trytond_project_plan-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/trytond_project_plan.egg-info/PKG-INFO` & `trytond_project_plan-7.2.0/trytond_project_plan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-project-plan
-Version: 7.0.0
+Name: trytond_project_plan
+Version: 7.2.0
 Summary: Tryton module to add planning capabilities on projects
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
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_project<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_project<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Project Plan Module
 ###################
 
 The Project Plan module adds planning features on top of the Project
 module.
```

### Comparing `trytond_project_plan-7.0.0/trytond_project_plan.egg-info/SOURCES.txt` & `trytond_project_plan-7.2.0/trytond_project_plan.egg-info/SOURCES.txt`

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
 allocation.py
```

### Comparing `trytond_project_plan-7.0.0/view/work_form.xml` & `trytond_project_plan-7.2.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/work.py` & `trytond_project_plan-7.2.0/work.py`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-7.0.0/work.xml` & `trytond_project_plan-7.2.0/work.xml`

 * *Files identical despite different names*

