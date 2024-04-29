# Comparing `tmp/trytond_document_incoming-7.0.0.tar.gz` & `tmp/trytond_document_incoming-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_document_incoming-7.0.0.tar", last modified: Mon Oct 30 17:29:43 2023, max compression
+gzip compressed data, was "trytond_document_incoming-7.2.0.tar", last modified: Mon Apr 29 15:40:16 2024, max compression
```

## Comparing `trytond_document_incoming-7.0.0.tar` & `trytond_document_incoming-7.2.0.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.642068 trytond_document_incoming-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2023-10-30 17:06:19.000000 trytond_document_incoming-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2023-10-30 17:06:18.000000 trytond_document_incoming-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2672 2023-10-30 17:29:43.642068 trytond_document_incoming-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.638734 trytond_document_incoming-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1682 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11747 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11016 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/document.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.638734 trytond_document_incoming-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      653 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/icons/tryton-document-incoming-split.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/icons/tryton-document-incoming.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1911 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/inbound_email.py
--rw-r--r--   0 ced       (1000) ced       (1000)      532 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/inbound_email.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.635401 trytond_document_incoming-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5262 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5270 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5283 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5246 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5225 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5151 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_document_incoming-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1416 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:29:43.642068 trytond_document_incoming-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4695 2023-10-27 17:38:49.000000 trytond_document_incoming-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.638734 trytond_document_incoming-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1829 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/tests/mutipage.pdf
--rw-r--r--   0 ced       (1000) ced       (1000)      875 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/tests/scenario_document_incoming.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/tests/scenario_document_incoming_split.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7107 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_document_incoming-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-30 17:06:15.000000 trytond_document_incoming-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.642068 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2672 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2412 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      111 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:29:43.000000 trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:43.638734 trytond_document_incoming-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/view/document_incoming_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/view/document_incoming_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/view/document_incoming_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/view/document_incoming_split_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      553 2023-10-24 07:57:53.000000 trytond_document_incoming-7.0.0/view/inbound_email_rule_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.439685 trytond_document_incoming-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:19:36.000000 trytond_document_incoming-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:36.000000 trytond_document_incoming-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2663 2024-04-29 15:40:16.436351 trytond_document_incoming-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      710 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.433018 trytond_document_incoming-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_document_incoming-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1682 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      891 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:09.000000 trytond_document_incoming-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11747 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10763 2024-04-27 16:30:39.000000 trytond_document_incoming-7.2.0/document.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.433018 trytond_document_incoming-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/icons/tryton-document-incoming-split.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/icons/tryton-document-incoming.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1911 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/inbound_email.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      532 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/inbound_email.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.436351 trytond_document_incoming-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5262 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5270 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5283 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5246 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5225 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5151 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:24.000000 trytond_document_incoming-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1416 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:16.439685 trytond_document_incoming-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4686 2024-04-27 16:30:39.000000 trytond_document_incoming-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.436351 trytond_document_incoming-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1829 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/tests/mutipage.pdf
+-rw-r--r--   0 ced       (1000) ced       (1000)      890 2024-04-22 12:14:36.000000 trytond_document_incoming-7.2.0/tests/scenario_document_incoming.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/tests/scenario_document_incoming_split.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7107 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:09.000000 trytond_document_incoming-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-29 15:19:32.000000 trytond_document_incoming-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.436351 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2663 2024-04-29 15:40:15.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2394 2024-04-29 15:40:16.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:15.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:40:15.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:43.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      111 2024-04-29 15:40:15.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:15.000000 trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:16.436351 trytond_document_incoming-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/view/document_incoming_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/view/document_incoming_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/view/document_incoming_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/view/document_incoming_split_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      553 2024-02-04 18:51:26.000000 trytond_document_incoming-7.2.0/view/inbound_email_rule_form.xml
```

### Comparing `trytond_document_incoming-7.0.0/COPYRIGHT` & `trytond_document_incoming-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2023 B2CK
-Copyright (C) 2023 Cédric Krier
+Copyright (C) 2023-2024 B2CK
+Copyright (C) 2023-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_document_incoming-7.0.0/LICENSE` & `trytond_document_incoming-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/PKG-INFO` & `trytond_document_incoming-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to manage incoming document
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-document-incoming
+Project-URL: Documentation, https://docs.tryton.org/modules-document-incoming
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton document incoming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pypdf>=3
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_inbound_email<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_inbound_email<7.3,>=7.2; extra == "test"
 
 ########################
 Document Incoming Module
 ########################
 
 The *Document Incoming Module* collects and process incoming documents.
