# Comparing `tmp/trytond_inbound_email-7.0.0.tar.gz` & `tmp/trytond_inbound_email-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_inbound_email-7.0.0.tar", last modified: Mon Oct 30 17:30:35 2023, max compression
+gzip compressed data, was "trytond_inbound_email-7.2.0.tar", last modified: Mon Apr 29 15:41:01 2024, max compression
```

## Comparing `trytond_inbound_email-7.0.0.tar` & `trytond_inbound_email-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.152313 trytond_inbound_email-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2023-10-30 17:06:51.000000 trytond_inbound_email-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2023-10-30 17:06:50.000000 trytond_inbound_email-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-10-30 17:30:35.152313 trytond_inbound_email-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.148980 trytond_inbound_email-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.148980 trytond_inbound_email-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    10896 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/inbound_email.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7323 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/inbound_email.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.145647 trytond_inbound_email-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4770 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4645 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4803 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4821 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4660 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4191 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3761 2023-10-30 16:47:45.000000 trytond_inbound_email-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1115 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:30:35.152313 trytond_inbound_email-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2023-10-27 17:38:49.000000 trytond_inbound_email-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.145647 trytond_inbound_email-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12855 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_inbound_email-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:06:47.000000 trytond_inbound_email-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.152313 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-10-30 17:30:34.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2094 2023-10-30 17:30:35.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:34.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-10-30 17:30:34.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:34.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       26 2023-10-30 17:30:34.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:30:34.000000 trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:30:35.148980 trytond_inbound_email-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      553 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_inbox_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_inbox_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_rule_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_rule_header_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-24 07:57:53.000000 trytond_inbound_email-7.0.0/view/inbound_email_rule_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:20:12.000000 trytond_inbound_email-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:20:11.000000 trytond_inbound_email-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2453 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.771832 trytond_inbound_email-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_inbound_email-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      891 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:11.000000 trytond_inbound_email-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.771832 trytond_inbound_email-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    10913 2024-03-17 11:01:36.000000 trytond_inbound_email-7.2.0/inbound_email.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7185 2024-04-27 16:30:39.000000 trytond_inbound_email-7.2.0/inbound_email.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4370 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4243 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4401 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4423 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4257 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3749 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2024-04-29 13:17:17.000000 trytond_inbound_email-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1115 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4544 2024-04-27 16:30:39.000000 trytond_inbound_email-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12661 2024-04-27 16:30:39.000000 trytond_inbound_email-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:11.000000 trytond_inbound_email-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:20:07.000000 trytond_inbound_email-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2453 2024-04-29 15:41:01.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-29 15:41:01.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:01.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:41:01.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:30:34.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       26 2024-04-29 15:41:01.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:01.000000 trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:01.775166 trytond_inbound_email-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      553 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_inbox_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_inbox_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_rule_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_rule_header_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-02-04 18:51:26.000000 trytond_inbound_email-7.2.0/view/inbound_email_rule_list_sequence.xml
```

### Comparing `trytond_inbound_email-7.0.0/COPYRIGHT` & `trytond_inbound_email-7.2.0/COPYRIGHT`

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

### Comparing `trytond_inbound_email-7.0.0/LICENSE` & `trytond_inbound_email-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/PKG-INFO` & `trytond_inbound_email-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_inbound_email
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to manage inbound email
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-inbound-email
+Project-URL: Documentation, https://docs.tryton.org/modules-inbound-email
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton inbound email
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,15 +47,15 @@
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
 
 ####################
 Inbound Email Module
 ####################
 
 The *Inbound Email Module* defines rules to apply to inbound emails.
