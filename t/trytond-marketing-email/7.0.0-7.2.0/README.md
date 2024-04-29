# Comparing `tmp/trytond_marketing_email-7.0.0.tar.gz` & `tmp/trytond_marketing_email-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_email-7.0.0.tar", last modified: Mon Oct 30 17:31:15 2023, max compression
+gzip compressed data, was "trytond_marketing_email-7.2.0.tar", last modified: Mon Apr 29 15:41:40 2024, max compression
```

## Comparing `trytond_marketing_email-7.0.0.tar` & `trytond_marketing_email-7.2.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.505839 trytond_marketing_email-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:23:06.000000 trytond_marketing_email-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-10-30 17:07:18.000000 trytond_marketing_email-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-10-30 17:07:17.000000 trytond_marketing_email-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3891 2023-10-30 17:31:15.505839 trytond_marketing_email-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.502506 trytond_marketing_email-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:23:06.000000 trytond_marketing_email-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:06.000000 trytond_marketing_email-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/email_subscribe.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/email_unsubscribe.html
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/empty.gif
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-07 15:40:36.000000 trytond_marketing_email-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.502506 trytond_marketing_email-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/icons/tryton-marketing-mail.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.502506 trytond_marketing_email-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6320 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6248 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6376 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6197 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5440 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5240 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6134 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6195 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_marketing_email-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19903 2023-10-07 15:40:36.000000 trytond_marketing_email-7.0.0/marketing.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10433 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-10-07 15:40:36.000000 trytond_marketing_email-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:31:15.505839 trytond_marketing_email-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4361 2023-10-27 17:38:49.000000 trytond_marketing_email-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.502506 trytond_marketing_email-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5610 2023-08-13 15:26:13.000000 trytond_marketing_email-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_marketing_email-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-10-30 17:07:14.000000 trytond_marketing_email-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.505839 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3891 2023-10-30 17:31:15.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1998 2023-10-30 17:31:15.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:31:15.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:31:15.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-10-30 17:31:15.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:31:15.000000 trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:15.502506 trytond_marketing_email-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/view/email_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-08-21 07:34:17.000000 trytond_marketing_email-7.0.0/view/email_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/view/email_message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/view/email_message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/view/send_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_email-7.0.0/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.814145 trytond_marketing_email-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      891 2024-04-29 15:20:42.000000 trytond_marketing_email-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2024-04-29 15:20:42.000000 trytond_marketing_email-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3891 2024-04-29 15:41:40.814145 trytond_marketing_email-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.810811 trytond_marketing_email-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_marketing_email-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:12.000000 trytond_marketing_email-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/email_subscribe.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/email_unsubscribe.html
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/empty.gif
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_marketing_email-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.810811 trytond_marketing_email-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/icons/tryton-marketing-mail.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.810811 trytond_marketing_email-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6320 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6248 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6376 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6197 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5440 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5240 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6134 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6195 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-04-27 16:43:24.000000 trytond_marketing_email-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19964 2024-04-29 13:17:17.000000 trytond_marketing_email-7.2.0/marketing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10226 2024-04-27 16:30:39.000000 trytond_marketing_email-7.2.0/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2024-02-04 18:51:26.000000 trytond_marketing_email-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:40.814145 trytond_marketing_email-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4361 2024-03-17 11:01:36.000000 trytond_marketing_email-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.810811 trytond_marketing_email-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5556 2024-04-27 16:30:39.000000 trytond_marketing_email-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:12.000000 trytond_marketing_email-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-04-29 15:20:38.000000 trytond_marketing_email-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.814145 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3891 2024-04-29 15:41:40.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1980 2024-04-29 15:41:40.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:40.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:41:40.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2024-04-29 15:41:40.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:40.000000 trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:40.814145 trytond_marketing_email-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/view/email_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-01-27 09:58:52.000000 trytond_marketing_email-7.2.0/view/email_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/view/email_message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/view/email_message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/view/send_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_email-7.2.0/web.py
```

### Comparing `trytond_marketing_email-7.0.0/CHANGELOG` & `trytond_marketing_email-7.2.0/CHANGELOG`

 * *Files 9% similar despite different names*

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

### Comparing `trytond_marketing_email-7.0.0/COPYRIGHT` & `trytond_marketing_email-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2018 Sergi Almacellas Abellana
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

### Comparing `trytond_marketing_email-7.0.0/LICENSE` & `trytond_marketing_email-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/PKG-INFO` & `trytond_marketing_email-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_email
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to manage marketing mailing lists
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
@@ -46,19 +46,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_marketing<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_web_user<7.1,>=7.0
-Requires-Dist: trytond_web_shortener<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_marketing<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_web_user<7.3,>=7.2
+Requires-Dist: trytond_web_shortener<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Marketing Email Module
 ######################
 
 The marketing_email module manages mailing lists.
