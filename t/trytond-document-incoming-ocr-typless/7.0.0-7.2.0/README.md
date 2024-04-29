# Comparing `tmp/trytond_document_incoming_ocr_typless-7.0.0.tar.gz` & `tmp/trytond_document_incoming_ocr_typless-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_document_incoming_ocr_typless-7.0.0.tar", last modified: Mon Oct 30 17:30:04 2023, max compression
+gzip compressed data, was "trytond_document_incoming_ocr_typless-7.2.0.tar", last modified: Mon Apr 29 15:40:35 2024, max compression
```

## Comparing `trytond_document_incoming_ocr_typless-7.0.0.tar` & `trytond_document_incoming_ocr_typless-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:04.428834 trytond_document_incoming_ocr_typless-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2023-10-30 17:06:32.000000 trytond_document_incoming_ocr_typless-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2023-10-30 17:06:32.000000 trytond_document_incoming_ocr_typless-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2965 2023-10-30 17:30:04.425500 trytond_document_incoming_ocr_typless-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:04.425500 trytond_document_incoming_ocr_typless-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2830 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2357 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11741 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/document.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      228 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:04.422167 trytond_document_incoming_ocr_typless-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      977 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      973 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      799 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 16:47:45.000000 trytond_document_incoming_ocr_typless-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:30:04.428834 trytond_document_incoming_ocr_typless-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4861 2023-10-27 17:38:49.000000 trytond_document_incoming_ocr_typless-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:04.425500 trytond_document_incoming_ocr_typless-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4013 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/tests/scenario_document_incoming_ocr_typless.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    24399 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/tests/supplier-invoice-sample.pdf
--rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_document_incoming_ocr_typless-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      193 2023-10-30 17:06:28.000000 trytond_document_incoming_ocr_typless-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:04.425500 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2965 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1831 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:04.425500 trytond_document_incoming_ocr_typless-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-10-24 07:57:53.000000 trytond_document_incoming_ocr_typless-7.0.0/view/document_incoming_ocr_service_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:19:51.000000 trytond_document_incoming_ocr_typless-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:51.000000 trytond_document_incoming_ocr_typless-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2956 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.352523 trytond_document_incoming_ocr_typless-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3092 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:10.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11741 2024-03-25 13:26:54.000000 trytond_document_incoming_ocr_typless-7.2.0/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/document.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-03-25 13:26:54.000000 trytond_document_incoming_ocr_typless-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.352523 trytond_document_incoming_ocr_typless-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      977 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      973 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      950 2024-04-29 13:17:17.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      799 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr_typless-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-03-25 13:26:54.000000 trytond_document_incoming_ocr_typless-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4852 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr_typless-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.352523 trytond_document_incoming_ocr_typless-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4017 2024-04-22 12:14:36.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/scenario_document_incoming_ocr_typless.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    24399 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/supplier-invoice-sample.pdf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:10.000000 trytond_document_incoming_ocr_typless-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      193 2024-04-29 15:19:47.000000 trytond_document_incoming_ocr_typless-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2956 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1813 2024-04-29 15:40:35.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:04.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:34.000000 trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:35.355857 trytond_document_incoming_ocr_typless-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr_typless-7.2.0/view/document_incoming_ocr_service_form.xml
```

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/COPYRIGHT` & `trytond_document_incoming_ocr_typless-7.2.0/COPYRIGHT`

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

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/LICENSE` & `trytond_document_incoming_ocr_typless-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/PKG-INFO` & `trytond_document_incoming_ocr_typless-7.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming_ocr_typless
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that integrates Typless OCR for incoming document
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-document-incoming-ocr-typless
+Project-URL: Documentation, https://docs.tryton.org/modules-document-incoming-ocr-typless
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton document incoming OCR Typless
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_document_incoming<7.1,>=7.0
-Requires-Dist: trytond_document_incoming_ocr<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_document_incoming<7.3,>=7.2
+Requires-Dist: trytond_document_incoming_ocr<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_document_incoming_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_document_incoming_invoice<7.3,>=7.2; extra == "test"
 
 ####################################
 Document Incoming OCR Typless Module
 ####################################
 
 The *Document Incoming OCR Typless Module* provides integration with `Typless
 <https://typless.com/>`_ services.