```

### Comparing `trytond_inbound_email-7.0.0/doc/conf.py` & `trytond_inbound_email-7.2.0/doc/conf.py`

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

### Comparing `trytond_inbound_email-7.0.0/doc/configuration.rst` & `trytond_inbound_email-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/doc/design.rst` & `trytond_inbound_email-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/doc/reference.rst` & `trytond_inbound_email-7.2.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/icons/LICENSE` & `trytond_inbound_email-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/inbound_email.py` & `trytond_inbound_email-7.2.0/inbound_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     data_id = fields.Char("Data ID", readonly=True)
     data_type = fields.Selection([
             ('mailchimp', "Mailchimp"),
             ('mailpace', "MailPace"),
             ('postmark', "Postmark"),
             ('raw', "Raw"),
             ('sendgrid', "SendGrid"),
-            ], "Data Type", required=True, readonly=True)
+            ], "Data Type", required=True, readonly=True, translate=False)
     rule = fields.Many2One('inbound.email.rule', "Rule", readonly=True)
     result = fields.Reference("Result", selection='get_models', readonly=True)
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls._order = [('id', 'DESC')]
```

### Comparing `trytond_inbound_email-7.0.0/inbound_email.xml` & `trytond_inbound_email-7.2.0/inbound_email.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_inbound_email-7.0.0/inbound_email.xml` & `trytond_inbound_email-7.2.0/inbound_email.xml`

```diff
@@ -26,28 +26,28 @@
     <record model="ir.action.act_window.view" id="act_inbound_email_inbox_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="inbound_email_inbox_view_form"/>
       <field name="act_window" ref="act_inbound_email_inbox_form"/>
     </record>
     <menuitem parent="menu_inbound_email" action="act_inbound_email_inbox_form" sequence="10" id="menu_inbound_email_inbox_form"/>
     <record model="ir.model.button" id="inbound_email_inbox_new_identifier_button">
+      <field name="model">inbound.email.inbox</field>
       <field name="name">new_identifier</field>
       <field name="string">New URL</field>
       <field name="confirm">This action will make the previous URL unusable. Do you want to continue?</field>
-      <field name="model" search="[('model', '=', 'inbound.email.inbox')]"/>
     </record>
     <record model="ir.model.access" id="access_inbound_email_inbox">
-      <field name="model" search="[('model', '=', 'inbound.email.inbox')]"/>
+      <field name="model">inbound.email.inbox</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_inbound_email_inbox_group_admin">
-      <field name="model" search="[('model', '=', 'inbound.email.inbox')]"/>
+      <field name="model">inbound.email.inbox</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="inbound_email_view_form">
@@ -77,32 +77,32 @@
     </record>
     <record model="ir.action.keyword" id="act_inbound_email_form_relate_keyword">
       <field name="keyword">form_relate</field>
       <field name="model">inbound.email.inbox,-1</field>
       <field name="action" ref="act_inbound_email_form_relate"/>
     </record>
     <record model="ir.model.access" id="access_inbound_email">
-      <field name="model" search="[('model', '=', 'inbound.email')]"/>
+      <field name="model">inbound.email</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_inbound_email_group_admin">
-      <field name="model" search="[('model', '=', 'inbound.email')]"/>
+      <field name="model">inbound.email</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.button" id="inbound_email_process_button">
+      <field name="model">inbound.email</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'inbound.email')]"/>
     </record>
     <record model="ir.ui.view" id="inbound_email_rule_view_form">
       <field name="model">inbound.email.rule</field>
       <field name="type">form</field>
       <field name="name">inbound_email_rule_form</field>
     </record>
     <record model="ir.ui.view" id="inbound_email_rule_view_list">
```

### Comparing `trytond_inbound_email-7.0.0/locale/bg.po` & `trytond_inbound_email-7.2.0/locale/bg.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/ca.po` & `trytond_inbound_email-7.2.0/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -162,27 +162,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr "Correu electrònic entrant"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr "Safata d'entrada"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr "MailPace"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr "Mailchimp"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr "Postmark"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr "En cru"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr "SendGrid"
```

### Comparing `trytond_inbound_email-7.0.0/locale/cs.po` & `trytond_inbound_email-7.2.0/locale/cs.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/de.po` & `trytond_inbound_email-7.2.0/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -158,27 +158,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr "Eingehende E-Mail"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr "Posteingang"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr "MailPace"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr "Mailchimp"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr "Postmark"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr "Rohdaten"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr "SendGrid"
```

### Comparing `trytond_inbound_email-7.0.0/locale/es.po` & `trytond_inbound_email-7.2.0/locale/nl.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,165 @@
 #
+#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:inbound.email,data:"
 msgid "Data"
-msgstr "Datos"
+msgstr "Gegevens"
 
 msgctxt "field:inbound.email,data_id:"
 msgid "Data ID"
