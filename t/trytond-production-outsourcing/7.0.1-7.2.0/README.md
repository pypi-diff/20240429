# Comparing `tmp/trytond_production_outsourcing-7.0.1.tar.gz` & `tmp/trytond_production_outsourcing-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_outsourcing-7.0.1.tar", last modified: Thu Feb 15 18:33:29 2024, max compression
+gzip compressed data, was "trytond_production_outsourcing-7.2.0.tar", last modified: Mon Apr 29 15:44:09 2024, max compression
```

## Comparing `trytond_production_outsourcing-7.0.1.tar` & `trytond_production_outsourcing-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:29.425599 trytond_production_outsourcing-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-02-15 18:33:26.000000 trytond_production_outsourcing-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-02-15 18:33:26.000000 trytond_production_outsourcing-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3113 2024-02-15 18:33:29.422266 trytond_production_outsourcing-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:29.418932 trytond_production_outsourcing-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2024-02-05 16:24:27.000000 trytond_production_outsourcing-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:29.422266 trytond_production_outsourcing-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1998 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2107 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2008 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1738 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2170 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2017 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2056 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1519 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9222 2024-02-10 10:12:06.000000 trytond_production_outsourcing-7.0.1/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      672 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-15 18:33:29.425599 trytond_production_outsourcing-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4467 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:29.422266 trytond_production_outsourcing-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4832 2024-02-05 16:24:27.000000 trytond_production_outsourcing-7.0.1/tests/scenario_production_outsourcing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      159 2024-02-05 16:24:27.000000 trytond_production_outsourcing-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:29.422266 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3113 2024-02-15 18:33:28.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1841 2024-02-15 18:33:29.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-15 18:33:28.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-02-15 18:33:28.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:58.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-02-15 18:33:28.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-15 18:33:28.000000 trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:29.422266 trytond_production_outsourcing-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/view/routing_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:38.000000 trytond_production_outsourcing-7.0.1/view/routing_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-29 15:22:35.000000 trytond_production_outsourcing-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:22:35.000000 trytond_production_outsourcing-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_outsourcing-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3113 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-01-16 14:00:21.000000 trytond_production_outsourcing-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:09.480256 trytond_production_outsourcing-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_production_outsourcing-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-01-16 14:00:21.000000 trytond_production_outsourcing-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:18.000000 trytond_production_outsourcing-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2107 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2008 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1738 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2170 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1553 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2017 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2056 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1519 2024-04-27 16:43:25.000000 trytond_production_outsourcing-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9203 2024-04-27 16:30:39.000000 trytond_production_outsourcing-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-01-16 14:00:21.000000 trytond_production_outsourcing-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      672 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_production_outsourcing-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4467 2024-03-17 11:01:36.000000 trytond_production_outsourcing-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4775 2024-04-27 16:30:39.000000 trytond_production_outsourcing-7.2.0/tests/scenario_production_outsourcing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:18.000000 trytond_production_outsourcing-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      159 2024-04-29 15:22:31.000000 trytond_production_outsourcing-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3113 2024-04-29 15:44:09.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1823 2024-04-29 15:44:09.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:09.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:44:09.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-04-29 15:44:09.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:09.000000 trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:09.483590 trytond_production_outsourcing-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:20.000000 trytond_production_outsourcing-7.2.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-01-16 14:00:20.000000 trytond_production_outsourcing-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-01-16 14:00:21.000000 trytond_production_outsourcing-7.2.0/view/routing_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_production_outsourcing-7.2.0/view/routing_list.xml
```

### Comparing `trytond_production_outsourcing-7.0.1/CHANGELOG` & `trytond_production_outsourcing-7.2.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-02-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_production_outsourcing-7.0.1/LICENSE` & `trytond_production_outsourcing-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/PKG-INFO` & `trytond_production_outsourcing-7.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_production_outsourcing
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to outsource production
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
@@ -47,21 +47,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_production_routing<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_production_routing<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Production Outsourcing Module
 #############################
 
 The production outsourcing module allows to outsource production order per
 routing. When such outsourced production is set to waiting, a purchase order is
 created and its cost is added to the production.
