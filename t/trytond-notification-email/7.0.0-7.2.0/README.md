# Comparing `tmp/trytond_notification_email-7.0.0.tar.gz` & `tmp/trytond_notification_email-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_notification_email-7.0.0.tar", last modified: Mon Oct 30 17:31:22 2023, max compression
+gzip compressed data, was "trytond_notification_email-7.2.0.tar", last modified: Mon Apr 29 15:41:47 2024, max compression
```

## Comparing `trytond_notification_email-7.0.0.tar` & `trytond_notification_email-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:22.665873 trytond_notification_email-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-22 17:23:06.000000 trytond_notification_email-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1589 2023-10-30 17:07:22.000000 trytond_notification_email-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-10-30 17:07:22.000000 trytond_notification_email-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_notification_email-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2928 2023-10-30 17:31:22.665873 trytond_notification_email-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-08-13 15:26:13.000000 trytond_notification_email-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:22.662540 trytond_notification_email-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-22 17:23:06.000000 trytond_notification_email-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:06.000000 trytond_notification_email-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-10-07 15:40:36.000000 trytond_notification_email-7.0.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1961 2023-08-13 15:26:13.000000 trytond_notification_email-7.0.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:22.659207 trytond_notification_email-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5948 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5835 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5986 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4218 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4636 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5737 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5735 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4404 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5669 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5565 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5576 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5372 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5654 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5627 2023-10-30 16:47:45.000000 trytond_notification_email-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4218 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5197 2023-10-28 12:11:23.000000 trytond_notification_email-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14218 2023-10-07 15:40:36.000000 trytond_notification_email-7.0.0/notification.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-08-13 15:26:13.000000 trytond_notification_email-7.0.0/notification.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:31:22.665873 trytond_notification_email-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4505 2023-10-27 17:38:49.000000 trytond_notification_email-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:22.662540 trytond_notification_email-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15692 2023-08-13 15:26:13.000000 trytond_notification_email-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_notification_email-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-10-30 17:07:18.000000 trytond_notification_email-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:22.662540 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2928 2023-10-30 17:31:22.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-10-30 17:31:22.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:31:22.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-10-30 17:31:22.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-10-30 17:31:22.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:31:22.000000 trytond_notification_email-7.0.0/trytond_notification_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:22.662540 trytond_notification_email-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1080 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_notification_email-7.0.0/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-08-13 15:26:13.000000 trytond_notification_email-7.0.0/view/ir_email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:20.000000 trytond_notification_email-7.0.0/view/trigger_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1690 2024-04-29 15:20:47.000000 trytond_notification_email-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:20:47.000000 trytond_notification_email-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_notification_email-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2928 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-01-27 09:58:52.000000 trytond_notification_email-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:47.533969 trytond_notification_email-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_notification_email-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:12.000000 trytond_notification_email-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2024-02-04 18:51:26.000000 trytond_notification_email-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1961 2024-01-27 09:58:52.000000 trytond_notification_email-7.2.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5948 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5835 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5986 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4218 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4636 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5737 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5735 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4404 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5669 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5565 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5576 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5372 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5643 2024-04-29 13:17:17.000000 trytond_notification_email-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5627 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4218 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5197 2024-04-27 16:43:24.000000 trytond_notification_email-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13346 2024-04-27 16:30:39.000000 trytond_notification_email-7.2.0/notification.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2324 2024-04-27 16:30:39.000000 trytond_notification_email-7.2.0/notification.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4505 2024-03-17 11:01:36.000000 trytond_notification_email-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15208 2024-04-27 16:30:39.000000 trytond_notification_email-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:12.000000 trytond_notification_email-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2024-04-29 15:20:43.000000 trytond_notification_email-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2928 2024-04-29 15:41:47.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2024-04-29 15:41:47.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:47.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:41:47.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2024-04-29 15:41:47.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:47.000000 trytond_notification_email-7.2.0/trytond_notification_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:47.537302 trytond_notification_email-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1080 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_notification_email-7.2.0/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-01-27 09:58:52.000000 trytond_notification_email-7.2.0/view/ir_email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:20.000000 trytond_notification_email-7.2.0/view/trigger_form.xml
```

### Comparing `trytond_notification_email-7.0.0/CHANGELOG` & `trytond_notification_email-7.2.0/CHANGELOG`

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

### Comparing `trytond_notification_email-7.0.0/COPYRIGHT` & `trytond_notification_email-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2016-2022 Sergi Almacellas Abellana
-Copyright (C) 2017-2023 Cédric Krier
-Copyright (C) 2017-2023 B2CK
+Copyright (C) 2017-2024 Cédric Krier
+Copyright (C) 2017-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_notification_email-7.0.0/LICENSE` & `trytond_notification_email-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/PKG-INFO` & `trytond_notification_email-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_notification_email
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for sending email notifications
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
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
 Requires-Dist: python-sql
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_company<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_commission<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_party<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_web_user<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_company<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_commission<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_party<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_web_user<7.3,>=7.2; extra == "test"
 
 Notification Email Module
 #########################
 
 The notification email module allows to define email templates which will be
 sent to a list of recipients when a trigger is fired on a record event.
 Extra reports from the same record can be attached to the email.