-msgstr "ID Datos"
+msgstr "Gegevens ID"
 
 msgctxt "field:inbound.email,data_type:"
 msgid "Data Type"
-msgstr "Tipo datos"
+msgstr "Soort gegevens"
 
 msgctxt "field:inbound.email,inbox:"
 msgid "Inbox"
-msgstr "Bandeja de entrada"
+msgstr "Postvak IN"
 
 msgctxt "field:inbound.email,result:"
 msgid "Result"
-msgstr "Resultado"
+msgstr "Resultaat"
 
 msgctxt "field:inbound.email,rule:"
 msgid "Rule"
-msgstr "Regla"
+msgstr "Regel"
 
 msgctxt "field:inbound.email.inbox,endpoint:"
 msgid "Endpoint"
-msgstr "Punto final"
+msgstr "Eindpunt"
 
 msgctxt "field:inbound.email.inbox,identifier:"
 msgid "Identifier"
-msgstr "Identificador"
+msgstr "Identificatie"
 
 msgctxt "field:inbound.email.inbox,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Naam"
 
 msgctxt "field:inbound.email.inbox,rules:"
 msgid "Rules"
-msgstr "Reglas"
+msgstr "Regels"
 
 msgctxt "field:inbound.email.rule,action:"
 msgid "Action"
-msgstr "Acción"
+msgstr "Actie"
 
 msgctxt "field:inbound.email.rule,attachment_name:"
 msgid "Attachment Name"
-msgstr "Nombre del adjunto"
+msgstr "Naam bijlage"
 
 msgctxt "field:inbound.email.rule,destination:"
 msgid "Destination"
-msgstr "Destino"
+msgstr "Bestemming"
 
 msgctxt "field:inbound.email.rule,headers:"
 msgid "Headers"
-msgstr "Cabeceras"
+msgstr "Koppen"
 
 msgctxt "field:inbound.email.rule,inbox:"
 msgid "Inbox"
-msgstr "Bandeja de entrada"
+msgstr "Postvak IN"
 
 msgctxt "field:inbound.email.rule,origin:"
 msgid "Origin"
-msgstr "Origen"
+msgstr "Oorsprong"
 
 msgctxt "field:inbound.email.rule,subject:"
 msgid "Subject"
-msgstr "Asunto"
+msgstr "Onderwerp"
 
 msgctxt "field:inbound.email.rule.header,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Naam"
 
 msgctxt "field:inbound.email.rule.header,rule:"
 msgid "Rule"
-msgstr "Regla"
+msgstr "Regel"
 
 msgctxt "field:inbound.email.rule.header,value:"
 msgid "Value"
-msgstr "Valor"
+msgstr "Waarde"
 
 msgctxt "help:inbound.email.inbox,endpoint:"
 msgid "The URL where the emails must be posted."
-msgstr "La URL a la que se deben enviar los correos electrónicos."
+msgstr "De URL waar de e-mails naartoe gestuurd moeten worden."
 
 msgctxt "help:inbound.email.inbox,rules:"
 msgid "The action of the first matching line is run."
-msgstr "La acción de la primera linea coincidente se ejecutará."
+msgstr "De actie van eerst overeenkomende regel wordt uitgevoerd."
 
 msgctxt "help:inbound.email.rule,attachment_name:"
 msgid "A regular expression to match any attachment name."
-msgstr "Una expresión regular que coincida con algún nombre del adjunto."
+msgstr "Een reguliere expressie voor het vinden van passende bijlage namen."
 
 msgctxt "help:inbound.email.rule,destination:"
 msgid "A regular expression to match any receiver email addresses."
-msgstr ""
-"Una expresión regular a coincidir con algún correo electrónico del "
-"destinatario."
+msgstr "Een reguliere expressie voor het vinden van passende email adressen."
 
 msgctxt "help:inbound.email.rule,origin:"
 msgid "A regular expression to match the sender email address."
 msgstr ""
-"Una expresión regular a coincidir con elcorreo electrónico del remitente."
+"Een reguliere expressie voor het vinden van passende afzender email "
+"adressen."
 
 msgctxt "help:inbound.email.rule,subject:"
 msgid "A regular expression to match the subject."
