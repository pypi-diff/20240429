# Comparing `tmp/trytond_document_incoming_ocr-7.0.1.tar.gz` & `tmp/trytond_document_incoming_ocr-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_document_incoming_ocr-7.0.1.tar", last modified: Sat Dec 16 10:05:33 2023, max compression
+gzip compressed data, was "trytond_document_incoming_ocr-7.2.0.tar", last modified: Mon Apr 29 15:40:29 2024, max compression
```

## Comparing `trytond_document_incoming_ocr-7.0.1.tar` & `trytond_document_incoming_ocr-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:33.906921 trytond_document_incoming_ocr-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      172 2023-12-16 10:05:31.000000 trytond_document_incoming_ocr-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2023-12-16 10:05:31.000000 trytond_document_incoming_ocr-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-12-16 10:05:33.906921 trytond_document_incoming_ocr-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:33.903588 trytond_document_incoming_ocr-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      701 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    18186 2023-12-10 12:43:36.000000 trytond_document_incoming_ocr-7.0.1/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4615 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/document.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:33.903588 trytond_document_incoming_ocr-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2018 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1957 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2011 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1931 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1755 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-12-16 10:05:33.906921 trytond_document_incoming_ocr-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4623 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:33.903588 trytond_document_incoming_ocr-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1443 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2023-10-30 17:55:12.000000 trytond_document_incoming_ocr-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:33.906921 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-12-16 10:05:33.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1804 2023-12-16 10:05:33.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-12-16 10:05:33.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-12-16 10:05:33.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:49.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-12-16 10:05:33.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-12-16 10:05:33.000000 trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:33.906921 trytond_document_incoming_ocr-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/view/document_incoming_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/view/document_incoming_ocr_service_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/view/document_incoming_ocr_service_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-10-30 17:06:38.000000 trytond_document_incoming_ocr-7.0.1/view/document_incoming_ocr_service_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:19:46.000000 trytond_document_incoming_ocr-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:46.000000 trytond_document_incoming_ocr-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.476010 trytond_document_incoming_ocr-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      701 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:09.000000 trytond_document_incoming_ocr-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    18186 2024-04-13 17:12:23.000000 trytond_document_incoming_ocr-7.2.0/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4523 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr-7.2.0/document.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.476010 trytond_document_incoming_ocr-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2018 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1957 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2011 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1755 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4614 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.476010 trytond_document_incoming_ocr-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1443 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:09.000000 trytond_document_incoming_ocr-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      205 2024-04-29 15:19:42.000000 trytond_document_incoming_ocr-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1786 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:56.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_list_sequence.xml
```

### Comparing `trytond_document_incoming_ocr-7.0.1/COPYRIGHT` & `trytond_document_incoming_ocr-7.2.0/COPYRIGHT`

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

### Comparing `trytond_document_incoming_ocr-7.0.1/LICENSE` & `trytond_document_incoming_ocr-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/PKG-INFO` & `trytond_document_incoming_ocr-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming_ocr
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to process incoming document with OCR
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-document-incoming-ocr
+Project-URL: Documentation, https://docs.tryton.org/modules-document-incoming-ocr
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton document incoming OCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,17 +47,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_document_incoming<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_document_incoming<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 ############################
 Document Incoming OCR Module
 ############################
 
 The *Document Incoming OCR Module* provides the basis to interact with OCR
```

### Comparing `trytond_document_incoming_ocr-7.0.1/__init__.py` & `trytond_document_incoming_ocr-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/account.py` & `trytond_document_incoming_ocr-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/doc/conf.py` & `trytond_document_incoming_ocr-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_document_incoming_ocr-7.0.1/doc/design.rst` & `trytond_document_incoming_ocr-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/document.py` & `trytond_document_incoming_ocr-7.2.0/document.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/document.xml` & `trytond_document_incoming_ocr-7.2.0/document.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_document_incoming_ocr-7.0.1/document.xml` & `trytond_document_incoming_ocr-7.2.0/document.xml`

```diff
@@ -5,17 +5,17 @@
   <data>
     <record model="ir.ui.view" id="document_incoming_view_form">
       <field name="model">document.incoming</field>
       <field name="inherit" ref="document_incoming.document_incoming_view_form"/>
       <field name="name">document_incoming_form</field>
     </record>
     <record model="ir.model.button" id="document_incoming_proceed_button">
+      <field name="model">document.incoming</field>
       <field name="name">ocr_send_feedback</field>
       <field name="string">Send Feedback</field>