```

### Comparing `trytond_notification_email-7.0.0/doc/conf.py` & `trytond_notification_email-7.2.0/doc/conf.py`

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

### Comparing `trytond_notification_email-7.0.0/ir.py` & `trytond_notification_email-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/ir.xml` & `trytond_notification_email-7.2.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/bg.po` & `trytond_notification_email-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/ca.po` & `trytond_notification_email-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/cs.po` & `trytond_notification_email-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/de.po` & `trytond_notification_email-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/es.po` & `trytond_notification_email-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/es_419.po` & `trytond_notification_email-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/et.po` & `trytond_notification_email-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/fa.po` & `trytond_notification_email-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/fi.po` & `trytond_notification_email-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/fr.po` & `trytond_notification_email-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/hu.po` & `trytond_notification_email-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/id.po` & `trytond_notification_email-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/it.po` & `trytond_notification_email-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/lo.po` & `trytond_notification_email-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/lt.po` & `trytond_notification_email-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/nl.po` & `trytond_notification_email-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/pl.po` & `trytond_notification_email-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/pt.po` & `trytond_notification_email-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/ro.po` & `trytond_notification_email-7.2.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 "Se aplică dacă este activată o coadă de lucrători."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
-"Sintaxa Genshi poate fi folosită cu „înregistrare” în contextul evaluării.\n"
+"Sintaxa Genshi poate fi folosită cu 'record' în contextul evaluării.\n"
 "Dacă este gol, va fi folosit numele raportului."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
 msgstr "Adăugați un declanșator pentru notificare."
 
 msgctxt "model:ir.action,name:act_email_form"
```

### Comparing `trytond_notification_email-7.0.0/locale/ru.po` & `trytond_notification_email-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/sl.po` & `trytond_notification_email-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/tr.po` & `trytond_notification_email-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/uk.po` & `trytond_notification_email-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/locale/zh_CN.po` & `trytond_notification_email-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/notification.py` & `trytond_notification_email-7.2.0/notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import mimetypes
-from email.encoders import encode_base64
-from email.header import Header
-from email.mime.application import MIMEApplication
-from email.mime.multipart import MIMEMultipart
-from email.mime.nonmultipart import MIMENonMultipart
-from email.utils import formataddr, getaddresses
+from email.utils import getaddresses
 
 from genshi.template import TextTemplate
 
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, ModelView, fields
 from trytond.pool import Pool
 from trytond.pyson import Eval, TimeDelta
 from trytond.report import get_email
-from trytond.sendmail import SMTPDataManager, sendmail_transactional
-from trytond.tools.email_ import convert_ascii_email, set_from_header
+from trytond.sendmail import SMTPDataManager, send_message_transactional
+from trytond.tools.email_ import format_address, has_rcpt, set_from_header
 from trytond.transaction import Transaction
 
 from .exceptions import TemplateError
 
 
 class Email(ModelSQL, ModelView):
     "Email Notification"