-msgstr "Una expresión regular a coincidir con el asunto."
+msgstr "Een reguliere expressie voor het vinden van een passend onderwerp."
 
 msgctxt "help:inbound.email.rule.header,name:"
 msgid "The name of the header."
-msgstr "El nombre de la cabecera."
+msgstr "De naam van de kop."
 
 msgctxt "help:inbound.email.rule.header,value:"
 msgid "A regular expression to match the header value."
-msgstr "Una expresión regular a coincidir con el valor de la cabecera."
+msgstr "Een reguliere expressie voor het vinden van een passende kop."
 
 msgctxt "model:inbound.email,name:"
 msgid "Inbound Email"
-msgstr "Correo electrónico entrante"
+msgstr "Inkomende e-mail"
 
 msgctxt "model:inbound.email.inbox,name:"
 msgid "Inbound Email Inbox"
-msgstr "Buzón de correo electrónico entrante"
+msgstr "Inkomende e-mail postvakin"
 
 msgctxt "model:inbound.email.rule,name:"
 msgid "Inbound Email Rule"
-msgstr "Regla de correo electrónico"
+msgstr "Inkomen e-mail regel"
 
 msgctxt "model:inbound.email.rule.header,name:"
 msgid "Inbound Email Rule Header"
-msgstr "Cabeceras de las reglas de correo electrónico entrante"
+msgstr "Inkomende email regel kop"
 
 msgctxt "model:ir.action,name:act_inbound_email_form_relate"
 msgid "E-mails"
-msgstr "Correos electrónicos"
+msgstr "E-mails"
 
 msgctxt "model:ir.action,name:act_inbound_email_inbox_form"
 msgid "Inbox"
-msgstr "Bandeja de entrada"
+msgstr "Postvak IN"
 
 msgctxt ""
 "model:ir.model.button,confirm:inbound_email_inbox_new_identifier_button"
 msgid ""
 "This action will make the previous URL unusable. Do you want to continue?"
-msgstr ""
-"Esta acción provocara que la URL anterior deje de funcionar. ¿Desea "
-"continuar?"
+msgstr "Deze actie maakt de vorige URL onbruikbaar. Wilt u doorgaan?"
 
 msgctxt ""
 "model:ir.model.button,string:inbound_email_inbox_new_identifier_button"
 msgid "New URL"
-msgstr "Nueva URL"
+msgstr "Nieuwe URL"
 
 msgctxt "model:ir.model.button,string:inbound_email_process_button"
 msgid "Process"
-msgstr "Procesar"
+msgstr "Verwerken"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
-msgstr "Correo electrónico entrante"
+msgstr "Inkomende e-mail"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
-msgstr "Bandeja de entrada"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr "MailPace"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr "Mailchimp"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr "Postmark"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr "En crudo"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr "SendGrid"
+msgstr "Postvak IN"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_inbound_email-7.0.0/locale/es_419.po` & `trytond_inbound_email-7.2.0/locale/es_419.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/et.po` & `trytond_inbound_email-7.2.0/locale/et.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/fa.po` & `trytond_inbound_email-7.2.0/locale/fa.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/fi.po` & `trytond_inbound_email-7.2.0/locale/fi.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/fr.po` & `trytond_inbound_email-7.2.0/locale/fr.po`

 * *Files 5% similar despite different names*

```diff
@@ -163,27 +163,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr "E-mail entrant"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr "Boîte de réception"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr "MailPace"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr "MailChimp"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr "Postmark"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr "Brut"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr "SendGrid"
```

### Comparing `trytond_inbound_email-7.0.0/locale/hu.po` & `trytond_inbound_email-7.2.0/locale/hu.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/id.po` & `trytond_inbound_email-7.2.0/locale/id.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/it.po` & `trytond_inbound_email-7.2.0/locale/it.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/lo.po` & `trytond_inbound_email-7.2.0/locale/lo.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/lt.po` & `trytond_inbound_email-7.2.0/locale/lt.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/nl.po` & `trytond_inbound_email-7.2.0/locale/es.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,167 @@
 #
-#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:inbound.email,data:"
 msgid "Data"
-msgstr "Gegevens"
+msgstr "Datos"
 
 msgctxt "field:inbound.email,data_id:"
 msgid "Data ID"