-      <field name="model" search="[('model', '=', 'document.incoming')]"/>
     </record>
     <record model="ir.ui.view" id="document_incoming_ocr_service_view_form">
       <field name="model">document.incoming.ocr.service</field>
       <field name="type">form</field>
       <field name="name">document_incoming_ocr_service_form</field>
     </record>
     <record model="ir.ui.view" id="document_incoming_ocr_service_view_list">
@@ -42,30 +42,30 @@
     <record model="ir.action.act_window.view" id="act_document_incoming_ocr_service_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="document_incoming_ocr_service_view_form"/>
       <field name="act_window" ref="act_document_incoming_ocr_service_form"/>
     </record>
     <menuitem parent="document_incoming.menu_configuration" action="act_document_incoming_ocr_service_form" sequence="20" id="menu_document_incoming_ocr_service_form"/>
     <record model="ir.model.access" id="access_document_incoming_ocr_service">
-      <field name="model" search="[('model', '=', 'document.incoming.ocr.service')]"/>
+      <field name="model">document.incoming.ocr.service</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_document_incoming_ocr_service_group_document_incoming_admin">
-      <field name="model" search="[('model', '=', 'document.incoming.ocr.service')]"/>
+      <field name="model">document.incoming.ocr.service</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_document_incoming_ocr_service_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'document.incoming.ocr.service')]"/>
+      <field name="model">document.incoming.ocr.service</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_document_incoming_ocr_service_companies1">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_document_incoming_ocr_service_companies"/>
     </record>
     <record model="ir.rule" id="rule_document_incoming_ocr_service_companies2">
```

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/bg.po` & `trytond_document_incoming_ocr-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/ca.po` & `trytond_document_incoming_ocr-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/cs.po` & `trytond_document_incoming_ocr-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/de.po` & `trytond_document_incoming_ocr-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/es.po` & `trytond_document_incoming_ocr-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/es_419.po` & `trytond_document_incoming_ocr-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/et.po` & `trytond_document_incoming_ocr-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/fa.po` & `trytond_document_incoming_ocr-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/fi.po` & `trytond_document_incoming_ocr-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/fr.po` & `trytond_document_incoming_ocr-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/hu.po` & `trytond_document_incoming_ocr-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/id.po` & `trytond_document_incoming_ocr-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/it.po` & `trytond_document_incoming_ocr-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/lo.po` & `trytond_document_incoming_ocr-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/lt.po` & `trytond_document_incoming_ocr-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/nl.po` & `trytond_document_incoming_ocr-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/pl.po` & `trytond_document_incoming_ocr-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/pt.po` & `trytond_document_incoming_ocr-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/ro.po` & `trytond_document_incoming_ocr-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/ru.po` & `trytond_document_incoming_ocr-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/sl.po` & `trytond_document_incoming_ocr-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/tr.po` & `trytond_document_incoming_ocr-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/uk.po` & `trytond_document_incoming_ocr-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/locale/zh_CN.po` & `trytond_document_incoming_ocr-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/setup.py` & `trytond_document_incoming_ocr-7.2.0/setup.py`

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
-            'https://docs.tryton.org/projects/modules-document-incoming-ocr'),
+            'https://docs.tryton.org/modules-document-incoming-ocr'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton document incoming OCR',
     package_dir={'trytond.modules.document_incoming_ocr': '.'},
     packages=(
         ['trytond.modules.document_incoming_ocr']
```

### Comparing `trytond_document_incoming_ocr-7.0.1/tests/test_module.py` & `trytond_document_incoming_ocr-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/tox.ini` & `trytond_document_incoming_ocr-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/PKG-INFO` & `trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-document-incoming-ocr
-Version: 7.0.1
+Name: trytond_document_incoming_ocr
+Version: 7.2.0
 Summary: Tryton module to process incoming document with OCR
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-document-incoming-ocr
+Project-URL: Documentation, https://docs.tryton.org/modules-document-incoming-ocr
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton document incoming OCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,17 +47,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_document_incoming<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_document_incoming<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 ############################
 Document Incoming OCR Module
 ############################
 
 The *Document Incoming OCR Module* provides the basis to interact with OCR
```

### Comparing `trytond_document_incoming_ocr-7.0.1/trytond_document_incoming_ocr.egg-info/SOURCES.txt` & `trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_document_incoming_ocr-7.0.1/view/document_incoming_ocr_service_form.xml` & `trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_form.xml`

 * *Files identical despite different names*