@@ -34,45 +29,45 @@
         "Subject", translate=True,
         help="The Genshi syntax can be used "
         "with 'record' in the evaluation context.\n"
         "If empty the report name will be used.")
     recipients = fields.Many2One(
         'ir.model.field', "Recipients",
         domain=[
-            ('model.model', '=', Eval('model')),
+            ('model', '=', Eval('model')),
             ],
         help="The field that contains the recipient(s).")
     fallback_recipients = fields.Many2One(
         'res.user', "Recipients Fallback User",
         domain=[
             ('email', '!=', None),
             ],
         states={
             'invisible': ~Eval('recipients'),
             },
         help="User notified when no recipients e-mail is found")
     recipients_secondary = fields.Many2One(
         'ir.model.field', "Secondary Recipients",
         domain=[
-            ('model.model', '=', Eval('model')),
+            ('model', '=', Eval('model')),
             ],
         help="The field that contains the secondary recipient(s).")
     fallback_recipients_secondary = fields.Many2One(
         'res.user', "Secondary Recipients Fallback User",
         domain=[
             ('email', '!=', None),
             ],
         states={
             'invisible': ~Eval('recipients_secondary'),
             },
         help="User notified when no secondary recipients e-mail is found")
     recipients_hidden = fields.Many2One(
         'ir.model.field', "Hidden Recipients",
         domain=[
-            ('model.model', '=', Eval('model')),
+            ('model', '=', Eval('model')),
             ],
         help="The field that contains the hidden recipient(s).")
     fallback_recipients_hidden = fields.Many2One(
         'res.user', "Hidden Recipients Fallback User",
         domain=[
             ('email', '!=', None),
             ],
@@ -157,57 +152,65 @@
     def search_model(cls, name, clause):
         return [('content.model',) + tuple(clause[1:])]
 
     def _get_addresses(self, value):
         pool = Pool()
         EmailTemplate = pool.get('ir.email.template')
         with Transaction().set_context(usage=self.contact_mechanism):
-            return EmailTemplate.get_addresses(value)
+            # reformat addresses with encoding
+            return [
+                format_address(e, n)
+                for n, e in getaddresses(EmailTemplate.get_addresses(value))]
 
     def _get_languages(self, value):
         pool = Pool()
         EmailTemplate = pool.get('ir.email.template')
         with Transaction().set_context(usage=self.contact_mechanism):
             return EmailTemplate.get_languages(value)
 
     def get_email(self, record, sender, to, cc, bcc, languages):
         pool = Pool()
         Attachment = pool.get('notification.email.attachment')
 
         # TODO order languages to get default as last one for title
-        content, title = get_email(self.content, record, languages)
-        language = list(languages)[-1]
+        msg, title = get_email(self.content, record, languages)
+        if languages:
+            language = list(languages)[-1].code
+        else:
+            language = None
         from_ = sender
-        with Transaction().set_context(language=language.code):
+        with Transaction().set_context(language=language):
             notification = self.__class__(self.id)
             if notification.from_:
                 from_ = notification.from_
             if self.subject:
                 title = (TextTemplate(notification.subject)
                     .generate(record=record)
                     .render())
 
         if self.attachments:
-            msg = MIMEMultipart('mixed')
-            msg.attach(content)
             for report in self.attachments:
-                msg.attach(Attachment.get_mime(report, record, language.code))
-        else:
-            msg = content
+                name, data = Attachment.get(report, record, language)
+                ctype, _ = mimetypes.guess_type(name)
+                if not ctype:
+                    ctype = 'application/octet-stream'
+                maintype, subtype = ctype.split('/', 1)
+                msg.add_attachment(
+                    data,
+                    maintype=maintype,
+                    subtype=subtype,
+                    filename=('utf-8', '', name))
 
         set_from_header(msg, sender, from_)
-        msg['To'] = ', '.join(
-            formataddr((n, convert_ascii_email(a)))
-            for n, a in getaddresses(to))
-        msg['Cc'] = ', '.join(
-            formataddr((n, convert_ascii_email(a)))
-            for n, a in getaddresses(cc))
-        msg['Subject'] = Header(title, 'utf-8')
+        msg['To'] = to
+        msg['Cc'] = cc
+        msg['Bcc'] = bcc
+        msg['Subject'] = title
         msg['Auto-Submitted'] = 'auto-generated'
-        return msg, title
+        return msg
 
     @classmethod
     def trigger(cls, records, trigger):
         "Action function for the triggers"
         notification_email = trigger.notification_email
         if not notification_email:
             raise ValueError(
@@ -238,28 +241,19 @@
             or config.get('email', 'from'))
         emails = []
         for record in records:
             to, to_languages = self._get_to(record)
             cc, cc_languages = self._get_cc(record)
             bcc, bcc_languages = self._get_bcc(record)
             languages = to_languages | cc_languages | bcc_languages
-            to_addrs = [
-                convert_ascii_email(e) for _, e in getaddresses(to + cc + bcc)]
-            if to_addrs:
-                msg, title = self.get_email(
-                    record, from_, to, cc, bcc, languages)
-                sendmail_transactional(
-                    from_, to_addrs, msg, datamanager=datamanager)
-                emails.append(Email(
-                        recipients=', '.join(to),
-                        recipients_secondary=', '.join(cc),
-                        recipients_hidden=', '.join(bcc),
-                        addresses=[{'address': a} for a in to_addrs],
-                        subject=title,
-                        resource=record,
+            msg = self.get_email(record, from_, to, cc, bcc, languages)
+            if has_rcpt(msg):
+                send_message_transactional(msg, datamanager=datamanager)
+                emails.append(Email.from_message(
+                        msg, resource=record,
                         notification_email=trigger.notification_email,
                         notification_trigger=trigger))
         Email.save(emails)
 
     def _get_recipients(self, record, name):
         if name == 'id':
             return record
@@ -347,31 +341,19 @@
 
     model = fields.Function(fields.Char("Model"), 'get_model')
 
     def get_model(self, name):
         return self.notification.model
 
     @classmethod
-    def get_mime(cls, report, record, language):
+    def get(cls, report, record, language):
         pool = Pool()
         Report = pool.get(report.report_name, type='report')
         with Transaction().set_context(language=language):
             ext, content, _, title = Report.execute(
                 [record.id], {
                     'action_id': report.id,
                     })
         name = '%s.%s' % (title, ext)
-        mimetype, _ = mimetypes.guess_type(name)
-        if mimetype:
-            msg = MIMENonMultipart(*mimetype.split('/'))
-            msg.set_payload(content)
-            encode_base64(msg)
-        else:
-            msg = MIMEApplication(content)
-        if not isinstance(name, str):
-            name = name.encode('utf-8')
-        if not isinstance(language, str):
-            language = language.encode('utf-8')
-        msg.add_header(
-            'Content-Disposition', 'attachment',
-            filename=('utf-8', language, name))
-        return msg
+        if isinstance(content, str):
+            content = content.encode('utf-8')
+        return name, content
```

### Comparing `trytond_notification_email-7.0.0/notification.xml` & `trytond_notification_email-7.2.0/notification.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_notification_email-7.0.0/notification.xml` & `trytond_notification_email-7.2.0/notification.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_email_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="email_view_form"/>
       <field name="act_window" ref="act_email_form"/>
     </record>
     <menuitem parent="ir.menu_models" action="act_email_form" sequence="50" id="menu_email_form"/>
     <record model="ir.model.access" id="access_email">
-      <field name="model" search="[('model', '=', 'notification.email')]"/>
+      <field name="model">notification.email</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_email_admin">
-      <field name="model" search="[('model', '=', 'notification.email')]"/>
+      <field name="model">notification.email</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_notification_email-7.0.0/setup.py` & `trytond_notification_email-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/tests/test_module.py` & `trytond_notification_email-7.2.0/tests/test_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime as dt
 import sys
 import unittest
-from unittest.mock import ANY, patch
+from unittest.mock import patch
 
 from trytond.config import config
 
 try:
     from trytond.modules.company.tests import CompanyTestMixin
 except ImportError:
     class CompanyTestMixin:
@@ -30,42 +30,37 @@
         super(NotificationEmailTestCase, self).setUp()
         reset_from = config.get('email', 'from', default='')
         config.set('email', 'from', FROM)
         self.addCleanup(lambda: config.set('email', 'from', reset_from))
 
     def _setup_notification(self, recipient_field='create_uid'):
         pool = Pool()
-        Model = pool.get('ir.model')
         ModelField = pool.get('ir.model.field')
         Action = pool.get('ir.action')
         Report = pool.get('ir.action.report')
         User = pool.get('res.user')
         NotificationEmail = pool.get('notification.email')
 
-        model, = Model.search([
-                ('model', '=', User.__name__),
-                ])
-
         action = Action(name="Notification Email", type='ir.action.report')
         action.save()
         report = Report()
         report.report_name = 'notification_notification.test.report'
         report.action = action
         report.template_extension = 'txt'
         report.report_content = b'Hello ${records[0].name}'
-        report.model = model.model
+        report.model = User.__name__
         report.save()
 
         user = User(Transaction().user)
         user.email = 'user@example.com'
         user.save()
 
         notification_email = NotificationEmail()
         notification_email.recipients, = ModelField.search([
-                ('model.model', '=', model.model),
+                ('model', '=', User.__name__),
                 ('name', '=', recipient_field),
                 ])
         notification_email.content = report
         notification_email.save()
 
     def run_tasks(self, count=None):
         pool = Pool()
@@ -81,15 +76,15 @@
                 if i >= count:
                     break
 
     @unittest.skipIf(
         (3, 5, 0) <= sys.version_info < (3, 5, 2), "python bug #25195")
     @with_transaction()
     def test_notification_email(self):
-        "Test email notificiation is sent on trigger"
+        "Test email notification is sent on trigger"
         pool = Pool()
         User = pool.get('res.user')
         Trigger = pool.get('ir.trigger')
         Model = pool.get('ir.model')
         NotificationEmail = pool.get('notification.email')
         Email = pool.get('ir.email')
 
@@ -105,29 +100,27 @@
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
-                notification_module, 'sendmail_transactional') as sendmail, \
+                notification_module,
+                'send_message_transactional') as send_message, \
                 patch.object(notification_module, 'SMTPDataManager'):
             user, = User.create([{'name': "Michael Scott", 'login': "msc"}])
             self.run_tasks()
-            sendmail.assert_called_once_with(
-                FROM, ['user@example.com'], ANY,
-                datamanager=ANY)
-            _, _, msg = sendmail.call_args[0]
+            send_message.assert_called_once()
+            msg, = send_message.call_args[0]
             self.assertEqual(msg['From'], FROM)
             self.assertEqual(msg['Subject'], 'Notification Email')
             self.assertEqual(msg['To'], 'Administrator <user@example.com>')
             self.assertEqual(msg['Auto-Submitted'], 'auto-generated')
-            self.assertEqual(msg.get_content_type(), 'multipart/alternative')
             self.assertEqual(
-                msg.get_payload(0).get_payload(), 'Hello Michael Scott')
+                msg.get_body().get_content(), 'Hello Michael Scott\n')
 
         email, = Email.search([])
         self.assertEqual(email.recipients, 'Administrator <user@example.com>')
         self.assertEqual(email.recipients_secondary, '')
         self.assertEqual(email.recipients_hidden, '')
         self.assertEqual(email.subject, 'Notification Email')
         self.assertEqual(email.resource, user)