```

### Comparing `trytond_document_incoming-7.0.0/__init__.py` & `trytond_document_incoming-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/doc/conf.py` & `trytond_document_incoming-7.2.0/doc/conf.py`

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

### Comparing `trytond_document_incoming-7.0.0/doc/configuration.rst` & `trytond_document_incoming-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/doc/design.rst` & `trytond_document_incoming-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/doc/reference.rst` & `trytond_document_incoming-7.2.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/doc/usage.rst` & `trytond_document_incoming-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/document.py` & `trytond_document_incoming-7.2.0/document.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/document.xml` & `trytond_document_incoming-7.2.0/document.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_document_incoming-7.0.0/document.xml` & `trytond_document_incoming-7.2.0/document.xml`

```diff
@@ -48,22 +48,22 @@
     <record model="ir.action.act_window.view" id="act_document_incoming_configuration_form_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="document_incoming_configuration_view_form"/>
       <field name="act_window" ref="act_document_incoming_configuration_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_document_incoming_configuration_form" sequence="10" id="menu_ocument_incoming_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_document_incoming_configuration">
-      <field name="model" search="[('model', '=', 'document.incoming.configuration')]"/>
+      <field name="model">document.incoming.configuration</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_document_incoming_configuration_group_document_incoming_admin">
-      <field name="model" search="[('model', '=', 'document.incoming.configuration')]"/>
+      <field name="model">document.incoming.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="document_incoming_view_form">
       <field name="model">document.incoming</field>
@@ -111,70 +111,70 @@
     </record>
     <menuitem parent="menu_document" action="act_document_incoming_form" sequence="10" id="menu_document_incoming"/>
     <record model="ir.ui.menu-res.group" id="menu_document_incoming_group_document_incoming">
       <field name="menu" ref="menu_document_incoming"/>
       <field name="group" ref="group_document_incoming"/>
     </record>
     <record model="ir.model.access" id="access_document_incoming">
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
+      <field name="model">document.incoming</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_document_incoming_group_document_incoming">
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
+      <field name="model">document.incoming</field>
       <field name="group" ref="group_document_incoming"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_document_incoming_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
+      <field name="model">document.incoming</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_document_incoming_companies1">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_document_incoming_companies"/>
     </record>
     <record model="ir.rule" id="rule_document_incoming_companies2">
       <field name="domain" eval="[('company', '=', None)]" pyson="1"/>
       <field name="rule_group" ref="rule_group_document_incoming_companies"/>
     </record>
     <record model="ir.model.button" id="document_incoming_cancel_button">
+      <field name="model">document.incoming</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.model.button" id="document_incoming_draft_button">
+      <field name="model">document.incoming</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.model.button" id="document_incoming_split_wizard_button">
+      <field name="model">document.incoming</field>
       <field name="name">split_wizard</field>
       <field name="string">Split</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.model.button" id="document_incoming_extract_email_button">
+      <field name="model">document.incoming</field>
       <field name="name">extract_email</field>
       <field name="string">Extract Email</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.model.button" id="document_incoming_process_button">
+      <field name="model">document.incoming</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.model.button" id="document_incoming_proceed_button">
+      <field name="model">document.incoming</field>
       <field name="name">proceed</field>
       <field name="string">Proceed</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_document_incoming_split">
       <field name="name">Split Incoming Document</field>
       <field name="wiz_name">document.incoming.split</field>
       <field name="model">document.incoming</field>
     </record>
     <record model="ir.ui.view" id="document_incoming_split_start_view_form">
