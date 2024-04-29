# Comparing `tmp/trytond_party_relationship-7.0.0.tar.gz` & `tmp/trytond_party_relationship-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party_relationship-7.0.0.tar", last modified: Mon Oct 30 17:31:44 2023, max compression
+gzip compressed data, was "trytond_party_relationship-7.2.0.tar", last modified: Mon Apr 29 15:42:08 2024, max compression
```

## Comparing `trytond_party_relationship-7.0.0.tar` & `trytond_party_relationship-7.2.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:44.389310 trytond_party_relationship-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:07.000000 trytond_party_relationship-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1849 2023-10-30 17:07:49.000000 trytond_party_relationship-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-10-30 17:07:49.000000 trytond_party_relationship-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party_relationship-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3291 2023-10-30 17:31:44.389310 trytond_party_relationship-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:44.385977 trytond_party_relationship-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:07.000000 trytond_party_relationship-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:07.000000 trytond_party_relationship-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:44.385977 trytond_party_relationship-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2237 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2113 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2261 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2294 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1955 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2100 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2257 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2015 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2186 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2274 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2231 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2288 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2238 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2258 2023-10-30 16:47:45.000000 trytond_party_relationship-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2100 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1955 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2206 2023-10-28 12:11:23.000000 trytond_party_relationship-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12209 2023-08-13 15:26:13.000000 trytond_party_relationship-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4075 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:31:44.389310 trytond_party_relationship-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2023-10-27 17:38:49.000000 trytond_party_relationship-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:44.385977 trytond_party_relationship-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10602 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_party_relationship-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       61 2023-10-30 17:07:39.000000 trytond_party_relationship-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:44.389310 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3291 2023-10-30 17:31:43.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-10-30 17:31:44.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:31:43.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:31:43.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:31:43.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:31:43.000000 trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:44.385977 trytond_party_relationship-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-01-16 14:00:20.000000 trytond_party_relationship-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/view/relation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/view/relation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/view/relation_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_party_relationship-7.0.0/view/relation_type_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1950 2024-04-29 15:21:03.000000 trytond_party_relationship-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2024-04-29 15:21:02.000000 trytond_party_relationship-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party_relationship-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3291 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:08.640083 trytond_party_relationship-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_party_relationship-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:13.000000 trytond_party_relationship-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2237 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2269 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2113 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2261 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2294 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1955 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2100 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2257 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2269 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2015 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2186 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2274 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2231 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2288 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2238 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2258 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2100 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1955 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2206 2024-04-27 16:43:24.000000 trytond_party_relationship-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12209 2024-01-27 09:58:52.000000 trytond_party_relationship-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3997 2024-04-27 16:30:39.000000 trytond_party_relationship-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2024-03-17 11:01:36.000000 trytond_party_relationship-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10602 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:13.000000 trytond_party_relationship-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       61 2024-04-29 15:20:58.000000 trytond_party_relationship-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3291 2024-04-29 15:42:08.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1583 2024-04-29 15:42:08.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:08.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:42:08.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:42:08.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:08.000000 trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:08.643417 trytond_party_relationship-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-01-16 14:00:20.000000 trytond_party_relationship-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/view/relation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/view/relation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/view/relation_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_party_relationship-7.2.0/view/relation_type_tree.xml
```

### Comparing `trytond_party_relationship-7.0.0/CHANGELOG` & `trytond_party_relationship-7.2.0/CHANGELOG`

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

### Comparing `trytond_party_relationship-7.0.0/COPYRIGHT` & `trytond_party_relationship-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2013 NaN·tic
-Copyright (C) 2014-2023 Cédric Krier.
-Copyright (C) 2014-2023 B2CK SPRL.
+Copyright (C) 2014-2024 Cédric Krier.
+Copyright (C) 2014-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_party_relationship-7.0.0/LICENSE` & `trytond_party_relationship-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/PKG-INFO` & `trytond_party_relationship-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_party_relationship
-Version: 7.0.0
+Version: 7.2.0
 Summary: Party Relationship module for Tryton
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Party Relationship Module
 #########################
 
 The party relationship module allows to define different types of relations
 between parties.
```

### Comparing `trytond_party_relationship-7.0.0/README.rst` & `trytond_party_relationship-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/doc/conf.py` & `trytond_party_relationship-7.2.0/doc/conf.py`

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

### Comparing `trytond_party_relationship-7.0.0/doc/index.rst` & `trytond_party_relationship-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/bg.po` & `trytond_party_relationship-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/ca.po` & `trytond_party_relationship-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/cs.po` & `trytond_party_relationship-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/de.po` & `trytond_party_relationship-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/es.po` & `trytond_party_relationship-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/es_419.po` & `trytond_party_relationship-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/et.po` & `trytond_party_relationship-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/fa.po` & `trytond_party_relationship-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/fi.po` & `trytond_party_relationship-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/fr.po` & `trytond_party_relationship-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/hu.po` & `trytond_party_relationship-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/id.po` & `trytond_party_relationship-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/it.po` & `trytond_party_relationship-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/lo.po` & `trytond_party_relationship-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/lt.po` & `trytond_party_relationship-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/nl.po` & `trytond_party_relationship-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/pl.po` & `trytond_party_relationship-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/pt.po` & `trytond_party_relationship-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/ro.po` & `trytond_party_relationship-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/ru.po` & `trytond_party_relationship-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/sl.po` & `trytond_party_relationship-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/tr.po` & `trytond_party_relationship-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/uk.po` & `trytond_party_relationship-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/locale/zh_CN.po` & `trytond_party_relationship-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/party.py` & `trytond_party_relationship-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/party.xml` & `trytond_party_relationship-7.2.0/party.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_party_relationship-7.0.0/party.xml` & `trytond_party_relationship-7.2.0/party.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_relation_type_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="relation_type_view_form"/>
       <field name="act_window" ref="act_relation_type"/>
     </record>
     <menuitem parent="party.menu_configuration" sequence="20" action="act_relation_type" id="menu_relation_type"/>
     <record model="ir.model.access" id="access_relation_type">
-      <field name="model" search="[('model', '=', 'party.relation.type')]"/>
+      <field name="model">party.relation.type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_relation_type_admin">
-      <field name="model" search="[('model', '=', 'party.relation.type')]"/>
+      <field name="model">party.relation.type</field>
       <field name="group" ref="party.group_party_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="relation_view_tree">
```

### Comparing `trytond_party_relationship-7.0.0/setup.py` & `trytond_party_relationship-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/tests/test_module.py` & `trytond_party_relationship-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/tox.ini` & `trytond_party_relationship-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/PKG-INFO` & `trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-party-relationship
-Version: 7.0.0
+Name: trytond_party_relationship
+Version: 7.2.0
 Summary: Party Relationship module for Tryton
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Party Relationship Module
 #########################
 
 The party relationship module allows to define different types of relations
 between parties.
```

### Comparing `trytond_party_relationship-7.0.0/trytond_party_relationship.egg-info/SOURCES.txt` & `trytond_party_relationship-7.2.0/trytond_party_relationship.egg-info/SOURCES.txt`

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
 party.py
```

### Comparing `trytond_party_relationship-7.0.0/view/relation_form.xml` & `trytond_party_relationship-7.2.0/view/relation_form.xml`

 * *Files identical despite different names*