```

### Comparing `trytond_marketing_email-7.0.0/README.rst` & `trytond_marketing_email-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/__init__.py` & `trytond_marketing_email-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/doc/conf.py` & `trytond_marketing_email-7.2.0/doc/conf.py`

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

### Comparing `trytond_marketing_email-7.0.0/doc/index.rst` & `trytond_marketing_email-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/email_subscribe.html` & `trytond_marketing_email-7.2.0/email_subscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/email_unsubscribe.html` & `trytond_marketing_email-7.2.0/email_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/icons/LICENSE` & `trytond_marketing_email-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/bg.po` & `trytond_marketing_email-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/ca.po` & `trytond_marketing_email-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/cs.po` & `trytond_marketing_email-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/de.po` & `trytond_marketing_email-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/es.po` & `trytond_marketing_email-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/es_419.po` & `trytond_marketing_email-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/et.po` & `trytond_marketing_email-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/fa.po` & `trytond_marketing_email-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/fi.po` & `trytond_marketing_email-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/fr.po` & `trytond_marketing_email-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/hu.po` & `trytond_marketing_email-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/id.po` & `trytond_marketing_email-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/it.po` & `trytond_marketing_email-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/lo.po` & `trytond_marketing_email-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/lt.po` & `trytond_marketing_email-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/nl.po` & `trytond_marketing_email-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/pl.po` & `trytond_marketing_email-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/pt.po` & `trytond_marketing_email-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/ro.po` & `trytond_marketing_email-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/ru.po` & `trytond_marketing_email-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/sl.po` & `trytond_marketing_email-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/tr.po` & `trytond_marketing_email-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/uk.po` & `trytond_marketing_email-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/locale/zh_CN.po` & `trytond_marketing_email-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/marketing.py` & `trytond_marketing_email-7.2.0/marketing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import random
 import time
 from collections import defaultdict
-from email.header import Header
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-from email.utils import formataddr, getaddresses
-from functools import lru_cache
+from email.headerregistry import Address
+from email.message import EmailMessage
+from functools import lru_cache, partial
 from urllib.parse import (
     parse_qs, parse_qsl, urlencode, urljoin, urlsplit, urlunsplit)
 
 from genshi.core import END, START, Attrs, QName
 from genshi.template import MarkupTemplate
+from genshi.template import TemplateError as GenshiTemplateError
 from sql import Literal
 from sql.aggregate import Count
 
 try:
     import html2text
 except ImportError:
     html2text = None
@@ -25,19 +24,18 @@
 from trytond.i18n import gettext
 from trytond.ir.session import token_hex
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, Unique, Workflow, fields)
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.report import Report, get_email
-from trytond.sendmail import SMTPDataManager, sendmail_transactional
+from trytond.sendmail import SMTPDataManager, send_message_transactional
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.tools.email_ import (
-    EmailNotValidError, convert_ascii_email, normalize_email, set_from_header,
-    validate_email)
+    EmailNotValidError, normalize_email, set_from_header, validate_email)
 from trytond.transaction import Transaction, inactive_records
 from trytond.url import http_host
 from trytond.wizard import Button, StateTransition, StateView, Wizard
 
 from .exceptions import EMailValidationError, TemplateError
 
 if not config.get(
@@ -46,20 +44,14 @@
         'html', 'plugins-marketing.email.message-content',
         'fullpage')
 
 URL_BASE = config.get('marketing', 'email_base', default=http_host())
 URL_OPEN = urljoin(URL_BASE, '/m/empty.gif')
 
 
-def _formataddr(name, email):
-    if name:
-        name = str(Header(name, 'utf-8'))
-    return formataddr((name, convert_ascii_email(email)))
-
-
 def _add_params(url, **params):
     parts = urlsplit(url)
     query = parse_qsl(parts.query)
     for key, value in sorted(params.items()):
         query.append((key, value))
     parts = list(parts)
     parts[3] = urlencode(query)
@@ -319,17 +311,16 @@
             record, = records
         if not record.active:
             from_cfg = (config.get('marketing', 'email_from')
                 or config.get('email', 'from'))
             msg, title = record.get_email_subscribe()
             set_from_header(msg, from_cfg, from_ or from_cfg)
             msg['To'] = record.email
-            msg['Subject'] = Header(title, 'utf-8')
-            sendmail_transactional(
-                from_cfg, [convert_ascii_email(record.email)], msg)
+            msg['Subject'] = title
+            send_message_transactional(msg)
 
     def request_unsubscribe(self, email, from_=None):
         pool = Pool()
         Email = pool.get('marketing.email')
 
         # Randomize processing time to prevent guessing whether the email
         # address was subscribed to the list or not.