-msgstr "Gegevens ID"
+msgstr "ID Datos"
 
 msgctxt "field:inbound.email,data_type:"
 msgid "Data Type"
-msgstr "Soort gegevens"
+msgstr "Tipo datos"
 
 msgctxt "field:inbound.email,inbox:"
 msgid "Inbox"
-msgstr "Postvak IN"
+msgstr "Bandeja de entrada"
 
 msgctxt "field:inbound.email,result:"
 msgid "Result"
-msgstr "Resultaat"
+msgstr "Resultado"
 
 msgctxt "field:inbound.email,rule:"
 msgid "Rule"
-msgstr "Regel"
+msgstr "Regla"
 
 msgctxt "field:inbound.email.inbox,endpoint:"
 msgid "Endpoint"
-msgstr "Eindpunt"
+msgstr "Punto final"
 
 msgctxt "field:inbound.email.inbox,identifier:"
 msgid "Identifier"
-msgstr "Identificatie"
+msgstr "Identificador"
 
 msgctxt "field:inbound.email.inbox,name:"
 msgid "Name"
-msgstr "Naam"
+msgstr "Nombre"
 
 msgctxt "field:inbound.email.inbox,rules:"
 msgid "Rules"
-msgstr "Regels"
+msgstr "Reglas"
 
 msgctxt "field:inbound.email.rule,action:"
 msgid "Action"
-msgstr "Actie"
+msgstr "Acción"
 
 msgctxt "field:inbound.email.rule,attachment_name:"
 msgid "Attachment Name"
-msgstr "Naam bijlage"
+msgstr "Nombre del adjunto"
 
 msgctxt "field:inbound.email.rule,destination:"
 msgid "Destination"
-msgstr "Bestemming"
+msgstr "Destino"
 
 msgctxt "field:inbound.email.rule,headers:"
 msgid "Headers"
-msgstr "Koppen"
+msgstr "Cabeceras"
 
 msgctxt "field:inbound.email.rule,inbox:"
 msgid "Inbox"
-msgstr "Postvak IN"
+msgstr "Bandeja de entrada"
 
 msgctxt "field:inbound.email.rule,origin:"
 msgid "Origin"
-msgstr "Oorsprong"
+msgstr "Origen"
 
 msgctxt "field:inbound.email.rule,subject:"
 msgid "Subject"
-msgstr "Onderwerp"
+msgstr "Asunto"
 
 msgctxt "field:inbound.email.rule.header,name:"
 msgid "Name"
-msgstr "Naam"
+msgstr "Nombre"
 
 msgctxt "field:inbound.email.rule.header,rule:"
 msgid "Rule"
-msgstr "Regel"
+msgstr "Regla"
 
 msgctxt "field:inbound.email.rule.header,value:"
 msgid "Value"
-msgstr "Waarde"
+msgstr "Valor"
 
 msgctxt "help:inbound.email.inbox,endpoint:"
 msgid "The URL where the emails must be posted."
-msgstr "De URL waar de e-mails naartoe gestuurd moeten worden."
+msgstr "La URL a la que se deben enviar los correos electrónicos."
 
 msgctxt "help:inbound.email.inbox,rules:"
 msgid "The action of the first matching line is run."
-msgstr "De actie van eerst overeenkomende regel wordt uitgevoerd."
+msgstr "La acción de la primera linea coincidente se ejecutará."
 
 msgctxt "help:inbound.email.rule,attachment_name:"
 msgid "A regular expression to match any attachment name."
-msgstr "Een reguliere expressie voor het vinden van passende bijlage namen."
+msgstr "Una expresión regular que coincida con algún nombre del adjunto."
 
 msgctxt "help:inbound.email.rule,destination:"
 msgid "A regular expression to match any receiver email addresses."
-msgstr "Een reguliere expressie voor het vinden van passende email adressen."
+msgstr ""
+"Una expresión regular a coincidir con algún correo electrónico del "
+"destinatario."
 
 msgctxt "help:inbound.email.rule,origin:"
 msgid "A regular expression to match the sender email address."
 msgstr ""
-"Een reguliere expressie voor het vinden van passende afzender email "
-"adressen."
+"Una expresión regular a coincidir con elcorreo electrónico del remitente."
 
 msgctxt "help:inbound.email.rule,subject:"
 msgid "A regular expression to match the subject."