@@ -158,24 +151,23 @@
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
-                notification_module, 'sendmail_transactional') as sendmail, \
+                notification_module,
+                'send_message_transactional') as send_message, \
                 patch.object(notification_module, 'SMTPDataManager'):
             user, = User.create([{
                         'name': "Michael Scott",
                         'login': "msc",
                         'email': 'msc@example.com'}])
             self.run_tasks()
-            sendmail.assert_called_once_with(
-                FROM, ['msc@example.com'], ANY,
-                datamanager=ANY)
+            send_message.assert_called_once()
 
         email, = Email.search([])
         self.assertEqual(email.recipients, 'Michael Scott <msc@example.com>')
         self.assertEqual(email.resource, user)
         self.assertEqual(email.notification_email, notification_email)
         self.assertEqual(email.notification_trigger, trigger)
 
@@ -202,22 +194,22 @@
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
-                notification_module, 'sendmail_transactional') as sendmail, \
+                notification_module,
+                'send_message_transactional') as send_message, \
                 patch.object(notification_module, 'SMTPDataManager'):
             User.create([{'name': "Michael Scott", 'login': "msc"}])
             self.run_tasks(1)
-            sendmail.assert_not_called()
+            send_message.assert_not_called()
             self.run_tasks()
-            sendmail.assert_called_once_with(
-                FROM, ['user@example.com'], ANY, datamanager=ANY)
+            send_message.assert_called_once()
 
     @with_transaction()
     def test_notification_email_attachment(self):
         "Test email notificiation with attachment"
         pool = Pool()
         Model = pool.get('ir.model')
         Report = pool.get('ir.action.report')