```

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/doc/conf.py` & `trytond_document_incoming_ocr_typless-7.2.0/doc/conf.py`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/doc/setup.rst` & `trytond_document_incoming_ocr_typless-7.2.0/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/document.py` & `trytond_document_incoming_ocr_typless-7.2.0/document.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/document.xml` & `trytond_document_incoming_ocr_typless-7.2.0/document.xml`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/bg.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/ca.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/cs.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/de.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/es.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/es_419.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/et.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/fa.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/fi.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/fr.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/hu.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/id.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/it.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/lo.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/lt.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/nl.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/pl.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/pt.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/ro.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/ru.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/sl.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/tr.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/locale/uk.po` & `trytond_document_incoming_ocr_typless-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/setup.py` & `trytond_document_incoming_ocr_typless-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-document-incoming-ocr-typless'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton document incoming OCR Typless',
     package_dir={'trytond.modules.document_incoming_ocr_typless': '.'},
     packages=(
```

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/tests/scenario_document_incoming_ocr_typless.rst` & `trytond_document_incoming_ocr_typless-7.2.0/tests/scenario_document_incoming_ocr_typless.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 Imports::
 
     >>> import os
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.tools import file_open
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, create_fiscalyear, get_accounts, create_tax)
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+    >>> from trytond.tools import file_open
 
 Activate modules::
 
     >>> config = activate_modules([
     ...     'document_incoming_ocr_typless',
     ...     'document_incoming_invoice'])
 
@@ -93,27 +92,25 @@
     >>> document.type = 'supplier_invoice'
     >>> document.save()
 
 Process document::
 
     >>> document.click('process')
     >>> invoice = document.result
-    >>> invoice.party == suppplier
-    True
+    >>> assertEqual(invoice.party, suppplier)
     >>> invoice.reference
     'INV-0007'
     >>> invoice.invoice_date
     datetime.date(2023, 6, 28)
     >>> invoice.payment_term_date
     datetime.date(2023, 7, 28)
     >>> len(invoice.lines)
     2
     >>> line_service, = [l for l in invoice.lines if l.product]
-    >>> line_service.product == service
-    True
+    >>> assertEqual(line_service.product, service)
     >>> line_service.quantity
     23.0
     >>> line_service.unit_price
     Decimal('2.5000')
     >>> line_goods, = [l for l in invoice.lines if not l.product]
     >>> line_goods.quantity
     40.0
@@ -121,16 +118,15 @@
     Decimal('5.0000')
     >>> len(invoice.taxes)
     2
     >>> sorted([t.amount for t in invoice.taxes])
     [Decimal('5.75'), Decimal('40.00')]
     >>> sorted([t.base for t in invoice.taxes])
     [Decimal('57.50'), Decimal('200.00')]
-    >>> {t.tax for t in invoice.taxes} == {tax_10, tax_20}
-    True
+    >>> assertEqual({t.tax for t in invoice.taxes}, {tax_10, tax_20})
     >>> invoice.untaxed_amount
     Decimal('257.50')
     >>> invoice.tax_amount
     Decimal('45.75')
     >>> invoice.total_amount
     Decimal('303.25')
```

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/tests/supplier-invoice-sample.pdf` & `trytond_document_incoming_ocr_typless-7.2.0/tests/supplier-invoice-sample.pdf`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/tests/test_module.py` & `trytond_document_incoming_ocr_typless-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/tox.ini` & `trytond_document_incoming_ocr_typless-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO` & `trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-document-incoming-ocr-typless
-Version: 7.0.0
+Name: trytond_document_incoming_ocr_typless
+Version: 7.2.0
 Summary: Tryton module that integrates Typless OCR for incoming document
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-document-incoming-ocr-typless
+Project-URL: Documentation, https://docs.tryton.org/modules-document-incoming-ocr-typless
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton document incoming OCR Typless
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_document_incoming<7.1,>=7.0
-Requires-Dist: trytond_document_incoming_ocr<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_document_incoming<7.3,>=7.2
+Requires-Dist: trytond_document_incoming_ocr<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_document_incoming_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_document_incoming_invoice<7.3,>=7.2; extra == "test"
 
 ####################################
 Document Incoming OCR Typless Module
 ####################################
 
 The *Document Incoming OCR Typless Module* provides integration with `Typless
 <https://typless.com/>`_ services.
```

### Comparing `trytond_document_incoming_ocr_typless-7.0.0/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt` & `trytond_document_incoming_ocr_typless-7.2.0/trytond_document_incoming_ocr_typless.egg-info/SOURCES.txt`

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