-msgstr "Een reguliere expressie voor het vinden van een passend onderwerp."
+msgstr "Una expresión regular a coincidir con el asunto."
 
 msgctxt "help:inbound.email.rule.header,name:"
 msgid "The name of the header."
-msgstr "De naam van de kop."
+msgstr "El nombre de la cabecera."
 
 msgctxt "help:inbound.email.rule.header,value:"
 msgid "A regular expression to match the header value."
-msgstr "Een reguliere expressie voor het vinden van een passende kop."
+msgstr "Una expresión regular a coincidir con el valor de la cabecera."
 
 msgctxt "model:inbound.email,name:"
 msgid "Inbound Email"
-msgstr "Inkomende e-mail"
+msgstr "Correo electrónico entrante"
 
 msgctxt "model:inbound.email.inbox,name:"
 msgid "Inbound Email Inbox"
-msgstr "Inkomende e-mail postvakin"
+msgstr "Buzón de correo electrónico entrante"
 
 msgctxt "model:inbound.email.rule,name:"
 msgid "Inbound Email Rule"
-msgstr "Inkomen e-mail regel"
+msgstr "Regla de correo electrónico"
 
 msgctxt "model:inbound.email.rule.header,name:"
 msgid "Inbound Email Rule Header"
-msgstr "Inkomende email regel kop"
+msgstr "Cabeceras de las reglas de correo electrónico entrante"
 
 msgctxt "model:ir.action,name:act_inbound_email_form_relate"
 msgid "E-mails"
-msgstr "E-mails"
+msgstr "Correos electrónicos"
 
 msgctxt "model:ir.action,name:act_inbound_email_inbox_form"
 msgid "Inbox"
-msgstr "Postvak IN"
+msgstr "Bandeja de entrada"
 
 msgctxt ""
 "model:ir.model.button,confirm:inbound_email_inbox_new_identifier_button"
 msgid ""
 "This action will make the previous URL unusable. Do you want to continue?"
-msgstr "Deze actie maakt de vorige URL onbruikbaar. Wilt u doorgaan?"
+msgstr ""
+"Esta acción provocara que la URL anterior deje de funcionar. ¿Desea "
+"continuar?"
 
 msgctxt ""
 "model:ir.model.button,string:inbound_email_inbox_new_identifier_button"
 msgid "New URL"
-msgstr "Nieuwe URL"
+msgstr "Nueva URL"
 
 msgctxt "model:ir.model.button,string:inbound_email_process_button"
 msgid "Process"
-msgstr "Verwerken"
+msgstr "Procesar"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
-msgstr "Inkomende e-mail"
+msgstr "Correo electrónico entrante"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
-msgstr "Postvak IN"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr "MailPace"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr "Mailchimp"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr "Postmark"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr "Ruwe data"
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr "SendGrid"
+msgstr "Bandeja de entrada"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_inbound_email-7.0.0/locale/pl.po` & `trytond_inbound_email-7.2.0/locale/pl.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/pt.po` & `trytond_inbound_email-7.2.0/locale/pt.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/ro.po` & `trytond_inbound_email-7.2.0/locale/ro.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/ru.po` & `trytond_inbound_email-7.2.0/locale/ru.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/sl.po` & `trytond_inbound_email-7.2.0/locale/sl.po`

 * *Files 7% similar despite different names*

```diff
@@ -157,32 +157,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr "Vhodna e-pošta"
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr "Prejeto"
-
-#, fuzzy
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr "MailPace"
-
-#, fuzzy
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr "Mailchimp"
-
-#, fuzzy
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr "Postmark"
-
-#, fuzzy
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr "Raw"
-
-#, fuzzy
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr "SendGrid"
```

### Comparing `trytond_inbound_email-7.0.0/locale/tr.po` & `trytond_inbound_email-7.2.0/locale/tr.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/uk.po` & `trytond_inbound_email-7.2.0/locale/uk.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/locale/zh_CN.po` & `trytond_inbound_email-7.2.0/locale/zh_CN.po`

 * *Files 3% similar despite different names*

```diff
@@ -156,27 +156,7 @@
 msgctxt "model:ir.ui.menu,name:menu_inbound_email"
 msgid "Inbound Email"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_inbound_email_inbox_form"
 msgid "Inbox"
 msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "MailPace"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Mailchimp"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Postmark"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "Raw"
