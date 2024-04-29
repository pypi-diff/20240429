# Comparing `tmp/trytond_party_avatar-7.0.0.tar.gz` & `tmp/trytond_party_avatar-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party_avatar-7.0.0.tar", last modified: Mon Oct 30 17:31:38 2023, max compression
+gzip compressed data, was "trytond_party_avatar-7.2.0.tar", last modified: Mon Apr 29 15:42:02 2024, max compression
```

## Comparing `trytond_party_avatar-7.0.0.tar` & `trytond_party_avatar-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:38.362615 trytond_party_avatar-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-10-22 17:23:07.000000 trytond_party_avatar-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-10-30 17:07:37.000000 trytond_party_avatar-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:07:37.000000 trytond_party_avatar-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2544 2023-10-30 17:31:38.362615 trytond_party_avatar-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      758 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:38.362615 trytond_party_avatar-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2813 2023-10-22 17:23:07.000000 trytond_party_avatar-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:07.000000 trytond_party_avatar-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:38.359281 trytond_party_avatar-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-28 12:11:23.000000 trytond_party_avatar-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      696 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:31:38.362615 trytond_party_avatar-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4570 2023-10-27 17:38:49.000000 trytond_party_avatar-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:38.359281 trytond_party_avatar-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_party_avatar-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_party_avatar-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      119 2023-10-30 17:07:27.000000 trytond_party_avatar-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:38.362615 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2544 2023-10-30 17:31:37.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2023-10-30 17:31:38.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:31:37.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-10-30 17:31:37.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:31:37.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:31:37.000000 trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:38.359281 trytond_party_avatar-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-08-13 15:26:13.000000 trytond_party_avatar-7.0.0/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-08-13 15:26:13.000000 trytond_party_avatar-7.0.0/view/employee_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-08-13 15:26:13.000000 trytond_party_avatar-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-08-13 15:26:13.000000 trytond_party_avatar-7.0.0/view/party_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:02.133587 trytond_party_avatar-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-29 15:20:57.000000 trytond_party_avatar-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:20:57.000000 trytond_party_avatar-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2535 2024-04-29 15:42:02.133587 trytond_party_avatar-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      758 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:02.130254 trytond_party_avatar-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-27 16:30:39.000000 trytond_party_avatar-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:13.000000 trytond_party_avatar-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:02.130254 trytond_party_avatar-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-27 16:43:24.000000 trytond_party_avatar-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      696 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:02.133587 trytond_party_avatar-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4561 2024-04-27 16:30:39.000000 trytond_party_avatar-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:02.130254 trytond_party_avatar-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_party_avatar-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:13.000000 trytond_party_avatar-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      119 2024-04-29 15:20:53.000000 trytond_party_avatar-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:02.133587 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2535 2024-04-29 15:42:01.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2024-04-29 15:42:02.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:01.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:42:01.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:42:01.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:01.000000 trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:02.133587 trytond_party_avatar-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-01-27 09:58:52.000000 trytond_party_avatar-7.2.0/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-01-27 09:58:52.000000 trytond_party_avatar-7.2.0/view/employee_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-01-27 09:58:52.000000 trytond_party_avatar-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-01-27 09:58:52.000000 trytond_party_avatar-7.2.0/view/party_list.xml
```

### Comparing `trytond_party_avatar-7.0.0/CHANGELOG` & `trytond_party_avatar-7.2.0/CHANGELOG`

 * *Files 25% similar despite different names*

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

### Comparing `trytond_party_avatar-7.0.0/COPYRIGHT` & `trytond_party_avatar-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_party_avatar-7.0.0/LICENSE` & `trytond_party_avatar-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party_avatar-7.0.0/PKG-INFO` & `trytond_party_avatar-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_party_avatar
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that adds avatar to parties
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-party-avatar
+Project-URL: Documentation, https://docs.tryton.org/modules-party-avatar
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party avatar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,18 +47,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_company<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_company<7.3,>=7.2; extra == "test"
 
 ###################
 Party Avatar Module
 ###################
 
 The *Party Avatar Module* adds an avatar to each party.
```

### Comparing `trytond_party_avatar-7.0.0/company.py` & `trytond_party_avatar-7.2.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_party_avatar-7.0.0/company.xml` & `trytond_party_avatar-7.2.0/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_party_avatar-7.0.0/doc/conf.py` & `trytond_party_avatar-7.2.0/doc/conf.py`

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

### Comparing `trytond_party_avatar-7.0.0/party.xml` & `trytond_party_avatar-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_party_avatar-7.0.0/setup.py` & `trytond_party_avatar-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-party-avatar'),
+            'https://docs.tryton.org/modules-party-avatar'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton party avatar',
     package_dir={'trytond.modules.party_avatar': '.'},
     packages=(
         ['trytond.modules.party_avatar']
```

### Comparing `trytond_party_avatar-7.0.0/tox.ini` & `trytond_party_avatar-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/PKG-INFO` & `trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-party-avatar
-Version: 7.0.0
+Name: trytond_party_avatar
+Version: 7.2.0
 Summary: Tryton module that adds avatar to parties
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-party-avatar
+Project-URL: Documentation, https://docs.tryton.org/modules-party-avatar
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party avatar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,18 +47,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_company<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_company<7.3,>=7.2; extra == "test"
 
 ###################
 Party Avatar Module
 ###################
 
 The *Party Avatar Module* adds an avatar to each party.
```

### Comparing `trytond_party_avatar-7.0.0/trytond_party_avatar.egg-info/SOURCES.txt` & `trytond_party_avatar-7.2.0/trytond_party_avatar.egg-info/SOURCES.txt`

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
 company.py
```