```

### Comparing `trytond_document_incoming-7.0.0/icons/LICENSE` & `trytond_document_incoming-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/icons/tryton-document-incoming-split.svg` & `trytond_document_incoming-7.2.0/icons/tryton-document-incoming-split.svg`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/inbound_email.py` & `trytond_document_incoming-7.2.0/inbound_email.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/inbound_email.xml` & `trytond_document_incoming-7.2.0/inbound_email.xml`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/bg.po` & `trytond_document_incoming-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/ca.po` & `trytond_document_incoming-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/cs.po` & `trytond_document_incoming-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/de.po` & `trytond_document_incoming-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/es.po` & `trytond_document_incoming-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/es_419.po` & `trytond_document_incoming-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/et.po` & `trytond_document_incoming-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/fa.po` & `trytond_document_incoming-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/fi.po` & `trytond_document_incoming-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/fr.po` & `trytond_document_incoming-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/hu.po` & `trytond_document_incoming-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/id.po` & `trytond_document_incoming-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/it.po` & `trytond_document_incoming-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/lo.po` & `trytond_document_incoming-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/lt.po` & `trytond_document_incoming-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/nl.po` & `trytond_document_incoming-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/pl.po` & `trytond_document_incoming-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/pt.po` & `trytond_document_incoming-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/ro.po` & `trytond_document_incoming-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/ru.po` & `trytond_document_incoming-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/sl.po` & `trytond_document_incoming-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/tr.po` & `trytond_document_incoming-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/uk.po` & `trytond_document_incoming-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/locale/zh_CN.po` & `trytond_document_incoming-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/routes.py` & `trytond_document_incoming-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/setup.py` & `trytond_document_incoming-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-document-incoming'),
+            'https://docs.tryton.org/modules-document-incoming'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton document incoming',
     package_dir={'trytond.modules.document_incoming': '.'},
     packages=(
         ['trytond.modules.document_incoming']
```

### Comparing `trytond_document_incoming-7.0.0/tests/mutipage.pdf` & `trytond_document_incoming-7.2.0/tests/mutipage.pdf`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/tests/scenario_document_incoming.rst` & `trytond_document_incoming-7.2.0/tests/scenario_document_incoming.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ==========================
 Document Incoming Scenario
 ==========================
 
 Imports::
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.tests.tools import activate_modules, assertEqual
     >>> from trytond.tools import file_open
 
 Activate modules::
 
     >>> config = activate_modules('document_incoming')
 
     >>> Document = Model.get('document.incoming')
@@ -27,10 +27,9 @@
 
 Process document::
 
     >>> document.click('process')
     >>> document.state
     'done'
     >>> new_document = document.result
-    >>> new_document.data == document.data
-    True
+    >>> assertEqual(new_document.data, document.data)
     >>> new_document.type
```

### Comparing `trytond_document_incoming-7.0.0/tests/scenario_document_incoming_split.rst` & `trytond_document_incoming-7.2.0/tests/scenario_document_incoming_split.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/tests/test_module.py` & `trytond_document_incoming-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/tox.ini` & `trytond_document_incoming-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/PKG-INFO` & `trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-document-incoming
-Version: 7.0.0
+Name: trytond_document_incoming
+Version: 7.2.0
 Summary: Tryton module to manage incoming document
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-document-incoming
+Project-URL: Documentation, https://docs.tryton.org/modules-document-incoming
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton document incoming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pypdf>=3
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_inbound_email<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_inbound_email<7.3,>=7.2; extra == "test"
 
 ########################
 Document Incoming Module
 ########################
 
 The *Document Incoming Module* collects and process incoming documents.
```

### Comparing `trytond_document_incoming-7.0.0/trytond_document_incoming.egg-info/SOURCES.txt` & `trytond_document_incoming-7.2.0/trytond_document_incoming.egg-info/SOURCES.txt`

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
 document.py
```

### Comparing `trytond_document_incoming-7.0.0/view/document_incoming_form.xml` & `trytond_document_incoming-7.2.0/view/document_incoming_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/view/document_incoming_list.xml` & `trytond_document_incoming-7.2.0/view/document_incoming_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming-7.0.0/view/inbound_email_rule_form.xml` & `trytond_document_incoming-7.2.0/view/inbound_email_rule_form.xml`

 * *Files identical despite different names*