@@ -345,17 +336,16 @@
             record, = records
             if record.active:
                 from_cfg = (config.get('marketing', 'email_from')
                     or config.get('email', 'from'))
                 msg, title = record.get_email_unsubscribe()
                 set_from_header(msg, from_cfg, from_ or from_cfg)
                 msg['To'] = record.email
-                msg['Subject'] = Header(title, 'utf-8')
-                sendmail_transactional(
-                    from_cfg, [convert_ascii_email(record.email)], msg)
+                msg['Subject'] = title
+                send_message_transactional(msg)
 
 
 class Message(Workflow, ModelSQL, ModelView):
     "Marketing E-mail Message"
     __name__ = 'marketing.email.message'
     _rec_name = 'title'
 
@@ -427,15 +417,15 @@
         if field_names and 'content' not in field_names:
             return
         for message in messages:
             if not message.content:
                 continue
             try:
                 MarkupTemplate(message.content)
-            except Exception as exception:
+            except GenshiTemplateError as exception:
                 raise TemplateError(
                     gettext('marketing_email'
                         '.msg_message_invalid_content',
                         message=message.rec_name,
                         exception=exception)) from exception
 
     @classmethod
@@ -501,41 +491,49 @@
             smtpd_datamanager = SMTPDataManager()
         if messages is None:
             messages = cls.search([
                     ('state', '=', 'sending'),
                     ])
 
         for message in messages:
-            template = MarkupTemplate(message.content)
+            try:
+                template = MarkupTemplate(message.content)
+            except GenshiTemplateError as exception:
+                raise TemplateError(
+                    gettext('marketing_email'
+                        '.msg_message_invalid_content',
+                        message=message.rec_name,
+                        exception=exception)) from exception
             for email in (emails or message.list_.emails):
                 content = (template
-                    .generate(email=email)
+                    .generate(
+                        email=email,
+                        short=partial(short, record=message))
                     .filter(convert_href(message))
                     .render())
 
                 name = email.party.rec_name if email.party else ''
                 from_cfg = (config.get('marketing', 'email_from')
                     or config.get('email', 'from'))
-                to = _formataddr(name, email.email)
+                to = Address(name, addr_spec=email.email)
 
-                msg = MIMEMultipart('alternative')
+                msg = EmailMessage()
                 set_from_header(msg, from_cfg, message.from_ or from_cfg)
                 msg['To'] = to
-                msg['Subject'] = Header(message.title, 'utf-8')
+                msg['Subject'] = message.title
                 if html2text:
                     converter = html2text.HTML2Text()
-                    part = MIMEText(
-                        converter.handle(content), 'plain', _charset='utf-8')
-                    msg.attach(part)
-                part = MIMEText(content, 'html', _charset='utf-8')
-                msg.attach(part)
-
-                sendmail_transactional(
-                    from_cfg, getaddresses([to]), msg,
-                    datamanager=smtpd_datamanager)
+                    content_text = converter.handle(content)
+                    msg.add_alternative(content_text, subtype='plain')
+                if msg.is_multipart():
+                    msg.add_alternative(content, subtype='html')
+                else:
+                    msg.set_content(content, subtype='html')
+
+                send_message_transactional(msg, datamanager=smtpd_datamanager)
         if not emails:
             cls.sent(messages)
 
 
 class SendTest(Wizard):
     "Send Test E-mail"
     __name__ = 'marketing.email.send_test'
```

### Comparing `trytond_marketing_email-7.0.0/marketing.xml` & `trytond_marketing_email-7.2.0/marketing.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_marketing_email-7.0.0/marketing.xml` & `trytond_marketing_email-7.2.0/marketing.xml`

```diff
@@ -24,22 +24,22 @@
     </record>
     <record model="ir.action.keyword" id="act_email_relate_list_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">marketing.email.list,-1</field>
       <field name="action" ref="act_email_relate_list"/>
     </record>
     <record model="ir.model.access" id="access_email">
-      <field name="model" search="[('model', '=', 'marketing.email')]"/>
+      <field name="model">marketing.email</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_email_marketing_email">
-      <field name="model" search="[('model', '=', 'marketing.email')]"/>
+      <field name="model">marketing.email</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="email_list_view_form">
@@ -64,22 +64,22 @@
     <record model="ir.action.act_window.view" id="act_email_list_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="email_list_view_form"/>
       <field name="act_window" ref="act_email_list_form"/>
     </record>
     <menuitem parent="marketing.menu_marketing" action="act_email_list_form" sequence="10" id="menu_email_list_form"/>
     <record model="ir.model.access" id="access_email_list">
-      <field name="model" search="[('model', '=', 'marketing.email.list')]"/>
+      <field name="model">marketing.email.list</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_email_list_marketing_email">
-      <field name="model" search="[('model', '=', 'marketing.email.list')]"/>
+      <field name="model">marketing.email.list</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.report" id="report_email_subscribe">
@@ -143,37 +143,37 @@
     </record>
     <record model="ir.action.keyword" id="act_email_message_form_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">marketing.email.list,-1</field>
       <field name="action" ref="act_email_message_form"/>
     </record>
     <record model="ir.model.button" id="message_draft_button">