-msgstr ""
-
-msgctxt "selection:inbound.email,data_type:"
-msgid "SendGrid"
-msgstr ""
```

### Comparing `trytond_inbound_email-7.0.0/routes.py` & `trytond_inbound_email-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/setup.py` & `trytond_inbound_email-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-inbound-email'),
+            'https://docs.tryton.org/modules-inbound-email'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton inbound email',
     package_dir={'trytond.modules.inbound_email': '.'},
     packages=(
         ['trytond.modules.inbound_email']
```

### Comparing `trytond_inbound_email-7.0.0/tests/test_module.py` & `trytond_inbound_email-7.2.0/tests/test_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import json
 import uuid
-from email.mime.application import MIMEApplication
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
+from email.message import EmailMessage
 from unittest.mock import patch
 
 from trytond.pool import Pool
 from trytond.protocols.wrappers import HTTPStatus
 from trytond.tests.test_tryton import (
     ModuleTestCase, RouteTestCase, with_transaction)
 from trytond.transaction import Transaction
 
 
 class InboundEmailTestCase(ModuleTestCase):
     "Test Inbound Email module"
     module = 'inbound_email'
 
     def get_message(self):
-        message = MIMEMultipart('mixed')
+        message = EmailMessage()
         message['From'] = "John Doe <john.doe@example.com>"
         message['To'] = (
             "Michael Scott <michael@example.com>, pam@example.com")
         message['Cc'] = 'jim@example.com'
         message['Subject'] = "The office"
 
-        text = MIMEText("Hello", 'plain')
-        message.attach(text)
-        attachment = MIMEApplication(b'bin')
-        attachment.add_header(
-            'Content-Disposition', 'attachment',
+        message.set_content("Hello")
+        message.add_attachment(
+            b'bin', maintype='application', subtype='octet-stream',
             filename='data.bin')
-        message.attach(attachment)
         return message
 
     def get_message_dict(self, headers):
         return {
             'from': 'john.doe@example.com',
             'to': ['michael@example.com', 'pam@example.com'],
             'cc': ['jim@example.com'],
             'subject': 'The office',
-            'text': 'Hello',
+            'text': 'Hello\n',
             'attachments': [{
                     'filename': 'data.bin',
                     'type': 'application/octet-stream',
                     'data': b'bin',
                     }],
             'headers': dict(headers.items()),
             }
@@ -165,15 +160,15 @@
                         'Email': 'pam@example.com',
                         },
                     ],
                 'CcFull': [{
                         'Email': 'jim@example.com',
                         }],
                 'Subject': 'The office',
-                'TextBody': 'Hello',
+                'TextBody': 'Hello\n',
                 'Attachments': [{
                         'Name': 'data.bin',
                         'Content': 'Ymlu',
                         'ContentType': 'application/octet-stream',
                         }],
                 'Headers': [{
                         'Name': 'Message-ID',
```

### Comparing `trytond_inbound_email-7.0.0/tox.ini` & `trytond_inbound_email-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/PKG-INFO` & `trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-inbound-email
-Version: 7.0.0
+Name: trytond_inbound_email
+Version: 7.2.0
 Summary: Tryton module to manage inbound email
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-inbound-email
+Project-URL: Documentation, https://docs.tryton.org/modules-inbound-email
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton inbound email
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,15 +47,15 @@
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
 
 ####################
 Inbound Email Module
 ####################
 
 The *Inbound Email Module* defines rules to apply to inbound emails.
```

### Comparing `trytond_inbound_email-7.0.0/trytond_inbound_email.egg-info/SOURCES.txt` & `trytond_inbound_email-7.2.0/trytond_inbound_email.egg-info/SOURCES.txt`

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
 inbound_email.py
```

### Comparing `trytond_inbound_email-7.0.0/view/inbound_email_form.xml` & `trytond_inbound_email-7.2.0/view/inbound_email_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_inbound_email-7.0.0/view/inbound_email_rule_form.xml` & `trytond_inbound_email-7.2.0/view/inbound_email_rule_form.xml`

 * *Files identical despite different names*