@@ -241,25 +233,23 @@
 
         notification_email, = NotificationEmail.search([])
         notification_email.attachments = [attachment]
         notification_email.save()
 
         user, = User.create([{'name': "Michael Scott", 'login': "msc"}])
 
-        msg, title = notification_email.get_email(
+        msg = notification_email.get_email(
             user, FROM, ['Administrator <user@example.com>'], [], [], [en])
 
         self.assertEqual(msg['From'], FROM)
         self.assertEqual(msg['Subject'], 'Notification Email')
         self.assertEqual(msg['To'], 'Administrator <user@example.com>')
         self.assertEqual(msg.get_content_type(), 'multipart/mixed')
-        self.assertEqual(
-            msg.get_payload(0).get_content_type(), 'multipart/alternative')
 
-        attachment = msg.get_payload(1)
+        attachment = list(msg.iter_attachments())[0]
         self.assertEqual(
             attachment.get_payload(None, True),
             b'attachment for Michael Scott')
         self.assertEqual(
             attachment.get_content_type(), 'text/plain')
         self.assertEqual(
             attachment.get_filename(), "Attachment-Michael Scott.txt")
@@ -281,15 +271,15 @@
 
         notification_email, = NotificationEmail.search([])
         notification_email.subject = 'Notification for ${record.name}'
         notification_email.save()
 
         user, = User.create([{'name': "Michael Scott", 'login': "msc"}])
 
-        msg, title = notification_email.get_email(
+        msg = notification_email.get_email(
             user, FROM, ['Administrator <user@example.com>'], [], [], [en])
 
         self.assertEqual(msg['Subject'], 'Notification for Michael Scott')
 
     @with_transaction()
     def test_notification_email_translated_subject(self):
         "Test email notificiation with translated subject"
@@ -317,15 +307,15 @@
 
         user, = User.create([{
                     'name': "Michael Scott",
                     'login': "msc",
                     'language': es.id,
                     }])
 
-        msg, title = notification_email.get_email(
+        msg = notification_email.get_email(
             user, FROM, ['Administrator <user@example.com>'], [], [], [es])
 
         self.assertEqual(msg['Subject'], 'Notificación para Michael Scott')
 
     @unittest.skipIf(
         (3, 5, 0) <= sys.version_info < (3, 5, 2), "python bug #25195")
     @with_transaction()
@@ -359,22 +349,21 @@
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
-                notification_module, 'sendmail_transactional') as sendmail, \
+                notification_module,
+                'send_message_transactional') as send_message, \
                 patch.object(notification_module, 'SMTPDataManager'):
             User.create([{'name': "Michael Scott", 'login': "msc"}])
             self.run_tasks()
-            sendmail.assert_called_once_with(
-                FROM, ['fallback@example.com'], ANY,
-                datamanager=ANY)
-            _, _, msg = sendmail.call_args[0]
+            send_message.assert_called_once()
+            msg, = send_message.call_args[0]
             self.assertEqual(msg['To'], 'Fallback <fallback@example.com>')
 
     @with_transaction()
     def test_notification_email_no_recipient(self):
         "Test email notification no recipient"
         pool = Pool()
         User = pool.get('res.user')
@@ -397,15 +386,16 @@
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
-                notification_module, 'get_email') as get_email, \
+                notification_module,
+                'send_message_transactional') as send_message_transactional, \
                 patch.object(notification_module, 'SMTPDataManager'):
             User.create([{'name': "Michael Scott", 'login': "msc"}])
             self.run_tasks()
-            get_email.assert_not_called()
+            send_message_transactional.assert_not_called()
 
 
 del ModuleTestCase
```

### Comparing `trytond_notification_email-7.0.0/tox.ini` & `trytond_notification_email-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-7.0.0/trytond_notification_email.egg-info/PKG-INFO` & `trytond_notification_email-7.2.0/trytond_notification_email.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-notification-email
-Version: 7.0.0
+Name: trytond_notification_email
+Version: 7.2.0
 Summary: Tryton module for sending email notifications
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
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
 Requires-Dist: python-sql
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_company<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_commission<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_party<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_web_user<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_company<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_commission<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_party<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_web_user<7.3,>=7.2; extra == "test"
 
 Notification Email Module
 #########################
 
 The notification email module allows to define email templates which will be
 sent to a list of recipients when a trigger is fired on a record event.
 Extra reports from the same record can be attached to the email.
```

### Comparing `trytond_notification_email-7.0.0/trytond_notification_email.egg-info/SOURCES.txt` & `trytond_notification_email-7.2.0/trytond_notification_email.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_notification_email-7.0.0/view/email_form.xml` & `trytond_notification_email-7.2.0/view/email_form.xml`

 * *Files identical despite different names*