+      <field name="model">marketing.email.message</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'marketing.email.message')]"/>
     </record>
     <record model="ir.model.button" id="message_send_button">
+      <field name="model">marketing.email.message</field>
       <field name="name">send</field>
       <field name="string">Send</field>
-      <field name="model" search="[('model', '=', 'marketing.email.message')]"/>
     </record>
     <record model="ir.model.button" id="message_send_test_button">
+      <field name="model">marketing.email.message</field>
       <field name="name">send_test</field>
       <field name="string">Send Test</field>
-      <field name="model" search="[('model', '=', 'marketing.email.message')]"/>
     </record>
     <record model="ir.model.access" id="access_email_message">
-      <field name="model" search="[('model', '=', 'marketing.email.message')]"/>
+      <field name="model">marketing.email.message</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_email_message_marketing_email">
-      <field name="model" search="[('model', '=', 'marketing.email.message')]"/>
+      <field name="model">marketing.email.message</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.wizard" id="wizard_send_test">
```

### Comparing `trytond_marketing_email-7.0.0/message.xml` & `trytond_marketing_email-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/setup.py` & `trytond_marketing_email-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/tests/test_module.py` & `trytond_marketing_email-7.2.0/tests/test_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,17 +49,18 @@
         Email = pool.get('marketing.email')
         EmailList = pool.get('marketing.email.list')
 
         email_list = EmailList(name="Test")
         email_list.save()
 
         with patch.object(
-                marketing_module, 'sendmail_transactional') as sendmail:
+                marketing_module,
+                'send_message_transactional') as send_message:
             email_list.request_subscribe('user@example.com')
-            sendmail.assert_called_once_with(FROM, ['user@example.com'], ANY)
+            send_message.assert_called_once()
 
         with inactive_records():
             email, = Email.search([
                     ('list_', '=', email_list.id),
                     ])
         token = email.email_token
         self.assertTrue(token)
@@ -94,17 +95,18 @@
         email.save()
 
         token = email.email_token
         self.assertTrue(token)
         self.assertTrue(email.active)
 
         with patch.object(
-                marketing_module, 'sendmail_transactional') as sendmail:
+                marketing_module,
+                'send_message_transactional') as send_message:
             email_list.request_unsubscribe('user@example.com')
-            sendmail.assert_called_once_with(FROM, ['user@example.com'], ANY)
+            send_message.assert_called_once()
 
         self.assertEqual(
             email.get_email_unsubscribe_url(),
             '%s?token=%s' % (UNSUBSCRIBE_URL, token))
 
         Email.unsubscribe_url(UNSUBSCRIBE_URL)
         self.assertTrue(email.active)
@@ -138,21 +140,20 @@
             '</body>'
             '</html>')
         message.save()
         Message.send([message])
 
         with patch.object(
                 marketing_module,
-                'sendmail_transactional') as sendmail:
+                'send_message_transactional') as send_message:
             smtpd_datamanager = Mock()
             Message.process(smtpd_datamanager=smtpd_datamanager)
 
-            sendmail.assert_called_once_with(
-                FROM, [('', 'user@example.com')], ANY,
-                datamanager=smtpd_datamanager)
+            send_message.assert_called_once_with(
+                ANY, datamanager=smtpd_datamanager)
         urls = ShortenedURL.search([
                 ('record', '=', str(message)),
                 ])
 
         self.assertEqual(message.state, 'sent')
         self.assertEqual(len(urls), 2)
```

### Comparing `trytond_marketing_email-7.0.0/tox.ini` & `trytond_marketing_email-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/PKG-INFO` & `trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-marketing-email
-Version: 7.0.0
+Name: trytond_marketing_email
+Version: 7.2.0
 Summary: Tryton module to manage marketing mailing lists
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
@@ -46,19 +46,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_marketing<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_web_user<7.1,>=7.0
-Requires-Dist: trytond_web_shortener<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_marketing<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_web_user<7.3,>=7.2
+Requires-Dist: trytond_web_shortener<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Marketing Email Module
 ######################
 
 The marketing_email module manages mailing lists.
```

### Comparing `trytond_marketing_email-7.0.0/trytond_marketing_email.egg-info/SOURCES.txt` & `trytond_marketing_email-7.2.0/trytond_marketing_email.egg-info/SOURCES.txt`

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
 email_subscribe.html
```

### Comparing `trytond_marketing_email-7.0.0/view/email_message_form.xml` & `trytond_marketing_email-7.2.0/view/email_message_form.xml`

 * *Files identical despite different names*