```

### Comparing `trytond_production_outsourcing-7.0.1/README.rst` & `trytond_production_outsourcing-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/__init__.py` & `trytond_production_outsourcing-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/doc/conf.py` & `trytond_production_outsourcing-7.2.0/doc/conf.py`

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

### Comparing `trytond_production_outsourcing-7.0.1/doc/index.rst` & `trytond_production_outsourcing-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/bg.po` & `trytond_production_outsourcing-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/ca.po` & `trytond_production_outsourcing-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/cs.po` & `trytond_production_outsourcing-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/de.po` & `trytond_production_outsourcing-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/es.po` & `trytond_production_outsourcing-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/es_419.po` & `trytond_production_outsourcing-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/et.po` & `trytond_production_outsourcing-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/fa.po` & `trytond_production_outsourcing-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/fi.po` & `trytond_production_outsourcing-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/fr.po` & `trytond_production_outsourcing-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/hu.po` & `trytond_production_outsourcing-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/id.po` & `trytond_production_outsourcing-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/it.po` & `trytond_production_outsourcing-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/lo.po` & `trytond_production_outsourcing-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/lt.po` & `trytond_production_outsourcing-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/nl.po` & `trytond_production_outsourcing-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/pl.po` & `trytond_production_outsourcing-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/pt.po` & `trytond_production_outsourcing-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/ro.po` & `trytond_production_outsourcing-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/ru.po` & `trytond_production_outsourcing-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/sl.po` & `trytond_production_outsourcing-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/tr.po` & `trytond_production_outsourcing-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/uk.po` & `trytond_production_outsourcing-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/locale/zh_CN.po` & `trytond_production_outsourcing-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/production.py` & `trytond_production_outsourcing-7.2.0/production.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         if line.unit_price is None:
             line.unit_price = round_price(Decimal(0))
         return line
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, productions):
+    def do(cls, productions):
         pool = Pool()
         Warning = pool.get('res.user.warning')
 
         def pending_purchase(production):
             return any(l.purchase_state in {'draft', 'quotation'}
                 for l in production.purchase_lines)
         pendings = list(filter(pending_purchase, productions))
@@ -238,8 +238,8 @@
                 names += '...'
             warning_name = Warning.format('pending_purchase.done', pendings)
             if Warning.check(warning_name):
                 raise PurchaseWarning(
                     warning_name,
                     gettext('production_outsourcing.msg_pending_purchase_done',
                         productions=names))
-        super(Production, cls).done(productions)
+        super().do(productions)
```

### Comparing `trytond_production_outsourcing-7.0.1/production.xml` & `trytond_production_outsourcing-7.2.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/purchase.py` & `trytond_production_outsourcing-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/setup.py` & `trytond_production_outsourcing-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/tests/scenario_production_outsourcing.rst` & `trytond_production_outsourcing-7.2.0/tests/scenario_production_outsourcing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ===============================
 Production Outsourcing Scenario
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('production_outsourcing')
 
 Create company::
 
@@ -103,16 +102,15 @@
 
 Create Routing::
 
     >>> Routing = Model.get('production.routing')
     >>> routing = Routing(name="Supplier")
     >>> routing.supplier = supplier
     >>> routing.supplier_service = service
-    >>> routing.supplier_service_supplier == service_supplier
-    True
+    >>> assertEqual(routing.supplier_service_supplier, service_supplier)
     >>> routing.supplier_quantity = 2
     >>> routing.boms.append(bom)
     >>> routing.save()
 
 Set Bill of Material and Routing to the Product::
 
     >>> ProductBOM = Model.get('product.product-production.bom')
@@ -127,18 +125,16 @@
     >>> production.bom = bom
     >>> production.routing = routing
     >>> production.quantity = 10
     >>> production.click('wait')
     >>> production.state
     'waiting'
     >>> purchase_line, = production.purchase_lines
-    >>> purchase_line.product == service
-    True
-    >>> purchase_line.product_supplier == service_supplier
-    True
+    >>> assertEqual(purchase_line.product, service)
+    >>> assertEqual(purchase_line.product_supplier, service_supplier)
     >>> purchase_line.quantity
     20.0
     >>> production.cost
     Decimal('410.0000')
 
 Reset to draft::
 
@@ -147,22 +143,22 @@
     []
 
 Try to do the production with pending purchase::
 
     >>> production.click('wait')
     >>> production.click('assign_force')
     >>> production.click('run')
-    >>> production.click('done')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> production.click('do')
     Traceback (most recent call last):
         ...
     PurchaseWarning: ...
 
 Validate the purchase::
 
     >>> purchase_line, = production.purchase_lines
     >>> purchase = purchase_line.purchase
     >>> purchase.click('quote')
     >>> purchase.click('confirm')
 
 Do the production::
 
-    >>> production.click('done')
+    >>> production.click('do')
```

### Comparing `trytond_production_outsourcing-7.0.1/tox.ini` & `trytond_production_outsourcing-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/PKG-INFO` & `trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_production_outsourcing
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to outsource production
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
@@ -47,21 +47,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_production_routing<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_production_routing<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Production Outsourcing Module
 #############################
 
 The production outsourcing module allows to outsource production order per
 routing. When such outsourced production is set to waiting, a purchase order is
 created and its cost is added to the production.
```

### Comparing `trytond_production_outsourcing-7.0.1/trytond_production_outsourcing.egg-info/SOURCES.txt` & `trytond_production_outsourcing-7.2.0/trytond_production_outsourcing.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_production_outsourcing-7.0.1/view/routing_form.xml` & `trytond_production_outsourcing-7.2.0/view/routing_form.xml`

 * *Files identical despite different names*

