# Comparing `tmp/trytond_marketing_automation-7.0.0.tar.gz` & `tmp/trytond_marketing_automation-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_automation-7.0.0.tar", last modified: Mon Oct 30 17:31:01 2023, max compression
+gzip compressed data, was "trytond_marketing_automation-7.2.0.tar", last modified: Mon Apr 29 15:41:28 2024, max compression
```

## Comparing `trytond_marketing_automation-7.0.0.tar` & `trytond_marketing_automation-7.2.0.tar`

### file list

```diff
@@ -1,83 +1,94 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:01.889108 trytond_marketing_automation-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:23:06.000000 trytond_marketing_automation-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1179 2023-10-30 17:07:08.000000 trytond_marketing_automation-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:07:08.000000 trytond_marketing_automation-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5073 2023-10-30 17:31:01.889108 trytond_marketing_automation-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2478 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      883 2023-10-20 08:46:02.000000 trytond_marketing_automation-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:01.885774 trytond_marketing_automation-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:23:06.000000 trytond_marketing_automation-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2478 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:06.000000 trytond_marketing_automation-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/empty.gif
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1367 2023-08-13 15:26:13.000000 trytond_marketing_automation-7.0.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-08-13 15:26:13.000000 trytond_marketing_automation-7.0.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:01.882441 trytond_marketing_automation-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13972 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13810 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14096 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12060 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13940 2023-10-30 16:47:45.000000 trytond_marketing_automation-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11291 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11915 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13712 2023-10-30 16:47:45.000000 trytond_marketing_automation-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11154 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12722 2023-10-30 16:47:45.000000 trytond_marketing_automation-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-10-28 12:11:23.000000 trytond_marketing_automation-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32547 2023-10-27 17:38:49.000000 trytond_marketing_automation-7.0.0/marketing_automation.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16627 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/marketing_automation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1574 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1683 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)      539 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:31:01.889108 trytond_marketing_automation-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4590 2023-10-27 17:38:49.000000 trytond_marketing_automation-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:01.885774 trytond_marketing_automation-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/tests/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/tests/reminder.html
--rw-r--r--   0 ced       (1000) ced       (1000)     6808 2023-10-20 08:46:02.000000 trytond_marketing_automation-7.0.0/tests/scenario_marketing_automation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2023-10-20 08:46:02.000000 trytond_marketing_automation-7.0.0/tests/scenario_marketing_automation_unsubscribable.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_marketing_automation-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-10-30 17:07:05.000000 trytond_marketing_automation-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:01.889108 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5073 2023-10-30 17:31:01.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2497 2023-10-30 17:31:01.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:31:01.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:31:01.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:31:01.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:31:01.000000 trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      554 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/unsubscribe.html
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:31:01.885774 trytond_marketing_automation-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/activity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-10-20 08:46:02.000000 trytond_marketing_automation-7.0.0/view/activity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-08-13 15:26:13.000000 trytond_marketing_automation-7.0.0/view/ir_email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/record_activity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/record_activity_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/record_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/record_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/view/scenario_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-10-20 08:46:02.000000 trytond_marketing_automation-7.0.0/view/scenario_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.0.0/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2024-04-29 15:20:32.000000 trytond_marketing_automation-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:20:32.000000 trytond_marketing_automation-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2957 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.057812 trytond_marketing_automation-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:12.000000 trytond_marketing_automation-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/empty.gif
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-04 22:18:16.000000 trytond_marketing_automation-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1367 2024-01-27 09:58:52.000000 trytond_marketing_automation-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2024-01-27 09:58:52.000000 trytond_marketing_automation-7.2.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.057812 trytond_marketing_automation-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18429 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18148 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18557 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16430 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18276 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15090 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16077 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17996 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14826 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16995 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14798 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37559 2024-04-29 13:17:17.000000 trytond_marketing_automation-7.2.0/marketing_automation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16310 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/marketing_automation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8800 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/marketing_automation_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5353 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/marketing_automation_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1574 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1683 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      539 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4817 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.057812 trytond_marketing_automation-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/reminder.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     8496 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3273 2024-04-27 16:30:39.000000 trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation_unsubscribable.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:12.000000 trytond_marketing_automation-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-29 15:20:28.000000 trytond_marketing_automation-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2957 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3201 2024-04-29 15:41:28.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:27.000000 trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      554 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/unsubscribe.html
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:28.061145 trytond_marketing_automation-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/activity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      825 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/activity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-01-27 09:58:52.000000 trytond_marketing_automation-7.2.0/view/ir_email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_activity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_activity_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/record_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_activity_graph_count.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_activity_graph_rate.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      734 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_activity_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_scenario_graph_count.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_scenario_graph_rate.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/reporting_scenario_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/view/scenario_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-22 12:14:36.000000 trytond_marketing_automation-7.2.0/view/scenario_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-04-15 07:12:15.000000 trytond_marketing_automation-7.2.0/web.py
```

### Comparing `trytond_marketing_automation-7.0.0/CHANGELOG` & `trytond_marketing_automation-7.2.0/CHANGELOG`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Add trend spark lines
+* Add reporting on scenario and activity per period
+* Display block rate instead of absolute value
+* Display email rates instead of absolute value
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
@@ -13,32 +21,39 @@
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow party to be unsubscribed from scenario
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
 * Remove support for Python 3.6
 
 Version 6.2.0 - 2021-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.0.0 - 2021-05-03
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow different FROM per language
 * Add format methods from Report to email rendering context
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 * Support Genshi expressions in email title
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Initial release
```

### Comparing `trytond_marketing_automation-7.0.0/COPYRIGHT` & `trytond_marketing_automation-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2018-2023 B2CK
-Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2024 B2CK
+Copyright (C) 2018-2024 Cédric Krier
 Copyright (C) 2018-2019 Nicolas Êvrard
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_marketing_automation-7.0.0/LICENSE` & `trytond_marketing_automation-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/__init__.py` & `trytond_marketing_automation-7.2.0/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.pool import Pool
 
-from . import ir, marketing_automation, party, routes, sale, web
+from . import (
+    ir, marketing_automation, marketing_automation_reporting, party, routes,
+    sale, web)
 
 __all__ = ['register', 'routes']
 
 
 def register():
     Pool.register(
         ir.Cron,
         ir.Email,
         marketing_automation.Scenario,
         marketing_automation.Activity,
         marketing_automation.Record,
         marketing_automation.RecordActivity,
+        marketing_automation_reporting.Context,
+        marketing_automation_reporting.Scenario,
+        marketing_automation_reporting.Activity,
         party.Party,
         party.PartyUnsubscribedScenario,
         web.ShortenedURL,
         module='marketing_automation', type_='model')
     Pool.register(
         sale.Sale,
         module='marketing_automation', type_='model',
```

### Comparing `trytond_marketing_automation-7.0.0/doc/conf.py` & `trytond_marketing_automation-7.2.0/doc/conf.py`

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

### Comparing `trytond_marketing_automation-7.0.0/ir.py` & `trytond_marketing_automation-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/ir.xml` & `trytond_marketing_automation-7.2.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/locale/bg.po` & `trytond_marketing_automation-7.2.0/locale/id.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,66 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr ""
+msgstr "Aktivitas"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr ""
+msgstr "Tindakan"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr ""
+msgstr "Cabang"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr ""
+msgstr "Kondisi"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
+msgstr "Jeda"
+
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
+msgstr "Dari"
+
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
@@ -48,27 +73,27 @@
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "Induk"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
@@ -80,23 +105,23 @@
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr ""
+msgstr "Skenario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr ""
+msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr ""
+msgstr "Aktivitas"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
@@ -114,29 +139,110 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Aktivitas"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Aktivitas"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Tanggal Penulisan"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Skenario"
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
@@ -156,20 +262,20 @@
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
 msgstr ""
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr ""
+msgstr "Pihak"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr ""
+msgstr "Skenario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
 msgstr ""
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
@@ -223,14 +329,24 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Aktivitas"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Skenario"
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -258,15 +374,15 @@
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Rancangan"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
 msgstr ""
 
 msgctxt ""
@@ -318,15 +434,15 @@
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Rancangan"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
@@ -344,14 +460,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -407,51 +535,68 @@
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
 msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr ""
+msgstr "Aktivitas"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr ""
+msgstr "Skenario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Dibatalkan"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Jeda"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Rancangan"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr ""
+msgstr "Sunting"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
@@ -463,12 +608,24 @@
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
+msgstr "Waktu"
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
 msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/ca.po` & `trytond_marketing_automation-7.2.0/locale/it.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,493 +1,653 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Attività"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Registre"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Acció"
+msgstr "Azione"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Fills"
+msgstr "Figlio"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Condició"
+msgstr "Condizione"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Retard"
+msgstr "Ritardo"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail cliccate"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "E-mail cliccate"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Correus electrònics clicats"
+msgstr "E-mail cliccate"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "De"
+msgstr "Da"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mail aperte"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "E-mail aperte"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Correus electrònics oberts"
+msgstr "E-mail aperte"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Plantilla de correu electrònic"
+msgstr "Modello E-mail"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "Títol del correu electrònic"
+msgstr "Titolo E-mail"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Esdeveniment"
+msgstr "Evento"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Nome"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negatiu"
+msgstr "Negativo"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "A"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Pare"
+msgstr "Padre"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Acció pare"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Registres"
+msgstr ""
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Bloquejat"
+msgstr "Bloccato"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Registre"
+msgstr ""
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "Identificador únic universal"
+msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Attività"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Acció d'activitat"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
 msgstr "A"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "Correus electrònics clicats"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "Correus electrònics oberts"
+msgstr "E-mail aperte"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Registre"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Stato"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Attività"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Attività"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail cliccate"
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "E-mail cliccate"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mail aperte"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "E-mail aperte"
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Da"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Bloccato"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Bloccato"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Scenario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Activitats"
+msgstr "Attività"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Bloccato"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "Bloccato"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domini"
+msgstr "Dominio"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Model"
+msgstr "Modello"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Nome"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Registres"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Registres bloquejats"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Stato"
 
+#, fuzzy
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Donar-se de baixa"
+msgstr "Annulla l'iscrizione"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercer de màrqueting"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Escenàris d'automatització de màrqueting no subscrits"
+msgstr "Automazione Marketing disiscrivi"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr ""
 
+#, fuzzy
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercer de màrqueting"
+msgstr ""
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"L'expressió PYSON que el registre ha de complir per tal d'executar-se l'activitat.\n"
-"El registre s'expressa amb \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Desprès de quant temps s'hauria d'executar l'acció."
+msgstr "Dopo quanto tempo l'azione dovrebbe essere eseguita."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr "Deixa buit per utilizar el valor definit al fitxer de configuració."
+msgstr "Lasciare vuoto per il valore definito nel file di configurazione."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"El contingut HTML del correu electrònic.\n"
-"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"L'assumpte del correu electrònic.\n"
-"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Marcar per executar l'activitat si l'esdeveniment no s'ha executat al acabar"
-" el retard."
+"Spunta per eseguire l'attività se l'evento non si è verificato entro la fine"
+" del ritardo."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Un domini PYSON utilitzat per filtrar registres vàlid per aquest escenari."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Si es marca els tercer també es de-suscribeixen de l'escenari."
+msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Activitats"
+msgstr "Attività"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "Correus electrònics"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Activitats del registre"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Registres"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Attività"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Scenario"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Escenaris"
+msgstr "Scenari"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Baixa d'automatització de màrqueting"
+msgstr "Automazione Marketing disiscrivi"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Tot"
+msgstr "Tutti"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Cancel·lat"
+msgstr "Annullato"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Finalitzat"
+msgstr "Fatto"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "In attesa"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Tot"
+msgstr "Tutti"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Bozza"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "En execució"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Aturat"
+msgstr "Fermato"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Condició no vàlida \"%(condition)s\" a l'activitat \"%(activity)s\" amb "
-"l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Plantilla de correu electrònic no vàlida a l'activitat \"%(activity)s\" amb "
-"l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ttítol de la plantilla de correu electrònic no vàlida a l'activitat "
-"\"%(activity)s\" amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "L'activitat del registre ha de ser única per registre i activitat."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "El registre ha de ser únic per cada escenari."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "L'UUID del registre ha de ser únic."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Domini no vàlid a l'escenari \"%(scenario)s\" amb l'excepció "
-"\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "Correu electrònic clicat"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "Correu electrònic obert"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Bloqueja"
+msgstr "Bloccato"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Bozza"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "Executa"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Atura"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Escenaris"
+msgstr "Scenari"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Activitat de màrqueting"
+msgstr ""
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Registre de màrqueting"
+msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Activitat del registre de màrqueting"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Automazione Marketing disiscrivi"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Automazione Marketing disiscrivi"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Automazione Marketing disiscrivi"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Escenari de màrqueting"
+msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Escenaris de-suscrits del tercer"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Donar-se de baixa"
+msgstr "Annulla l'iscrizione"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Sentim veure't marxar, i ens disculpem si hem aclaparat la teva safata "
-"d'entrada."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "T'has donat de baixa"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr "T'has donat de baixa amb èxit d'aquest tipus de correu electrònic."
+msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Processar activitats de màrqueting"
+msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Executar disparadors del escenaris de màrqueting"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "Correu electrònic enviat"
+msgstr "Invia E-mail"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "Correu electrònic clicat"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "Correu electrònic obert"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "Correu electrònic clicat"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "Correu electrònic no clicat"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "Correu electrònic no obert"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "Correu electrònic obert"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Activitat"
+msgstr "Attività"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Escenari"
+msgstr "Scenario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Cancel·lada"
+msgstr "Annullato"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Finalitzada"
+msgstr "Fatto"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "In attesa"
+
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Ritardo"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Bozza"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "En execució"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Aturat"
+msgstr "Fermato"
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Desprès"
+msgstr "Dopo"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Edita"
+msgstr "Modifica"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Si"
+msgstr "Se"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "A"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Plantilla:"
+msgstr "Modello:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Títol:"
+msgstr "Titolo:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Hora"
+msgstr "Tempo"
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Automatització de màrqueting"
+msgstr "Automazione Marketing disiscrivi"
```

### Comparing `trytond_marketing_automation-7.0.0/locale/cs.po` & `trytond_marketing_automation-7.2.0/locale/ro.po`

 * *Files 16% similar despite different names*

```diff
@@ -8,36 +8,60 @@
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr ""
+msgstr "Acțiune"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr ""
+msgstr "Copii"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -60,15 +84,15 @@
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "Părinte"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
@@ -114,21 +138,98 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr ""
+msgstr "Domeniu"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_marketing_automation-7.0.0/locale/de.po` & `trytond_marketing_automation-7.2.0/locale/sl.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,495 +1,667 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Aktivität"
+msgstr "Aktivnost"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Datensatz"
+msgstr "Zapis"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Aktion"
+msgstr "Ukrep"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Untergeordnet"
+msgstr "Podukrepi"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Bedingung"
+msgstr "Pogoj"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Verzögerung"
+msgstr "Zakasnitev"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-poštni kliki"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "E-poštni kliki"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-poštni kliki"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Angeklickte E-Mails"
+msgstr "E-poštni kliki"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Von"
+msgstr "Od"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-pošta odprta"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "E-pošta odprta"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Geöffnete E-Mails"
+msgstr "E-pošta odprta"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "E-Mail Vorlage"
+msgstr "E-poštna predloga"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "E-Mail Titel"
+msgstr "E-poštna zadeva"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Ereignis"
+msgstr "Dogodek"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Name"
+msgstr "Naziv"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negativ"
+msgstr "Negativno"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "Bei"
+msgstr "Na"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Übergeordnet"
+msgstr "Matični ukrep"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Übergeordnete Aktion"
+msgstr "Matični ukrep"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Datensätze"
+msgstr "Zapisi"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Gesperrt"
+msgstr "Blokiran"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Datensatz"
+msgstr "Zapis"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Szenario"
+msgstr "Scenarij"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
 msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Aktivität"
+msgstr "Aktivnost"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Aktivität Aktion"
+msgstr "Ukrep aktivnosti"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "Um"
+msgstr "Ob"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "Angeklickte E-Mail"
+msgstr "E-poštni kliki"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "Geöffnete E-Mail"
+msgstr "E-pošta odprta"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Datensatz"
+msgstr "Zapis"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Stanje"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Aktivnost"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Ukrep aktivnosti"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-poštni kliki"
+
+#, fuzzy
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-poštni kliki"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "E-poštni kliki"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-pošta odprta"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "E-pošta odprta"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr "Zapisi"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Od"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Blokiran"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr "Zapisi"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Blokirani zapisi"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Scenarij"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Aktivitäten"
+msgstr "Aktivnosti"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Blokiran"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "Blokiran"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Wertebereich (Domain)"
+msgstr "Domena"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Modell"
+msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Name"
+msgstr "Naziv"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Datensätze"
+msgstr "Zapisi"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Blockierte Datensätze"
+msgstr "Blokirani zapisi"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Stanje"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Abmeldbar"
+msgstr "Odjava"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Partei"
+msgstr "Marketing Partner"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Marketingautomatisierungsszenario abgemeldet"
+msgstr ""
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Partei"
+msgstr "Partner"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Szenario"
+msgstr "Scenarij"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Partei"
+msgstr "Marketing partner"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"Der PYSON Ausdruck, dem der Datensatz entsprechen muss, damit die Aktivität ausgeführt wird.\n"
-"Der Datensatz wird durch \"self\" repräsentiert."
+"Izraz PYSON, s katerim se mora zapis ujemati, da se aktivnost izvaja.\n"
+"Zapis je predstavljen s \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Nach welcher Zeit die Aktion ausgeführt werden soll."
+msgstr "Po koliko časa naj bo ukrep izveden."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr "Leer lassen, um den Wert aus der Konfigurationsdatei zu verwenden."
+msgstr ""
+"Pustite prazno, da uporabite vrednost opredeljeno v konfiguracijski "
+"datoteki."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Der HTML Content der E-Mail.\n"
-"Die Genshi Syntax kann mit 'record' im Evaluierungskontext verwendet werden."
+"HTML vsebina e-pošte.\n"
+"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Der Betreff der E-Mail.\n"
-"Die Genshi Syntax kann mit 'record' im Evaluierungskontext verwendet werden."
+"Zadeva te e-pošte.\n"
+"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Aktivieren um die Aktivität auszulösen, wenn das Ereignis nach Ablauf des "
-"Verzögerungszeitraums noch nicht eingetreten ist."
+"Označite, če želite izvesti aktivnost, v kolikor do dogodka ni prišlo v "
+"opredeljenem zamiku."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Ein PYSON Wertebereich (Domain) zum Filtern der Datensätze, die diesem "
-"Szenario entsprechen."
+"PYSON domena, ki se uporabi za filtriranje zapisov, ki so veljavno za ta "
+"scenarij."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Wenn ausgewählt, dann werden Parteien auch vom Szenario abgemeldet."
+msgstr "Označite, da se partner lahko odjavi s tega scenarija."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Aktivitäten"
+msgstr "Aktivnosti"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "E-Mails"
+msgstr "E-pošte"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Datensatzaktivitäten"
+msgstr "Zapisi aktivnosti"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Datensätze"
+msgstr "Zapisi"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Ukrep aktivnosti"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Scenarij"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Szenarien"
+msgstr "Scenariji"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Abmeldung Marketingautomatisierung"
+msgstr "Odjave automatizacije marketinga"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Vse"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Annulliert"
+msgstr "Preklicano"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Erledigt"
+msgstr "Zaključeno"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "Wartend"
+msgstr "V čakanju"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Vse"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Entwurf"
+msgstr "Osnutek"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "In Ausführung"
+msgstr "V izvajanju"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Gestoppt"
+msgstr "Ustavljeno"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Ungültige Bedingung \"%(condition)s\" in Aktiviät \"%(activity)s\" mit "
-"Fehler \"%(exception)s\"."
+"Neveljaven pogojo \"%(condition)s\" v aktivnosti \"%(activity)s\" z napako "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ungültige E-Mail Vorlage in Aktivität \"%(activity)s\" mit Fehler "
+"Neveljavna e-poštna predloga v aktivnosti \"%(activity)s\" z napako "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ungültiger E-Mail Betreff in Aktivität \"%(activity)s\" mit Fehler "
+"Neveljavna e-poštna zadeva v aktivnosti \"%(activity)s\" z napako "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr ""
-"Eine Datensatzaktivität kann es je Datensatz und Aktivität nur einmal geben."
+msgstr "Zapis aktivnosti mora biti edinstven po zapisu in aktivnosti."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "Es kann je Szenario nur einen Datensatz geben."
+msgstr "Zapis mora biti edinstven po scenariju."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "Die UUID des Datensatzes existiert bereits."
+msgstr "UUID zapisa mora biti edinstven."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Ungültiger Wertebereich (Domain) in Szenario \"%(scenario)s\" mit Fehler "
-"\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "E-Mail angeklickt"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "E-Mail geöffnet"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Gesperrt"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Entwurf"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "Ausführen"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Stopp"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Szenarien"
+msgstr ""
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Marketingaktivität"
+msgstr ""
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Marketingdatensatz"
+msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Marketing Datensatzaktivität"
+msgstr ""
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Odjave automatizacije marketinga"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Odjave automatizacije marketinga"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Odjave automatizacije marketinga"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Marketing Szenario"
+msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Partei Abmelden Szenario"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Abmelden"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Wir bedauern Ihre Abmeldung und entschuldigen uns sofern wir Ihren "
-"Posteingang überflutet haben sollten."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "Sie sind abgemeldet"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr "Sie haben sich für diese Art von E-Mails erfolgreich abgemeldet."
+msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Marketingaktivitäten ausführen"
+msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Marketingszenarios auslösen"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "E-Mail senden"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "E-Mail angeklickt"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "E-Mail geöffnet"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "E-Mail angeklickt"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "E-Mail nicht angeklickt"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "E-Mail nicht geöffnet"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "E-Mail geöffnet"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Aktivität"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Szenario"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Annulliert"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Erledigt"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "Wartend"
+msgstr ""
+
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Zakasnitev"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Entwurf"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "In Ausführung"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Gestoppt"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Nach"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Bearbeiten"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Wenn"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "Bei"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Vorlage:"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Titel:"
+msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Zeit"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Marketingautomatisierung"
+msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/es.po` & `trytond_marketing_automation-7.2.0/locale/fr.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,495 +1,672 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr "Activité"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Registro"
+msgstr "Enregistrement"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Acción"
+msgstr "Action"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Hijos"
+msgstr "Enfants"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Condición"
+msgstr "Condition"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Retraso"
+msgstr "Délai"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail cliqué"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "E-mail cliqué"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-mail cliqué"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "Correos electrónicos pulsados"
+msgstr "E-mails cliqués"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr "De"
 
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mail ouvert"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "E-mail ouvert"
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "Correos electrónicos abiertos"
+msgstr "E-mails ouverts"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Plantilla de correo electrónico"
+msgstr "Modèle d'e-mail"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "Titulo del correo electrónico"
+msgstr "Titre de l'e-mail"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Evento"
+msgstr "Événement"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negativo"
+msgstr "Négatif"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "A"
+msgstr "Sur"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr "Parent"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Acción padre"
+msgstr "Action parente"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Registros"
+msgstr "Enregistrements"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Bloqueado"
+msgstr "Bloqué"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Registro"
+msgstr "Enregistrement"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr "Scénario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "Identificador único universal"
+msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr "Activité"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Acción de actividad"
+msgstr "Action de l'activité"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "A"
+msgstr "À"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr "E-mail cliqué"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr "E-mail ouvert"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Registro"
+msgstr "Enregistrement"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "État"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Activité"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Action de l'activité"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail cliqué"
+
+#, fuzzy
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-mail cliqué"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "E-mails cliqués"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mail ouvert"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "E-mails ouverts"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr "Enregistrements"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Date de modification"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Bloqué"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr "Enregistrements"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Enregistrements bloqués"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Scénario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Actividades"
+msgstr "Activés"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Bloqué"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "Bloqué"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Dominio"
+msgstr "Domaine"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Modelo"
+msgstr "Modèle"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Registros"
+msgstr "Enregistrements"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Registros bloqueados"
+msgstr "Enregistrements bloqués"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "État"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Darse de baja"
+msgstr "Dés-inscriptible"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercero del marketing"
+msgstr "Tiers de marketing"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Escenarios de automatización de marketing no suscritos"
+msgstr "Désinscription au scenario d'automatisation du marketing"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tiers"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr "Scénario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tercero del marketing"
+msgstr "Tiers de marketing"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"La condicion PYSON que debe satisfacer el registro para ejecutar la actividad.\n"
-"El registro es representado por \"self\"."
+"L'expression PYSON à laquelle l'enregistrement doit correspondre afin d’exécuter l'activité.\n"
+"L'enregistrement est représenté par « self »."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Después de cuánto tiempo debe ser ejecutada la acción."
+msgstr "Après combien de temps l'action doit être exécutée."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
 msgstr ""
-"Dejar vacío para usar el valor definido en el archivo de configuración."
+"Laissez vide pour utiliser la valeur définie dans le fichier de "
+"configuration."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"El contenido HTML del correo electrónico.\n"
-"La sintaxis Genshi puede ser utilizada con 'record' en el contexto de evaluación."
+"Le contenu HTML de l'e-mail.\n"
+"La syntaxe Genshi peut être utilisée avec « record » comme contexte d'évaluation."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"El asunto del correo electrónico.\n"
-"La sintaxis Genshi puede ser utilizada con 'record' en el contexto de evaluación."
+"Le sujet de l'e-mail.\n"
+"La syntaxe Genshi peut être utilisée avec « record » comme contexte d'évaluation."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Marcar para ejecutar la actividad si el evento no ha ocurrido al final de la"
-" fecha retrasada."
+"Cochez pour exécuter l'activité si l'événement ne s'est pas produit à la fin"
+" du délai."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Dominio PYSON usado para filtrar los registros válidos para este escenario."
+"Le domaine PYSON utilisé pour filtrer les enregistrements valides pour ce "
+"scénario."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Si se marca los terceros también se de-suscriben del escenario."
+msgstr "Si cochée, les tiers sont également désabonnées du scénario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Actividades"
+msgstr "Activés"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "Correos electrónicos"
+msgstr "E-mails"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Registro de actividades"
+msgstr "Enregistrements d'activités"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Registros"
+msgstr "Enregistrements"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Action de l'activité"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Scénario"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Escenarios"
+msgstr "Scénarios"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Baja de la automatización de marketing"
+msgstr "Désinscription à l'automatisation du marketing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Tous"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Annulés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Realizado"
+msgstr "Effectués"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "En attente"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Tous"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillons"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "En ejecución"
+msgstr "En cours"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Parado"
+msgstr "Arrêtés"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Condición \"%(condition)s\" inválida en la actividad \"%(activity)s\" con la"
-" excepción \"%(exception)s\"."
+"Condition « %(condition)s » non-valide sur l'activité « %(activity)s » avec "
+"l'exception « %(exception)s »."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Plantilla de correo electrónico inválida en la actividad \"%(activity)s\" "
-"con la excepción \"%(exception)s\"."
+"Modèle d'e-mail non-valide sur l'activité « %(activity)s » avec l'exception "
+"« %(exception)s »."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Título de correo electrónico inválido en la actividad \"%(activity)s\" con "
-"la excepción \"%(exception)s\"."
+"Titre d'e-mail non-valide sur l'activité « %(activity)s » avec l'exception "
+"« %(exception)s »."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "La actividad del registro debe ser única por registro y actividad."
+msgstr ""
+"L'enregistrement d'activité doit être unique par enregistrement et activité."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "El registro debe ser único por escenario."
+msgstr "L'enregistrement doit être unique par scénario."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "El UUID del registro debe ser único."
+msgstr "L'UUID de l'enregistrement doit être unique."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Dominio inválido en el escenario \"%(scenario)s\" con la excepción "
-"\"%(exception)s\"."
+"Domaine non-valide sur le scénario « %(scenario)s » avec l'exception "
+"« %(exception)s »."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr "E-mails cliqués"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr "E-mails ouverts"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Bloquear"
+msgstr "Bloquer"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillons"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "Ejecutar"
+msgstr "Exécuter"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Parar"
+msgstr "Arrêter"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Escenarios"
+msgstr "Scénarios"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Actividad de marketing"
+msgstr "Activité de marketing"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Registro de marketing"
+msgstr "Enregistrement de marketing"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Actividad del registro de marketing"
+msgstr "Enregistrement d'activité marketing"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Enregistrement d'activité marketing"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Automatisation du marketing"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Désinscription au scenario d'automatisation du marketing"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Escenario de marketing"
+msgstr "Scénario marketing"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Escenarios de-suscritos del tercero"
+msgstr "Scénario de désinscription de tiers"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Darse de baja"
+msgstr "Désinscription"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Lamentamos verle marchar y le pedimos disculpas en caso que hubiéramos "
-"abusado de su bandeja de entrada de correo electrónico."
+"Nous sommes désolé de vous voir partir, et nous présentons nos excuses si "
+"nous avons submergé votre boîte."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "Te has dado de baja"
+msgstr "Vous êtes désinscrit"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr ""
-"Se ha dado de baja de este tipo de correo electrónico satisfactoriamente."
+msgstr "Vous avez été désinscrit avec succès de ce type d'e-mail."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Procesar actividad de marketing"
+msgstr "Traiter les activités marketing"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Ejecutar disparadores de escenarios de marketing"
+msgstr "Déclencher les scénarios marketing"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "Enviar correo electrónico"
+msgstr "Envoyer un e-mail"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr "E-mail cliqué"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr "E-mail ouvert"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "Correo electrónico pulsado"
+msgstr "E-mail cliqué"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "Correo electrónico no pulsado"
+msgstr "E-mail non cliqué"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "Correo electrónico no abierto"
+msgstr "E-mail non ouvert"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "Correo electrónico abierto"
+msgstr "E-mail ouvert"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Actividad"
+msgstr "Activité"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Escenario"
+msgstr "Scénario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Annulé"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Finalizado"
+msgstr "Terminé"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "En espera"
+msgstr "En attente"
+
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Délai"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "En ejecución"
+msgstr "En cours"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Detenido"
+msgstr "Arrêté"
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Después"
+msgstr "Après"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Editar"
+msgstr "Éditer"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
 msgstr "Si"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "En"
+msgstr "Sur"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Plantilla:"
+msgstr "Modèle :"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Título:"
+msgstr "Titre :"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Hora"
+msgstr "Heure"
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Automatización de marketing"
+msgstr "Automatisation du marketing"
```

### Comparing `trytond_marketing_automation-7.0.0/locale/es_419.po` & `trytond_marketing_automation-7.2.0/locale/bg.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/et.po` & `trytond_marketing_automation-7.2.0/locale/et.po`

 * *Files 14% similar despite different names*

```diff
@@ -24,22 +24,51 @@
 msgid "Condition"
 msgstr "Tingimus"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr "Viide"
 
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail vajutatud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "E-mail vajutatud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-mail vajutatud"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr "E-mailid valitud"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr "Saatja"
 
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mail avatud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "E-mail avatud"
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr "E-mailid avatud"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr "E-maili vorm"
@@ -116,18 +145,110 @@
 msgid "Record"
 msgstr "Kirje"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr "Olek"
 
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Aktiviteet"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Aktiviteedi toiming"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail vajutatud"
+
+#, fuzzy
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-mail vajutatud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "E-mailid valitud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mail avatud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "E-mailid avatud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr "Kirjed"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Kirjutamise kuupäev"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Blokeeirtud"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr "Kirjed"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Blokeeritud kirjed"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Stsenaarium"
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr "Aktiviteedid"
 
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Blokeeirtud"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "Blokeeirtud"
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr "Domeen"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr "Mudel"
@@ -227,14 +348,24 @@
 msgid "Record Activities"
 msgstr "Kirje aktiviteedid"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Kirjed"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Aktiviteedi toiming"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Stsenaarium"
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr "Stsenaariumid"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr "Turunduse automatiseerimine - tellimuse tühistamine"
@@ -349,14 +480,29 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Turunduse automatiseerimine - tellimuse tühistamine"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Turunduse automatiseerimine - tellimuse tühistamine"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Turunduse automatiseerimine - tellimuse tühistamine"
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -430,27 +576,44 @@
 msgid "Done"
 msgstr "Tehtud"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr "Ootel"
 
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Viide"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr "Mustand"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr "Töös"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr "Peatatud"
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr "Pärast"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr "Muuda"
 
@@ -470,11 +633,23 @@
 msgid "Title:"
 msgstr "Teema:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr "Aeg"
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr "Turunduse automatiseerimine - tellimuse tühistamine"
```

### Comparing `trytond_marketing_automation-7.0.0/locale/fa.po` & `trytond_marketing_automation-7.2.0/locale/cs.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/fi.po` & `trytond_marketing_automation-7.2.0/locale/es_419.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/fr.po` & `trytond_marketing_automation-7.2.0/locale/nl.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,497 +1,671 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Activité"
+msgstr "Activiteit"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Enregistrement"
+msgstr "Record"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Action"
+msgstr "Actie"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Enfants"
+msgstr "Onderliggende niveaus"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Condition"
+msgstr "Voorwaarde"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Délai"
+msgstr "Vertraging"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail Geklikt"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "E-mail Geklikt"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-mail Geklikt"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-mails cliqués"
+msgstr "E-mails Geklikt"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "De"
+msgstr "Van"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mails geopend"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "E-mails geopend"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-mails ouverts"
+msgstr "E-mails geopend"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Modèle d'e-mail"
+msgstr "Email sjabloon"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "Titre de l'e-mail"
+msgstr "E-mail titel"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Événement"
+msgstr "Evenement"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Naam"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Négatif"
+msgstr "Negatief"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "Sur"
+msgstr "Op"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Parent"
+msgstr "Bovenliggend niveau"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Action parente"
+msgstr "Bovenliggende actie (parent)"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Enregistrements"
+msgstr "Records"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Bloqué"
+msgstr "geblokkeerd"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Enregistrement"
+msgstr "Record"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Scénario"
+msgstr "Scenario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
 msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Activité"
+msgstr "Activiteit"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Action de l'activité"
+msgstr "Activiteit actie"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "À"
+msgstr "Op"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "E-mail cliqué"
+msgstr "E-mail Geklikt"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "E-mail ouvert"
+msgstr "E-mails geopend"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Enregistrement"
+msgstr "Record"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "État"
+msgstr "Status"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Activiteit"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Activiteit actie"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "E-mail Geklikt"
+
+#, fuzzy
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "E-mail Geklikt"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "E-mails Geklikt"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "E-mails geopend"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "E-mails geopend"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr "Records"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Bewerkingsdatum"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "geblokkeerd"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr "Records"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Geblokkeerde records"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Scenario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Activés"
+msgstr "Activiteiten"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "geblokkeerd"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "geblokkeerd"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domaine"
+msgstr "Domein (domain)"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Modèle"
+msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Naam"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Enregistrements"
+msgstr "Records"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Enregistrements bloqués"
+msgstr "Geblokkeerde records"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "État"
+msgstr "Status"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Dés-inscriptible"
+msgstr "Afmelden mogelijk"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tiers de marketing"
+msgstr "Marketing Relatie"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Désinscription au scenario d'automatisation du marketing"
+msgstr "Marketing Abonnement opgezegd"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Relatie"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scénario"
+msgstr "Scenario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Tiers de marketing"
+msgstr "Marketing Relatie"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"L'expression PYSON à laquelle l'enregistrement doit correspondre afin d’exécuter l'activité.\n"
-"L'enregistrement est représenté par « self »."
+"De PYSON-expressie waaraan het record moet voldoen om de activiteit te kunnen uitvoeren.\n"
+"Het record wordt vertegenwoordigd door \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Après combien de temps l'action doit être exécutée."
+msgstr "Na hoeveel tijd moet de actie worden uitgevoerd."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
 msgstr ""
-"Laissez vide pour utiliser la valeur définie dans le fichier de "
-"configuration."
+"Laat leeg om de waarde te gebruiken die gedefinieerd is in het "
+"configuratiebestand."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Le contenu HTML de l'e-mail.\n"
-"La syntaxe Genshi peut être utilisée avec « record » comme contexte d'évaluation."
+"De HTML-inhoud van de e-mail.\n"
+"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Le sujet de l'e-mail.\n"
-"La syntaxe Genshi peut être utilisée avec « record » comme contexte d'évaluation."
+"Het onderwerp van de e-mail.\n"
+"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Cochez pour exécuter l'activité si l'événement ne s'est pas produit à la fin"
-" du délai."
+"Schakel het selectievakje in om de activiteit uit te voeren als het "
+"evenement niet is gebeurd aan het einde van de vertraging."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Le domaine PYSON utilisé pour filtrer les enregistrements valides pour ce "
-"scénario."
+"Een PYSON-domein dat wordt gebruikt om records te filteren die geldig zijn "
+"voor dit scenario."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Si cochée, les tiers sont également désabonnées du scénario."
+msgstr ""
+"Indien aangevinkt worden de relaties ook uitgeschreven uit het scenario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Activés"
+msgstr "Activiteiten"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
 msgstr "E-mails"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Enregistrements d'activités"
+msgstr "Activiteiten opnemen"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Enregistrements"
+msgstr "Records"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Activiteit actie"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Scenario"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Scénarios"
+msgstr "scenario's"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Désinscription à l'automatisation du marketing"
+msgstr "Marketing Automatizerings Abonnement opzeggen"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Tous"
+msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Annulés"
+msgstr "Geannuleerd"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Effectués"
+msgstr "Klaar"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "En attente"
+msgstr "In afwachting"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Tous"
+msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Brouillons"
+msgstr "Concept"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "En cours"
+msgstr "in uitvoering"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Arrêtés"
+msgstr "gestopt"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Condition « %(condition)s » non-valide sur l'activité « %(activity)s » avec "
-"l'exception « %(exception)s »."
+"Ongeldige voorwaarde \"%(condition)s\" in activiteit \"%(activity)s\" met "
+"uitzondering \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Modèle d'e-mail non-valide sur l'activité « %(activity)s » avec l'exception "
-"« %(exception)s »."
+"Ongeldige e-mailsjabloon in activiteit \"%(activity s\" met uitzondering "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Titre d'e-mail non-valide sur l'activité « %(activity)s » avec l'exception "
-"« %(exception)s »."
+"Ongeldige e-mailtitel in activiteit \"%(activity s\" met uitzondering "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr ""
-"L'enregistrement d'activité doit être unique par enregistrement et activité."
+msgstr "Recordactiviteit moet uniek zijn per record en activiteit."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "L'enregistrement doit être unique par scénario."
+msgstr "Record moet uniek zijn per scenario."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "L'UUID de l'enregistrement doit être unique."
+msgstr "UUID van het record moet uniek zijn."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Domaine non-valide sur le scénario « %(scenario)s » avec l'exception "
-"« %(exception)s »."
+"Ongeldig domein in scenario \"%(scenario)s\" met uitzondering "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "E-mails cliqués"
+msgstr "E-mail Geklikt"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "E-mails ouverts"
+msgstr "E-mails geopend"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Bloquer"
+msgstr "Blokkeer"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Brouillons"
+msgstr "Concept"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "Exécuter"
+msgstr "uitvoeren"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "Arrêter"
+msgstr "stop"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Scénarios"
+msgstr "scenario's"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Activité de marketing"
+msgstr "Marketing activiteit"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Enregistrement de marketing"
+msgstr "Marketingrecord"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Enregistrement d'activité marketing"
+msgstr "Marketingrecordactiviteit"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Marketingrecordactiviteit"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Marketing Abonnement Opzeggen"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Marketing Abonnement opgezegd"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Scénario marketing"
+msgstr "Marketingscenario"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Scénario de désinscription de tiers"
+msgstr "Relatie Uitschrijf Scenario"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Désinscription"
+msgstr "Afmelden"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Nous sommes désolé de vous voir partir, et nous présentons nos excuses si "
-"nous avons submergé votre boîte."
+"Het spijt ons u te zien gaan. Onze excuses als we uw inbox vervuild hebben ."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "Vous êtes désinscrit"
+msgstr "U bent uitgeschreven"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr "Vous avez été désinscrit avec succès de ce type d'e-mail."
+msgstr "U bent succesvol afgemeld voor dit soort e-mail."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Traiter les activités marketing"
+msgstr "Marketingactiviteit verwerken"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Déclencher les scénarios marketing"
+msgstr "Trigger Marketing Scenario's"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "Envoyer un e-mail"
+msgstr "E-mail verzenden"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "E-mail cliqué"
+msgstr "E-mail Geklikt"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "E-mail ouvert"
+msgstr "E-mails geopend"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "E-mail cliqué"
+msgstr "E-mail Geklikt"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "E-mail non cliqué"
+msgstr "E-mail niet aangeklikt"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "E-mail non ouvert"
+msgstr "E-mail niet geopend"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "E-mail ouvert"
+msgstr "E-mails geopend"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Activité"
+msgstr "Activiteit"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Scénario"
+msgstr "Scenario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Annulé"
+msgstr "Geannuleerd"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Terminé"
+msgstr "Klaar"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "En attente"
+msgstr "In afwachting"
+
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Vertraging"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "Concept"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "En cours"
+msgstr "in uitvoering"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Arrêté"
+msgstr "gestopt"
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Après"
+msgstr "Na"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Éditer"
+msgstr "Bewerk"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Si"
+msgstr "Als"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "Sur"
+msgstr "Op"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Modèle :"
+msgstr "Sjabloon:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Titre :"
+msgstr "Titel:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Heure"
+msgstr "Tijd"
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Automatisation du marketing"
+msgstr "Marketing Abonnement Opzeggen"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_marketing_automation-7.0.0/locale/hu.po` & `trytond_marketing_automation-7.2.0/locale/fa.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/id.po` & `trytond_marketing_automation-7.2.0/locale/fi.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Aktivitas"
+msgstr ""
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Tindakan"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Cabang"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Kondisi"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Jeda"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Dari"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
@@ -49,27 +72,27 @@
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Induk"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
@@ -81,23 +104,23 @@
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Skenario"
+msgstr ""
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "UUID"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Aktivitas"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
@@ -115,29 +138,106 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Model"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nama"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
@@ -157,20 +257,20 @@
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
 msgstr ""
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Pihak"
+msgstr ""
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Skenario"
+msgstr ""
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
 msgstr ""
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
@@ -224,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -259,15 +367,15 @@
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Rancangan"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
 msgstr ""
 
 msgctxt ""
@@ -319,15 +427,15 @@
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Rancangan"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
@@ -345,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -408,51 +528,67 @@
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
 msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Aktivitas"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Skenario"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Dibatalkan"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Rancangan"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Sunting"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
@@ -464,12 +600,24 @@
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Waktu"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/it.po` & `trytond_marketing_automation-7.2.0/locale/hu.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,197 +1,294 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Attività"
+msgstr ""
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Azione"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Figlio"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Condizione"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Ritardo"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-mail cliccate"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Da"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-mail aperte"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Modello E-mail"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "Titolo E-mail"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Evento"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negativo"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
 msgstr ""
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Bloccato"
+msgstr ""
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr ""
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "UUID"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Attività"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "A"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "E-mail aperte"
+msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Stato"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Attività"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Dominio"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Modello"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Stato"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Annulla l'iscrizione"
+msgstr ""
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Automazione Marketing disiscrivi"
+msgstr ""
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
 msgstr ""
 
-#, fuzzy
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr ""
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
 msgstr ""
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Dopo quanto tempo l'azione dovrebbe essere eseguita."
+msgstr ""
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr "Lasciare vuoto per il valore definito nel file di configurazione."
+msgstr ""
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
 
@@ -202,87 +299,93 @@
 msgstr ""
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Spunta per eseguire l'attività se l'evento non si è verificato entro la fine"
-" del ritardo."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Attività"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Scenari"
+msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Automazione Marketing disiscrivi"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Tutti"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Fatto"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "In attesa"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Tutti"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Bozza"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Fermato"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
 
@@ -318,58 +421,69 @@
 msgid "E-Mail Clicked"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Bloccato"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Bozza"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "Scenari"
+msgstr ""
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
 msgstr ""
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Annulla l'iscrizione"
+msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
 
 msgctxt "report:marketing.automation.unsubscribe:"
@@ -386,15 +500,15 @@
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
 msgstr ""
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "Invia E-mail"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
 msgstr ""
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
@@ -414,69 +528,96 @@
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
 msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Attività"
+msgstr ""
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Fatto"
+msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "In attesa"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Bozza"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "Fermato"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Dopo"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Modifica"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Se"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Modello:"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Titolo:"
+msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Tempo"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Automazione Marketing disiscrivi"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_marketing_automation-7.0.0/locale/lo.po` & `trytond_marketing_automation-7.2.0/locale/lo.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/lt.po` & `trytond_marketing_automation-7.2.0/locale/lt.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/nl.po` & `trytond_marketing_automation-7.2.0/locale/ca.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,496 +1,668 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Record"
+msgstr "Registre"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Actie"
+msgstr "Acció"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Onderliggende niveaus"
+msgstr "Fills"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Voorwaarde"
+msgstr "Condició"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Vertraging"
+msgstr "Retard"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "Correus electrònics clicats"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "Correus electrònics clicats"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "Correus electrònics clicats"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-mails Geklikt"
+msgstr "Correus electrònics clicats"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Van"
+msgstr "De"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "Correus electrònics oberts"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "Correus electrònics oberts"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-mails geopend"
+msgstr "Correus electrònics oberts"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "Email sjabloon"
+msgstr "Plantilla de correu electrònic"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "E-mail titel"
+msgstr "Títol del correu electrònic"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Evenement"
+msgstr "Esdeveniment"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Naam"
+msgstr "Nom"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negatief"
+msgstr "Negatiu"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "Op"
+msgstr "A"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Bovenliggend niveau"
+msgstr "Pare"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Bovenliggende actie (parent)"
+msgstr "Acció pare"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "geblokkeerd"
+msgstr "Bloquejat"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Record"
+msgstr "Registre"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
-msgstr "UUID"
+msgstr "Identificador únic universal"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Activiteit actie"
+msgstr "Acció d'activitat"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "Op"
+msgstr "A"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correus electrònics clicats"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correus electrònics oberts"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Record"
+msgstr "Registre"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Estat"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Activitat"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Acció d'activitat"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "Correus electrònics clicats"
+
+#, fuzzy
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "Correus electrònics clicats"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "Correus electrònics clicats"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "Correus electrònics oberts"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "Correus electrònics oberts"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr "Registres"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Data de modificació"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Bloquejat"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr "Registres"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Registres bloquejats"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Escenari"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Activiteiten"
+msgstr "Activitats"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Bloquejat"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "Bloquejat"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domein (domain)"
+msgstr "Domini"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Naam"
+msgstr "Nom"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Geblokkeerde records"
+msgstr "Registres bloquejats"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Estat"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Afmelden mogelijk"
+msgstr "Donar-se de baixa"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Relatie"
+msgstr "Tercer de màrqueting"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr "Marketing Abonnement opgezegd"
+msgstr "Escenàris d'automatització de màrqueting no subscrits"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Relatie"
+msgstr "Tercer"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Relatie"
+msgstr "Tercer de màrqueting"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"De PYSON-expressie waaraan het record moet voldoen om de activiteit te kunnen uitvoeren.\n"
-"Het record wordt vertegenwoordigd door \"self\"."
+"L'expressió PYSON que el registre ha de complir per tal d'executar-se l'activitat.\n"
+"El registre s'expressa amb \"self\"."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Na hoeveel tijd moet de actie worden uitgevoerd."
+msgstr "Desprès de quant temps s'hauria d'executar l'acció."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr ""
-"Laat leeg om de waarde te gebruiken die gedefinieerd is in het "
-"configuratiebestand."
+msgstr "Deixa buit per utilizar el valor definit al fitxer de configuració."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"De HTML-inhoud van de e-mail.\n"
-"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
+"El contingut HTML del correu electrònic.\n"
+"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Het onderwerp van de e-mail.\n"
-"De Genshi-syntaxis kan gebruikt worden met 'record' in de evaluatiecontext."
+"L'assumpte del correu electrònic.\n"
+"La sintaxi Genshi es pot fer servir amb 'record' al context d'avaluació."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Schakel het selectievakje in om de activiteit uit te voeren als het "
-"evenement niet is gebeurd aan het einde van de vertraging."
+"Marcar per executar l'activitat si l'esdeveniment no s'ha executat al acabar"
+" el retard."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"Een PYSON-domein dat wordt gebruikt om records te filteren die geldig zijn "
-"voor dit scenario."
+"Un domini PYSON utilitzat per filtrar registres vàlid per aquest escenari."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr ""
-"Indien aangevinkt worden de relaties ook uitgeschreven uit het scenario."
+msgstr "Si es marca els tercer també es de-suscribeixen de l'escenari."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Activiteiten"
+msgstr "Activitats"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "E-mails"
+msgstr "Correus electrònics"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Activiteiten opnemen"
+msgstr "Activitats del registre"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Records"
+msgstr "Registres"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Acció d'activitat"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Escenari"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "scenario's"
+msgstr "Escenaris"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Marketing Automatizerings Abonnement opzeggen"
+msgstr "Baixa d'automatització de màrqueting"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Geannuleerd"
+msgstr "Cancel·lat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Finalitzat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "In afwachting"
+msgstr "En espera"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Esborrany"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "in uitvoering"
+msgstr "En execució"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "gestopt"
+msgstr "Aturat"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Ongeldige voorwaarde \"%(condition)s\" in activiteit \"%(activity)s\" met "
-"uitzondering \"%(exception)s\"."
+"Condició no vàlida \"%(condition)s\" a l'activitat \"%(activity)s\" amb "
+"l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ongeldige e-mailsjabloon in activiteit \"%(activity s\" met uitzondering "
-"\"%(exception)s\"."
+"Plantilla de correu electrònic no vàlida a l'activitat \"%(activity)s\" amb "
+"l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ongeldige e-mailtitel in activiteit \"%(activity s\" met uitzondering "
-"\"%(exception)s\"."
+"Ttítol de la plantilla de correu electrònic no vàlida a l'activitat "
+"\"%(activity)s\" amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "Recordactiviteit moet uniek zijn per record en activiteit."
+msgstr "L'activitat del registre ha de ser única per registre i activitat."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "Record moet uniek zijn per scenario."
+msgstr "El registre ha de ser únic per cada escenari."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "UUID van het record moet uniek zijn."
+msgstr "L'UUID del registre ha de ser únic."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Ongeldig domein in scenario \"%(scenario)s\" met uitzondering "
+"Domini no vàlid a l'escenari \"%(scenario)s\" amb l'excepció "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correu electrònic clicat"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correu electrònic obert"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr "Blokkeer"
+msgstr "Bloqueja"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Esborrany"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr "uitvoeren"
+msgstr "Executa"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr "stop"
+msgstr "Atura"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr "scenario's"
+msgstr "Escenaris"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr "Marketing activiteit"
+msgstr "Activitat de màrqueting"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr "Marketingrecord"
+msgstr "Registre de màrqueting"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr "Marketingrecordactiviteit"
+msgstr "Activitat del registre de màrqueting"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Activitat del registre de màrqueting"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Automatització de màrqueting"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Escenàris d'automatització de màrqueting no subscrits"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr "Marketingscenario"
+msgstr "Escenari de màrqueting"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr "Relatie Uitschrijf Scenario"
+msgstr "Escenaris de-suscrits del tercer"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr "Afmelden"
+msgstr "Donar-se de baixa"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
-"Het spijt ons u te zien gaan. Onze excuses als we uw inbox vervuild hebben ."
+"Sentim veure't marxar, i ens disculpem si hem aclaparat la teva safata "
+"d'entrada."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr "U bent uitgeschreven"
+msgstr "T'has donat de baixa"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr "U bent succesvol afgemeld voor dit soort e-mail."
+msgstr "T'has donat de baixa amb èxit d'aquest tipus de correu electrònic."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr "Marketingactiviteit verwerken"
+msgstr "Processar activitats de màrqueting"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr "Trigger Marketing Scenario's"
+msgstr "Executar disparadors del escenaris de màrqueting"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr "E-mail verzenden"
+msgstr "Correu electrònic enviat"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correu electrònic clicat"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correu electrònic obert"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr "E-mail Geklikt"
+msgstr "Correu electrònic clicat"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr "E-mail niet aangeklikt"
+msgstr "Correu electrònic no clicat"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr "E-mail niet geopend"
+msgstr "Correu electrònic no obert"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr "E-mails geopend"
+msgstr "Correu electrònic obert"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr "Activiteit"
+msgstr "Activitat"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr "Scenario"
+msgstr "Escenari"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr "Geannuleerd"
+msgstr "Cancel·lada"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Finalitzada"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
-msgstr "In afwachting"
+msgstr "En espera"
+
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Retard"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Esborrany"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr "in uitvoering"
+msgstr "En execució"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
-msgstr "gestopt"
+msgstr "Aturat"
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr "Na"
+msgstr "Desprès"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr "Bewerk"
+msgstr "Edita"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr "Als"
+msgstr "Si"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr "Op"
+msgstr "A"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr "Sjabloon:"
+msgstr "Plantilla:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr "Titel:"
+msgstr "Títol:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
-msgstr "Tijd"
+msgstr "Hora"
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr "Marketing Abonnement Opzeggen"
+msgstr "Automatització de màrqueting"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_marketing_automation-7.0.0/locale/pl.po` & `trytond_marketing_automation-7.2.0/locale/pl.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/pt.po` & `trytond_marketing_automation-7.2.0/locale/pt.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/ro.po` & `trytond_marketing_automation-7.2.0/locale/ru.po`

 * *Files 17% similar despite different names*

```diff
@@ -8,36 +8,60 @@
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Copii"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -60,15 +84,15 @@
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Părinte"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
@@ -114,21 +138,98 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domeniu"
+msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_marketing_automation-7.0.0/locale/ru.po` & `trytond_marketing_automation-7.2.0/locale/tr.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/sl.po` & `trytond_marketing_automation-7.2.0/locale/de.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,492 +1,670 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:ir.email,marketing_automation_activity:"
 msgid "Activity"
-msgstr "Aktivnost"
+msgstr "Aktivität"
 
 msgctxt "field:ir.email,marketing_automation_record:"
 msgid "Record"
-msgstr "Zapis"
+msgstr "Datensatz"
 
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
-msgstr "Ukrep"
+msgstr "Aktion"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
-msgstr "Podukrepi"
+msgstr "Untergeordnet"
 
 msgctxt "field:marketing.automation.activity,condition:"
 msgid "Condition"
-msgstr "Pogoj"
+msgstr "Bedingung"
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
-msgstr "Zakasnitev"
+msgstr "Verzögerung"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "Angeklickte E-Mail"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr "Angeklickte E-Mail"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "Angeklickte E-Mail"
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
-msgstr "E-poštni kliki"
+msgstr "Angeklickte E-Mails"
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
-msgstr "Od"
+msgstr "Von"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "Geöffnete E-Mail"
+
+#, fuzzy
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr "Geöffnete E-Mail"
 
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
-msgstr "E-pošta odprta"
+msgstr "Geöffnete E-Mails"
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
-msgstr "E-poštna predloga"
+msgstr "E-Mail Vorlage"
 
 msgctxt "field:marketing.automation.activity,email_title:"
 msgid "E-Mail Title"
-msgstr "E-poštna zadeva"
+msgstr "E-Mail Titel"
 
 msgctxt "field:marketing.automation.activity,event:"
 msgid "Event"
-msgstr "Dogodek"
+msgstr "Ereignis"
 
 msgctxt "field:marketing.automation.activity,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "Name"
 
 msgctxt "field:marketing.automation.activity,negative:"
 msgid "Negative"
-msgstr "Negativno"
+msgstr "Negativ"
 
 msgctxt "field:marketing.automation.activity,on:"
 msgid "On"
-msgstr "Na"
+msgstr "Bei"
 
 msgctxt "field:marketing.automation.activity,parent:"
 msgid "Parent"
-msgstr "Matični ukrep"
+msgstr "Übergeordnet"
 
 msgctxt "field:marketing.automation.activity,parent_action:"
 msgid "Parent Action"
-msgstr "Matični ukrep"
+msgstr "Übergeordnete Aktion"
 
 msgctxt "field:marketing.automation.activity,record_count:"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Datensätze"
 
 msgctxt "field:marketing.automation.record,blocked:"
 msgid "Blocked"
-msgstr "Blokiran"
+msgstr "Gesperrt"
 
 msgctxt "field:marketing.automation.record,record:"
 msgid "Record"
-msgstr "Zapis"
+msgstr "Datensatz"
 
 msgctxt "field:marketing.automation.record,scenario:"
 msgid "Scenario"
-msgstr "Scenarij"
+msgstr "Szenario"
 
 msgctxt "field:marketing.automation.record,uuid:"
 msgid "UUID"
 msgstr "UUID"
 
 msgctxt "field:marketing.automation.record.activity,activity:"
 msgid "Activity"
-msgstr "Aktivnost"
+msgstr "Aktivität"
 
 msgctxt "field:marketing.automation.record.activity,activity_action:"
 msgid "Activity Action"
-msgstr "Ukrep aktivnosti"
+msgstr "Aktivität Aktion"
 
 msgctxt "field:marketing.automation.record.activity,at:"
 msgid "At"
-msgstr "Ob"
+msgstr "Um"
 
 msgctxt "field:marketing.automation.record.activity,email_clicked:"
 msgid "E-Mail Clicked"
-msgstr "E-poštni kliki"
+msgstr "Angeklickte E-Mail"
 
 msgctxt "field:marketing.automation.record.activity,email_opened:"
 msgid "E-Mail Opened"
-msgstr "E-pošta odprta"
+msgstr "Geöffnete E-Mail"
 
 msgctxt "field:marketing.automation.record.activity,record:"
 msgid "Record"
-msgstr "Zapis"
+msgstr "Datensatz"
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr "Status"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr "Aktivität"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr "Aktivität Aktion"
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr "Angeklickte E-Mail"
+
+#, fuzzy
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr "Angeklickte E-Mail"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr "Angeklickte E-Mails"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr "Geöffnete E-Mail"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr "Geöffnete E-Mails"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr "Datensätze"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr "Zuletzt geändert"
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Gesperrt"
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr "Datensätze"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr "Blockierte Datensätze"
+
+#, fuzzy
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr "Szenario"
 
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
-msgstr "Aktivnosti"
+msgstr "Aktivitäten"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr "Gesperrt"
+
+#, fuzzy
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr "Gesperrt"
 
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
-msgstr "Domena"
+msgstr "Wertebereich (Domain)"
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
-msgstr "Model"
+msgstr "Modell"
 
 msgctxt "field:marketing.automation.scenario,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "Name"
 
 msgctxt "field:marketing.automation.scenario,record_count:"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Datensätze"
 
 msgctxt "field:marketing.automation.scenario,record_count_blocked:"
 msgid "Records Blocked"
-msgstr "Blokirani zapisi"
+msgstr "Blockierte Datensätze"
 
 msgctxt "field:marketing.automation.scenario,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr "Status"
 
 msgctxt "field:marketing.automation.scenario,unsubscribable:"
 msgid "Unsubscribable"
-msgstr "Odjava"
+msgstr "Abmeldbar"
 
 msgctxt "field:party.party,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing Partner"
+msgstr "Marketing Partei"
 
 msgctxt "field:party.party,marketing_scenario_unsubscribed:"
 msgid "Marketing Automation Scenario Unsubscribed"
-msgstr ""
+msgstr "Marketingautomatisierungsszenario abgemeldet"
 
 msgctxt "field:party.party-unsubscribed-marketing.automation.scenario,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr "Partei"
 
 msgctxt ""
 "field:party.party-unsubscribed-marketing.automation.scenario,scenario:"
 msgid "Scenario"
-msgstr "Scenarij"
+msgstr "Szenario"
 
 msgctxt "field:sale.sale,marketing_party:"
 msgid "Marketing Party"
-msgstr "Marketing partner"
+msgstr "Marketing Partei"
 
 msgctxt "help:marketing.automation.activity,condition:"
 msgid ""
 "The PYSON statement that the record must match in order to execute the activity.\n"
 "The record is represented by \"self\"."
 msgstr ""
-"Izraz PYSON, s katerim se mora zapis ujemati, da se aktivnost izvaja.\n"
-"Zapis je predstavljen s \"self\"."
+"Der PYSON Ausdruck, dem der Datensatz entsprechen muss, damit die Aktivität ausgeführt wird.\n"
+"Der Datensatz wird durch \"self\" repräsentiert."
 
 msgctxt "help:marketing.automation.activity,delay:"
 msgid "After how much time the action should be executed."
-msgstr "Po koliko časa naj bo ukrep izveden."
+msgstr "Nach welcher Zeit die Aktion ausgeführt werden soll."
 
 msgctxt "help:marketing.automation.activity,email_from:"
 msgid "Leave empty to use the value defined in the configuration file."
-msgstr ""
-"Pustite prazno, da uporabite vrednost opredeljeno v konfiguracijski "
-"datoteki."
+msgstr "Leer lassen, um den Wert aus der Konfigurationsdatei zu verwenden."
 
 msgctxt "help:marketing.automation.activity,email_template:"
 msgid ""
 "The HTML content of the E-mail.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"HTML vsebina e-pošte.\n"
-"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
+"Der HTML Content der E-Mail.\n"
+"Die Genshi Syntax kann mit 'record' im Evaluierungskontext verwendet werden."
 
 msgctxt "help:marketing.automation.activity,email_title:"
 msgid ""
 "The subject of the email.\n"
 "The Genshi syntax can be used with 'record' in the evaluation context."
 msgstr ""
-"Zadeva te e-pošte.\n"
-"Lahko uporabite Genshi sintakso z 'record' v kontekstu vrednotenja."
+"Der Betreff der E-Mail.\n"
+"Die Genshi Syntax kann mit 'record' im Evaluierungskontext verwendet werden."
 
 msgctxt "help:marketing.automation.activity,negative:"
 msgid ""
 "Check to execute the activity if the event has not happened by the end of "
 "the delay."
 msgstr ""
-"Označite, če želite izvesti aktivnost, v kolikor do dogodka ni prišlo v "
-"opredeljenem zamiku."
+"Aktivieren um die Aktivität auszulösen, wenn das Ereignis nach Ablauf des "
+"Verzögerungszeitraums noch nicht eingetreten ist."
 
 msgctxt "help:marketing.automation.scenario,domain:"
 msgid "A PYSON domain used to filter records valid for this scenario."
 msgstr ""
-"PYSON domena, ki se uporabi za filtriranje zapisov, ki so veljavno za ta "
-"scenarij."
+"Ein PYSON Wertebereich (Domain) zum Filtern der Datensätze, die diesem "
+"Szenario entsprechen."
 
 msgctxt "help:marketing.automation.scenario,unsubscribable:"
 msgid "If checked parties are also unsubscribed from the scenario."
-msgstr "Označite, da se partner lahko odjavi s tega scenarija."
+msgstr "Wenn ausgewählt, dann werden Parteien auch vom Szenario abgemeldet."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
-msgstr "Aktivnosti"
+msgstr "Aktivitäten"
 
 msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
 msgid "E-mails"
-msgstr "E-pošte"
+msgstr "E-Mails"
 
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
-msgstr "Zapisi aktivnosti"
+msgstr "Datensatzaktivitäten"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
-msgstr "Zapisi"
+msgstr "Datensätze"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr "Aktivität Aktion"
+
+#, fuzzy
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr "Szenario"
 
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
-msgstr "Scenariji"
+msgstr "Szenarien"
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
-msgstr "Odjave automatizacije marketinga"
+msgstr "Abmeldung Marketingautomatisierung"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_all"
 msgid "All"
-msgstr "Vse"
+msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Preklicano"
+msgstr "Annulliert"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_done"
 msgid "Done"
-msgstr "Zaključeno"
+msgstr "Erledigt"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_record_activity_form_domain_waiting"
 msgid "Waiting"
-msgstr "V čakanju"
+msgstr "Wartend"
 
 msgctxt "model:ir.action.act_window.domain,name:act_scenario_form_domain_all"
 msgid "All"
-msgstr "Vse"
+msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_draft"
 msgid "Draft"
-msgstr "Osnutek"
+msgstr "Entwurf"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_running"
 msgid "Running"
-msgstr "V izvajanju"
+msgstr "In Ausführung"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_scenario_form_domain_stopped"
 msgid "Stopped"
-msgstr "Ustavljeno"
+msgstr "Gestoppt"
 
 msgctxt "model:ir.message,text:msg_activity_invalid_condition"
 msgid ""
 "Invalid condition \"%(condition)s\" in activity \"%(activity)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"Neveljaven pogojo \"%(condition)s\" v aktivnosti \"%(activity)s\" z napako "
-"\"%(exception)s\"."
+"Ungültige Bedingung \"%(condition)s\" in Aktiviät \"%(activity)s\" mit "
+"Fehler \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_template"
 msgid ""
 "Invalid e-mail template in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Neveljavna e-poštna predloga v aktivnosti \"%(activity)s\" z napako "
+"Ungültige E-Mail Vorlage in Aktivität \"%(activity)s\" mit Fehler "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_invalid_email_title"
 msgid ""
 "Invalid e-mail title in activity \"%(activity)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Neveljavna e-poštna zadeva v aktivnosti \"%(activity)s\" z napako "
+"Ungültiger E-Mail Betreff in Aktivität \"%(activity)s\" mit Fehler "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_activity_record_unique"
 msgid "Record Activity must be unique by record and activity."
-msgstr "Zapis aktivnosti mora biti edinstven po zapisu in aktivnosti."
+msgstr ""
+"Eine Datensatzaktivität kann es je Datensatz und Aktivität nur einmal geben."
 
 msgctxt "model:ir.message,text:msg_record_scenario_record_unique"
 msgid "Record must be unique by scenario."
-msgstr "Zapis mora biti edinstven po scenariju."
+msgstr "Es kann je Szenario nur einen Datensatz geben."
 
 msgctxt "model:ir.message,text:msg_record_uuid_unique"
 msgid "UUID of record must be unique."
-msgstr "UUID zapisa mora biti edinstven."
+msgstr "Die UUID des Datensatzes existiert bereits."
 
 msgctxt "model:ir.message,text:msg_scenario_invalid_domain"
 msgid "Invalid domain in scenario \"%(scenario)s\" with exception \"%(exception)s\"."
 msgstr ""
+"Ungültiger Wertebereich (Domain) in Szenario \"%(scenario)s\" mit Fehler "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_clicked_button"
 msgid "E-Mail Clicked"
-msgstr ""
+msgstr "E-Mail angeklickt"
 
 msgctxt "model:ir.model.button,string:record_activity_on_email_opened_button"
 msgid "E-Mail Opened"
-msgstr ""
+msgstr "E-Mail geöffnet"
 
 msgctxt "model:ir.model.button,string:record_block_button"
 msgid "Block"
-msgstr ""
+msgstr "Gesperrt"
 
 msgctxt "model:ir.model.button,string:scenario_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Entwurf"
 
 msgctxt "model:ir.model.button,string:scenario_run_button"
 msgid "Run"
-msgstr ""
+msgstr "Ausführen"
 
 msgctxt "model:ir.model.button,string:scenario_stop_button"
 msgid "Stop"
-msgstr ""
+msgstr "Stopp"
 
 msgctxt "model:ir.ui.menu,name:menu_scenario_form"
 msgid "Scenarios"
-msgstr ""
+msgstr "Szenarien"
 
 msgctxt "model:marketing.automation.activity,name:"
 msgid "Marketing Activity"
-msgstr ""
+msgstr "Marketingaktivität"
 
 msgctxt "model:marketing.automation.record,name:"
 msgid "Marketing Record"
-msgstr ""
+msgstr "Marketingdatensatz"
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
-msgstr ""
+msgstr "Marketing Datensatzaktivität"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr "Marketing Datensatzaktivität"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr "Marketingautomatisierung"
+
+#, fuzzy
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr "Marketingautomatisierungsszenario abgemeldet"
 
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
-msgstr ""
+msgstr "Marketing Szenario"
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
-msgstr ""
+msgstr "Partei Abmelden Szenario"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "Unsubscribe"
-msgstr ""
+msgstr "Abmelden"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid ""
 "We are sorry to see you go, and apologize if we have overwhelmed your inbox."
 msgstr ""
+"Wir bedauern Ihre Abmeldung und entschuldigen uns sofern wir Ihren "
+"Posteingang überflutet haben sollten."
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You are unsubscribed"
-msgstr ""
+msgstr "Sie sind abgemeldet"
 
 msgctxt "report:marketing.automation.unsubscribe:"
 msgid "You have been successfully unsubscribed from this kind of email."
-msgstr ""
+msgstr "Sie haben sich für diese Art von E-Mails erfolgreich abgemeldet."
 
 msgctxt "selection:ir.cron,method:"
 msgid "Process Marketing Activity"
-msgstr ""
+msgstr "Marketingaktivitäten ausführen"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Trigger Marketing Scenarios"
-msgstr ""
+msgstr "Marketingszenarios auslösen"
 
 msgctxt "selection:marketing.automation.activity,action:"
 msgid "Send E-Mail"
-msgstr ""
+msgstr "E-Mail senden"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Clicked"
-msgstr ""
+msgstr "E-Mail angeklickt"
 
 msgctxt "selection:marketing.automation.activity,event:"
 msgid "E-Mail Opened"
-msgstr ""
+msgstr "E-Mail geöffnet"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Clicked"
-msgstr ""
+msgstr "E-Mail angeklickt"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Clicked"
-msgstr ""
+msgstr "E-Mail nicht angeklickt"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Not Opened"
-msgstr ""
+msgstr "E-Mail nicht geöffnet"
 
 msgctxt "selection:marketing.automation.activity,on:"
 msgid "E-Mail Opened"
-msgstr ""
+msgstr "E-Mail geöffnet"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Activity"
-msgstr ""
+msgstr "Aktivität"
 
 msgctxt "selection:marketing.automation.activity,parent:"
 msgid "Scenario"
-msgstr ""
+msgstr "Szenario"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Annulliert"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Done"
-msgstr ""
+msgstr "Erledigt"
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
+msgstr "Wartend"
+
+#, fuzzy
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr "Verzögerung"
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Entwurf"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
-msgstr ""
+msgstr "In Ausführung"
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
+msgstr "Gestoppt"
+
+msgctxt "view:marketing.automation.activity:"
+msgid "%"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "After"
-msgstr ""
+msgstr "Nach"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
-msgstr ""
+msgstr "Bearbeiten"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "If"
-msgstr ""
+msgstr "Wenn"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "On"
-msgstr ""
+msgstr "Bei"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Template:"
-msgstr ""
+msgstr "Vorlage:"
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Title:"
-msgstr ""
+msgstr "Titel:"
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
+msgstr "Zeit"
+
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
 msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
-msgstr ""
+msgstr "Marketingautomatisierung"
```

### Comparing `trytond_marketing_automation-7.0.0/locale/tr.po` & `trytond_marketing_automation-7.2.0/locale/uk.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/locale/uk.po` & `trytond_marketing_automation-7.2.0/locale/zh_CN.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,46 @@
 msgid "Condition"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,delay:"
 msgid "Delay"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_rate_trend:"
+msgid "E-mail Click Rate Trend"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_click_through_rate_trend:"
+msgid "E-mail Click-Through Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_clicked:"
 msgid "E-Mails Clicked"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_from:"
 msgid "From"
 msgstr ""
 
+msgctxt "field:marketing.automation.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.activity,email_open_rate_trend:"
+msgid "E-mail Open Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,email_opened:"
 msgid "E-Mails Opened"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,email_template:"
 msgid "E-Mail Template"
 msgstr ""
@@ -114,18 +138,95 @@
 msgid "Record"
 msgstr ""
 
 msgctxt "field:marketing.automation.record.activity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:marketing.automation.reporting.activity,activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,activity_action:"
+msgid "Activity Action"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_click_rate:"
+msgid "E-mail Click Rate"
+msgstr ""
+
+msgctxt ""
+"field:marketing.automation.reporting.activity,email_click_through_rate:"
+msgid "E-mail Click-Through Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_clicked:"
+msgid "E-Mails Clicked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_open_rate:"
+msgid "E-mail Open Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,email_opened:"
+msgid "E-Mails Opened"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.activity,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,from_date:"
+msgid "From Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,period:"
+msgid "Period"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.context,to_date:"
+msgid "To Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,date:"
+msgid "Date"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count:"
+msgid "Records"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,record_count_blocked:"
+msgid "Records Blocked"
+msgstr ""
+
+msgctxt "field:marketing.automation.reporting.scenario,scenario:"
+msgid "Scenario"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,activities:"
 msgid "Activities"
 msgstr ""
 
+msgctxt "field:marketing.automation.scenario,block_rate:"
+msgid "Block Rate"
+msgstr ""
+
+msgctxt "field:marketing.automation.scenario,block_rate_trend:"
+msgid "Block Rate Trend"
+msgstr ""
+
 msgctxt "field:marketing.automation.scenario,domain:"
 msgid "Domain"
 msgstr ""
 
 msgctxt "field:marketing.automation.scenario,model:"
 msgid "Model"
 msgstr ""
@@ -223,14 +324,22 @@
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_reporting_activity"
+msgid "Activity Reporting"
+msgstr ""
+
+msgctxt "model:ir.action,name:act_reporting_scenario"
+msgid "Scenario Reporting"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_scenario_form"
 msgid "Scenarios"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_unsubscribe"
 msgid "Marketing Automation Unsubscribe"
 msgstr ""
@@ -344,14 +453,26 @@
 msgid "Marketing Record"
 msgstr ""
 
 msgctxt "model:marketing.automation.record.activity,name:"
 msgid "Marketing Record Activity"
 msgstr ""
 
+msgctxt "model:marketing.automation.reporting.activity,name:"
+msgid "Marketing Automation Reporting Activity"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.context,name:"
+msgid "Marketing Automation Reporting Context"
+msgstr ""
+
+msgctxt "model:marketing.automation.reporting.scenario,name:"
+msgid "Marketing Automation Reporting Scenario"
+msgstr ""
+
 msgctxt "model:marketing.automation.scenario,name:"
 msgid "Marketing Scenario"
 msgstr ""
 
 msgctxt "model:party.party-unsubscribed-marketing.automation.scenario,name:"
 msgid "Party Unsubscribed Scenario"
 msgstr ""
@@ -425,27 +546,43 @@
 msgid "Done"
 msgstr ""
 
 msgctxt "selection:marketing.automation.record.activity,state:"
 msgid "Waiting"
 msgstr ""
 
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Day"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Month"
+msgstr ""
+
+msgctxt "selection:marketing.automation.reporting.context,period:"
+msgid "Year"
+msgstr ""
+
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Draft"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Running"
 msgstr ""
 
 msgctxt "selection:marketing.automation.scenario,state:"
 msgid "Stopped"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.activity:"
 msgid "After"
 msgstr ""
 
 msgctxt "view:marketing.automation.activity:"
 msgid "Edit"
 msgstr ""
 
@@ -465,10 +602,22 @@
 msgid "Title:"
 msgstr ""
 
 msgctxt "view:marketing.automation.record.activity:"
 msgid "Time"
 msgstr ""
 
+msgctxt "view:marketing.automation.reporting.activity:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.reporting.scenario:"
+msgid "%"
+msgstr ""
+
+msgctxt "view:marketing.automation.scenario:"
+msgid "%"
+msgstr ""
+
 msgctxt "view:party.party:"
 msgid "Marketing Automation"
 msgstr ""
```

### Comparing `trytond_marketing_automation-7.0.0/marketing_automation.py` & `trytond_marketing_automation-7.2.0/marketing_automation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 import logging
 import time
 import uuid
 from collections import defaultdict
-from email.header import Header
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-from email.utils import formataddr, getaddresses
+from email.message import EmailMessage
+from functools import partial
 from urllib.parse import (
     parse_qsl, quote, urlencode, urljoin, urlsplit, urlunsplit)
 
+from dateutil.relativedelta import relativedelta
+
 try:
     import html2text
 except ImportError:
     html2text = None
 
 from genshi.core import END, START, Attrs, QName
-from genshi.template import MarkupTemplate, TextTemplate
+from genshi.template import MarkupTemplate
+from genshi.template import TemplateError as GenshiTemplateError
+from genshi.template import TextTemplate
 from sql import Literal
 from sql.aggregate import Count
 
+try:
+    import pygal
+except ImportError:
+    pygal = None
+
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
     EvalEnvironment, Index, ModelSQL, ModelView, Unique, Workflow, dualmethod,
     fields)
 from trytond.pool import Pool
 from trytond.pyson import Eval, If, PYSONDecoder, TimeDelta
 from trytond.report import Report
-from trytond.sendmail import SMTPDataManager, sendmail_transactional
-from trytond.tools import grouped_slice, reduce_ids
-from trytond.tools.email_ import convert_ascii_email, set_from_header
+from trytond.sendmail import SMTPDataManager, send_message_transactional
+from trytond.tools import grouped_slice, pairwise_longest, reduce_ids
+from trytond.tools.email_ import format_address, has_rcpt, set_from_header
 from trytond.transaction import Transaction
 from trytond.url import http_host
 from trytond.wsgi import Base64Converter
 
 from .exceptions import ConditionError, DomainError, TemplateError
 from .mixin import MarketingAutomationMixin
 
@@ -48,35 +55,84 @@
 
 USE_SSL = bool(config.get('ssl', 'certificate'))
 URL_BASE = config.get('marketing', 'automation_base', default=http_host())
 URL_OPEN = urljoin(URL_BASE, '/m/empty.gif')
 logger = logging.getLogger(__name__)
 
 
-def _formataddr(name, email):
-    if name:
-        name = str(Header(name, 'utf-8'))
-    return formataddr((name, convert_ascii_email(email)))
-
-
-class Scenario(Workflow, ModelSQL, ModelView):
+def trend_mixin(model_name, field_name):
+    class TrendMixin:
+        __slots__ = ()
+
+        def get_trend(self, name):
+            name = name[:-len('_trend')]
+            if pygal:
+                chart = pygal.Line()
+                chart.add('', [
+                        getattr(ts, name, 0) or 0
+                        for ts in self.trends])
+                return chart.render_sparktext()
+
+        @property
+        def trends(self):
+            pool = Pool()
+            Model = pool.get(model_name)
+            Date = pool.get('ir.date')
+
+            delta = self._trend_period_delta()
+            date = Date.today()
+            date -= 10 * delta
+
+            records = Model.search([
+                    ('date', '>=', date),
+                    (field_name, '=', self.id),
+                    ],
+                order=[('date', 'ASC')])
+            for record, next_record in pairwise_longest(records):
+                yield record
+                if delta and next_record:
+                    date = record.date + delta
+                    while date < next_record.date:
+                        yield None
+                        date += delta
+
+        @classmethod
+        def _trend_period_delta(cls):
+            context = Transaction().context
+            return {
+                'year': relativedelta(years=1),
+                'month': relativedelta(months=1),
+                'day': relativedelta(days=1),
+                }.get(context.get('period', 'month'))
+    return TrendMixin
+
+
+class Scenario(
+        trend_mixin('marketing.automation.reporting.scenario', 'scenario'),
+        Workflow, ModelSQL, ModelView):
     "Marketing Scenario"
     __name__ = 'marketing.automation.scenario'
 
     name = fields.Char("Name", translate=True)
     model = fields.Selection('get_models', "Model", required=True)
     domain = fields.Char(
         "Domain", required=True,
         help="A PYSON domain used to filter records valid for this scenario.")
     activities = fields.One2Many(
         'marketing.automation.activity', 'parent', "Activities")
     record_count = fields.Function(
         fields.Integer("Records"), 'get_record_count')
     record_count_blocked = fields.Function(
         fields.Integer("Records Blocked"), 'get_record_count')
+    block_rate = fields.Function(
+        fields.Float("Block Rate"),
+        'get_rate')
+    block_rate_trend = fields.Function(
+        fields.Char("Block Rate Trend"),
+        'get_trend')
     unsubscribable = fields.Boolean(
         "Unsubscribable",
         help="If checked parties are also unsubscribed from the scenario.")
     state = fields.Selection([
             ('draft', "Draft"),
             ('running', "Running"),
             ('stopped', "Stopped"),
@@ -141,15 +197,15 @@
         others = []
         for scenario in scenarios:
             if scenario.state == 'draft':
                 drafts.append(scenario)
             else:
                 others.append(scenario)
 
-        count = {name: dict.fromkeys(map(int, scenarios)) for name in names}
+        count = {name: defaultdict(int) for name in names}
         for sub in grouped_slice(others):
             cursor.execute(*record.select(
                     record.scenario,
                     Count(Literal('*')),
                     Count(Literal('*'), filter_=record.blocked),
                     where=reduce_ids(record.scenario, sub),
                     group_by=record.scenario))
@@ -165,14 +221,23 @@
                 count['record_count'][scenario.id] = Model.search(
                     domain, count=True)
             except Exception:
                 pass
         return count
 
     @classmethod
+    def get_rate(cls, scenarios, names):
+        rates = {name: defaultdict(float) for name in names}
+        for scenario in scenarios:
+            if 'block_rate' in names and scenario.record_count:
+                rates['block_rate'][scenario.id] = round(
+                    scenario.record_count_blocked / scenario.record_count, 2)
+        return rates
+
+    @classmethod
     def validate_fields(cls, scenarios, field_names):
         super().validate_fields(scenarios, field_names)
         cls.check_domain(scenarios)
 
     @classmethod
     def check_domain(cls, scenarios, field_names=None):
         pool = Pool()
@@ -256,15 +321,17 @@
                             and not record.eval(activity.condition)):
                         continue
                     record_activities.append(
                         RecordActivity.get(record, activity))
             RecordActivity.save(record_activities)
 
 
-class Activity(ModelSQL, ModelView):
+class Activity(
+        trend_mixin('marketing.automation.reporting.activity', 'activity'),
+        ModelSQL, ModelView):
     "Marketing Activity"
     __name__ = 'marketing.automation.activity'
 
     name = fields.Char("Name", translate=True, required=True)
     parent = fields.Reference(
         "Parent", [
             ('marketing.automation.scenario', "Scenario"),
@@ -356,14 +423,57 @@
         fields.Integer(
             "E-Mails Clicked",
             states={
                 'invisible': Eval('action') != 'send_email',
                 }),
         'get_record_count')
 
+    email_open_rate = fields.Function(
+        fields.Float(
+            "E-mail Open Rate",
+            states={
+                'invisible': Eval('action') != 'send_email',
+                }),
+        'get_rate')
+    email_open_rate_trend = fields.Function(
+        fields.Char(
+            "E-mail Open Rate Trend",
+            states={
+                'invisible': Eval('action') != 'send_email',
+                }),
+        'get_trend')
+    email_click_rate = fields.Function(
+        fields.Float(
+            "E-mail Click Rate",
+            states={
+                'invisible': Eval('action') != 'send_email',
+                }),
+        'get_rate')
+    email_click_rate_trend = fields.Function(
+        fields.Char(
+            "E-mail Click Rate Trend",
+            states={
+                'invisible': Eval('action') != 'send_email',
+                }),
+        'get_trend')
+    email_click_through_rate = fields.Function(
+        fields.Float(
+            "E-mail Click-Through Rate",
+            states={
+                'invisible': Eval('action') != 'send_email',
+                }),
+        'get_rate')
+    email_click_through_rate_trend = fields.Function(
+        fields.Char(
+            "E-mail Click-Through Rate Trend",
+            states={
+                'invisible': Eval('action') != 'send_email',
+                }),
+        'get_trend')
+
     @classmethod
     def __setup__(cls):
         super().__setup__()
         for name in ['event', 'on']:
             field = getattr(cls, name)
             domain = [(name, '=', None)]
             for parent_action, events in cls._parent_action_events().items():
@@ -431,16 +541,15 @@
     @classmethod
     def get_record_count(cls, activities, names):
         pool = Pool()
         RecordActivity = pool.get('marketing.automation.record.activity')
         record_activity = RecordActivity.__table__()
         cursor = Transaction().connection.cursor()
 
-        count = {name: dict.fromkeys(map(int, activities), 0)
-            for name in names}
+        count = {name: defaultdict(int) for name in names}
         for sub in grouped_slice(activities):
             cursor.execute(*record_activity.select(
                     record_activity.activity,
                     Count(Literal('*'),
                         filter_=record_activity.state == 'done'),
                     Count(Literal('*'), filter_=record_activity.email_opened),
                     Count(Literal('*'), filter_=record_activity.email_clicked),
@@ -452,14 +561,29 @@
                 if 'email_opened' in count:
                     count['email_opened'][id_] = email_opened
                 if 'email_clicked' in count:
                     count['email_clicked'][id_] = email_clicked
         return count
 
     @classmethod
+    def get_rate(cls, activities, names):
+        rates = {name: defaultdict(float) for name in names}
+        for activity in activities:
+            if 'email_open_rate' in names and activity.record_count:
+                rates['email_open_rate'][activity.id] = round(
+                    activity.email_opened / activity.record_count, 2)
+            if 'email_click_rate' in names and activity.record_count:
+                rates['email_click_rate'][activity.id] = round(
+                    activity.email_clicked / activity.record_count, 2)
+            if 'email_click_through_rate' in names and activity.email_opened:
+                rates['email_click_through_rate'][activity.id] = round(
+                    activity.email_clicked / activity.email_opened, 2)
+        return rates
+
+    @classmethod
     def validate_fields(cls, activities, fields_names):
         super().validate_fields(activities, fields_names)
         for activity in activities:
             activity.check_condition(fields_names)
             activity.check_email_title(fields_names)
             activity.check_email_template(fields_names)
 
@@ -480,29 +604,29 @@
     def check_email_template(self, fields_names=None):
         if fields_names and 'email_template' not in fields_names:
             return
         if not self.email_template:
             return
         try:
             MarkupTemplate(self.email_template)
-        except Exception as exception:
+        except GenshiTemplateError as exception:
             raise TemplateError(
                 gettext('marketing_automation'
                     '.msg_activity_invalid_email_template',
                     activity=self.rec_name,
                     exception=exception)) from exception
 
     def check_email_title(self, fields_names=None):
         if fields_names and 'email_title' not in fields_names:
             return
         if not self.email_title:
             return
         try:
             TextTemplate(self.email_title)
-        except Exception as exception:
+        except GenshiTemplateError as exception:
             raise TemplateError(
                 gettext('marketing_automation'
                     '.msg_activity_invalid_email_title',
                     activity=self.rec_name,
                     exception=exception)) from exception
 
     def execute(self, activity, **kwargs):
@@ -524,32 +648,29 @@
                 RecordActivity.get(record, child)
                 for child in self.children])
 
     def _email_recipient(self, record):
         party = record.marketing_party
         contact = party.contact_mechanism_get('email')
         if contact and contact.email:
-            return _formataddr(
-                contact.name or party.rec_name,
-                contact.email)
+            return format_address(
+                contact.email, contact.name or party.rec_name)
 
     def execute_send_email(
             self, record_activity, smtpd_datamanager=None, **kwargs):
         pool = Pool()
         WebShortener = pool.get('web.shortened_url')
         Email = pool.get('ir.email')
         record = record_activity.record
 
         with Transaction().set_context(language=record.language):
             record = record.__class__(record.id)
             translated = self.__class__(self.id)
 
         to = self._email_recipient(record.record)
-        if not to:
-            return
 
         def unsubscribe(redirect):
             parts = urlsplit(urljoin(
                     URL_BASE, quote('/m/%(database)s/unsubscribe' % {
                             'database': Base64Converter(None).to_url(
                                 Transaction().database.name),
                             })))
@@ -589,63 +710,75 @@
                                 (QName('height'), '1'),
                                 (QName('width'), '1'),
                                 ])), pos
                     yield END, QName('img'), pos
                 yield kind, data, pos
 
         context = self.email_context(record)
-        title = (TextTemplate(translated.email_title)
-            .generate(**context)
-            .render())
-        template = MarkupTemplate(translated.email_template)
-        content = (template
-            .generate(**context)
-            .filter(convert_href)
-            .render())
+        context['short'] = partial(short, event='on_email_clicked')
+        try:
+            title = (TextTemplate(translated.email_title)
+                .generate(**context)
+                .render())
+        except GenshiTemplateError as exception:
+            raise TemplateError(
+                gettext('marketing_automation'
+                    '.msg_activity_invalid_email_title',
+                    activity=self.rec_name,
+                    exception=exception)) from exception
+        try:
+            template = MarkupTemplate(translated.email_template)
+            content = (template
+                .generate(**context)
+                .filter(convert_href)
+                .render())
+        except GenshiTemplateError as exception:
+            raise TemplateError(gettext('marketing_automation'
+                    '.msg_activity_invalid_email_template',
+                    activity=self.rec_name,
+                    exception=exception)) from exception
 
-        from_ = (config.get('marketing', 'email_from')
-            or config.get('email', 'from'))
-        msg = MIMEMultipart('alternative')
-        set_from_header(msg, from_, translated.email_from or from_)
-        msg['To'] = to
-        msg['Subject'] = Header(title, 'utf-8')
-        if html2text:
-            converter = html2text.HTML2Text()
-            part = MIMEText(
-                converter.handle(content), 'plain', _charset='utf-8')
-            msg.attach(part)
-        part = MIMEText(content, 'html', _charset='utf-8')
-        msg.attach(part)
-
-        to_addrs = [a for _, a in getaddresses([to])]
-        if to_addrs:
-            sendmail_transactional(
-                from_, to_addrs, msg, datamanager=smtpd_datamanager)
-
-            email = Email(
-                recipients=to,
-                addresses=[{'address': a} for a in to_addrs],
-                subject=title,
-                resource=record.record,
+        msg = self._email(translated.email_from, to, title, content)
+
+        if has_rcpt(msg):
+            send_message_transactional(msg, datamanager=smtpd_datamanager)
+            email = Email.from_message(
+                msg, resource=record.record,
                 marketing_automation_activity=self,
-                marketing_automation_record=record,
-                )
+                marketing_automation_record=record)
             email.save()
 
     def email_context(self, record):
         return {
             'record': record.record,
             'format_date': Report.format_date,
             'format_datetime': Report.format_datetime,
             'format_timedelta': Report.format_timedelta,
             'format_currency': Report.format_currency,
             'format_number': Report.format_number,
             'datetime': datetime,
             }
 
+    def _email(self, sender, to, subject, content):
+        msg = EmailMessage()
+        from_ = (config.get('marketing', 'email_from')
+            or config.get('email', 'from'))
+        set_from_header(msg, from_, sender or from_)
+        msg['To'] = to
+        msg['Subject'] = subject
+        if html2text:
+            converter = html2text.HTML2Text()
+            content_text = converter.handle(content)
+            msg.add_alternative(content_text, subtype='plain')
+        if msg.is_multipart():
+            msg.add_alternative(content, subtype='html')
+        else:
+            msg.set_content(content, subtype='html')
+        return msg
+
 
 class Record(ModelSQL, ModelView):
     "Marketing Record"
     __name__ = 'marketing.automation.record'
 
     scenario = fields.Many2One(
         'marketing.automation.scenario', "Scenario",
@@ -757,14 +890,15 @@
     activity_action = fields.Function(
         fields.Selection('get_activity_actions', "Activity Action"),
         'on_change_with_activity_action')
     at = fields.DateTime(
         "At",
         states={
             'readonly': Eval('state') != 'waiting',
+            'required': Eval('state') == 'done',
             })
     email_opened = fields.Boolean(
         "E-Mail Opened",
         states={
             'invisible': Eval('activity_action') != 'send_email',
             })
     email_clicked = fields.Boolean(
```

### Comparing `trytond_marketing_automation-7.0.0/marketing_automation.xml` & `trytond_marketing_automation-7.2.0/marketing_automation.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_marketing_automation-7.0.0/marketing_automation.xml` & `trytond_marketing_automation-7.2.0/marketing_automation.xml`

```diff
@@ -50,42 +50,42 @@
     <record model="ir.action.act_window.domain" id="act_scenario_form_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="act_window" ref="act_scenario_form"/>
     </record>
     <menuitem parent="marketing.menu_marketing" action="act_scenario_form" sequence="10" id="menu_scenario_form"/>
     <record model="ir.model.access" id="access_scenario">
-      <field name="model" search="[('model', '=', 'marketing.automation.scenario')]"/>
+      <field name="model">marketing.automation.scenario</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_scenario_marketing">
-      <field name="model" search="[('model', '=', 'marketing.automation.scenario')]"/>
+      <field name="model">marketing.automation.scenario</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="scenario_draft_button">
+      <field name="model">marketing.automation.scenario</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'marketing.automation.scenario')]"/>
     </record>
     <record model="ir.model.button" id="scenario_run_button">
+      <field name="model">marketing.automation.scenario</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'marketing.automation.scenario')]"/>
     </record>
     <record model="ir.model.button" id="scenario_stop_button">
+      <field name="model">marketing.automation.scenario</field>
       <field name="name">stop</field>
       <field name="string">Stop</field>
-      <field name="model" search="[('model', '=', 'marketing.automation.scenario')]"/>
     </record>
     <record model="ir.ui.view" id="activity_view_list">
       <field name="model">marketing.automation.activity</field>
       <field name="type">tree</field>
       <field name="priority" eval="10"/>
       <field name="name">activity_tree</field>
     </record>
@@ -123,22 +123,22 @@
     </record>
     <record model="ir.action.keyword" id="act_activity_tree_keyword2">
       <field name="keyword">tree_open</field>
       <field name="model">marketing.automation.scenario,-1</field>
       <field name="action" ref="act_activity_tree"/>
     </record>
     <record model="ir.model.access" id="access_activity">
-      <field name="model" search="[('model', '=', 'marketing.automation.activity')]"/>
+      <field name="model">marketing.automation.activity</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_activity_marketing">
-      <field name="model" search="[('model', '=', 'marketing.automation.activity')]"/>
+      <field name="model">marketing.automation.activity</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="record_view_list">
@@ -168,32 +168,32 @@
     </record>
     <record model="ir.action.keyword" id="act_record_form_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">marketing.automation.scenario,-1</field>
       <field name="action" ref="act_record_form"/>
     </record>
     <record model="ir.model.access" id="access_record">
-      <field name="model" search="[('model', '=', 'marketing.automation.record')]"/>
+      <field name="model">marketing.automation.record</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_record_marketing">
-      <field name="model" search="[('model', '=', 'marketing.automation.record')]"/>
+      <field name="model">marketing.automation.record</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="record_block_button">
+      <field name="model">marketing.automation.record</field>
       <field name="name">block</field>
       <field name="string">Block</field>
-      <field name="model" search="[('model', '=', 'marketing.automation.record')]"/>
     </record>
     <record model="ir.ui.view" id="record_activity_view_list">
       <field name="model">marketing.automation.record.activity</field>
       <field name="type">tree</field>
       <field name="name">record_activity_list</field>
     </record>
     <record model="ir.ui.view" id="record_activity_view_form">
@@ -247,41 +247,41 @@
     </record>
     <record model="ir.action.keyword" id="act_record_activity_form_keyword2">
       <field name="keyword">form_relate</field>
       <field name="model">marketing.automation.activity,-1</field>
       <field name="action" ref="act_record_activity_form"/>
     </record>
     <record model="ir.model.access" id="access_record_activity">
-      <field name="model" search="[('model', '=', 'marketing.automation.record.activity')]"/>
+      <field name="model">marketing.automation.record.activity</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_record_activity_marketing">
-      <field name="model" search="[('model', '=', 'marketing.automation.record.activity')]"/>
+      <field name="model">marketing.automation.record.activity</field>
       <field name="group" ref="marketing.group_marketing"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="record_activity_on_email_opened_button">
+      <field name="model">marketing.automation.record.activity</field>
       <field name="name">on_email_opened</field>
       <field name="string">E-Mail Opened</field>
-      <field name="model" search="[('model', '=', 'marketing.automation.record.activity')]"/>
     </record>
     <record model="ir.model.button" id="record_activity_on_email_clicked_button">
+      <field name="model">marketing.automation.record.activity</field>
       <field name="name">on_email_clicked</field>
       <field name="string">E-Mail Clicked</field>
-      <field name="model" search="[('model', '=', 'marketing.automation.record.activity')]"/>
     </record>
     <record model="ir.action.report" id="report_unsubscribe">
       <field name="name">Marketing Automation Unsubscribe</field>
-      <field name="model"/>
+      <field name="model" eval="None"/>
       <field name="report_name">marketing.automation.unsubscribe</field>
       <field name="report">marketing_automation/unsubscribe.html</field>
       <field name="template_extension">html</field>
     </record>
     <record model="ir.cron" id="cron_scenario_trigger">
       <field name="method">marketing.automation.scenario|trigger</field>
       <field name="interval_number" eval="1"/>
```

### Comparing `trytond_marketing_automation-7.0.0/message.xml` & `trytond_marketing_automation-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/mixin.py` & `trytond_marketing_automation-7.2.0/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/party.py` & `trytond_marketing_automation-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/routes.py` & `trytond_marketing_automation-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/sale.py` & `trytond_marketing_automation-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/setup.py` & `trytond_marketing_automation-7.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
 def get_require_version(name):
     require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
@@ -37,36 +40,39 @@
 
 if minor_version % 2:
     download_url = ''
 else:
     download_url = 'http://downloads.tryton.org/%s.%s/' % (
         major_version, minor_version)
 
-requires = ['Genshi']
+requires = ['Genshi', 'python-dateutil']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
-    get_require_version('trytond_sale')]
+    get_require_version('trytond_sale'),
+    'pygal',
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module to plan, '
     'coordinate and manage marketing campaigns',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": (
+            'https://docs.tryton.org/modules-marketing-automation'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton marketing automation',
     package_dir={'trytond.modules.marketing_automation': '.'},
     packages=(
         ['trytond.modules.marketing_automation']
@@ -119,14 +125,15 @@
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     license='GPL-3',
     python_requires='>=3.8',
     install_requires=requires,
     extras_require={
+        'sparklines': ['pygal'],
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     marketing_automation = trytond.modules.marketing_automation
     """,
```

### Comparing `trytond_marketing_automation-7.0.0/tests/scenario_marketing_automation.rst` & `trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Marketing Automation Scenario
 =============================
 
 Imports::
 
     >>> import datetime
     >>> import re
-    >>> from proteus import Model, Wizard
-    >>> from proteus.config import get_config
+    >>> from unittest.mock import patch
+
+    >>> from proteus import Model
+    >>> from trytond.modules.marketing_automation import marketing_automation
     >>> from trytond.pyson import Eval, PYSONEncoder
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.tests.tools import (
+    ...     activate_modules, assertEqual, assertIn, assertTrue)
     >>> from trytond.tools import file_open
 
-Patch sendmail_transactional::
+Patch send_message_transactional::
 
-    >>> from unittest.mock import patch
-    >>> from trytond.modules.marketing_automation import marketing_automation
     >>> smtp_calls = patch.object(
-    ...     marketing_automation, 'sendmail_transactional').start()
+    ...     marketing_automation, 'send_message_transactional').start()
     >>> manager = patch.object(
     ...     marketing_automation, 'SMTPDataManager').start()
 
 Activate modules::
 
     >>> config = activate_modules('marketing_automation')
 
     >>> Email = Model.get('ir.email')
+    >>> ReportingScenario = Model.get('marketing.automation.reporting.scenario')
+    >>> ReportingActivity = Model.get('marketing.automation.reporting.activity')
 
 Create a party::
 
     >>> Party = Model.get('party.party')
     >>> party = Party()
     >>> party.name = "Michael Scott"
     >>> contact = party.contact_mechanisms.new()
@@ -101,20 +104,31 @@
     ...     ('method', '=', 'marketing.automation.record.activity|process'),
     ...     ])
     >>> cron_trigger.click('run_once')
     >>> cron_process.click('run_once')
 
     >>> Record = Model.get('marketing.automation.record')
     >>> record, = Record.find([])
-    >>> record.record == party
-    True
+    >>> assertEqual(record.record, party)
     >>> scenario.record_count
     1
     >>> scenario.record_count_blocked
     0
+    >>> scenario.block_rate
+    0.0
+    >>> bool(scenario.block_rate_trend)
+    True
+
+    >>> reporting, = ReportingScenario.find([])
+    >>> reporting.record_count
+    1
+    >>> reporting.record_count_blocked
+    0
+    >>> reporting.block_rate
+    0.0
 
 Check email sent::
 
     >>> ShortenedURL = Model.get('web.shortened_url')
     >>> open_url, = ShortenedURL.find([
     ...         ('redirect_url', 'like', '%/m/empty.gif'),
     ...         ])
@@ -131,47 +145,39 @@
     'done'
     >>> root_activity.reload()
     >>> root_activity.record_count
     1
 
     >>> smtp_calls.call_count
     1
-    >>> from_, to, msg = smtp_calls.call_args[0]
+    >>> msg, = smtp_calls.call_args[0]
     >>> smtp_calls.reset_mock()
-    >>> msg = msg.get_payload(0).get_payload(decode=True).decode('utf-8')
-    >>> to == [contact.value]
-    True
-    >>> re.search(r'Hello, (.*)!', msg).group(1) == party.name
-    True
+    >>> msg = msg.get_body().get_content()
+    >>> assertEqual(re.search(r'Hello, (.*)!', msg).group(1), party.name)
     >>> open_url.shortened_url in msg
     True
-    >>> open_url.record == record_activity
-    True
+    >>> assertEqual(open_url.record, record_activity)
     >>> open_url.method
     'marketing.automation.record.activity|on_email_opened'
     >>> click_url.shortened_url in msg
     True
-    >>> click_url.record == record_activity
-    True
+    >>> assertEqual(click_url.record, record_activity)
     >>> click_url.method
     'marketing.automation.record.activity|on_email_clicked'
-    >>> record.uuid in msg
-    True
+    >>> assertIn(record.uuid, msg)
 
     >>> email, = Email.find([])
     >>> email.recipients
     'Michael Scott <michael@example.com>'
     >>> email.subject
     'Hello'
     >>> email.resource == party
     True
-    >>> email.marketing_automation_activity == root_activity
-    True
-    >>> bool(email.marketing_automation_record)
-    True
+    >>> assertEqual(email.marketing_automation_activity, root_activity)
+    >>> assertTrue(email.marketing_automation_record)
 
 Trigger open email and reminder after delay::
 
     >>> record_activity.click('on_email_opened')
 
     >>> open_activity, = RecordActivity.find([
     ...         ('record', '=', record.id),
@@ -186,14 +192,48 @@
 
     >>> open_activity.reload()
     >>> open_activity.state
     'done'
     >>> root_activity.reload()
     >>> root_activity.email_opened
     1
+    >>> root_activity.email_opened
+    1
+    >>> root_activity.email_clicked
+    0
+    >>> root_activity.email_open_rate
+    1.0
+    >>> bool(root_activity.email_open_rate_trend)
+    True
+    >>> root_activity.email_click_rate
+    0.0
+    >>> bool(root_activity.email_click_rate_trend)
+    True
+    >>> root_activity.email_click_through_rate
+    0.0
+    >>> bool(root_activity.email_click_through_rate_trend)
+    True
+
+    >>> reporting, = ReportingActivity.find([
+    ...         ('activity', '=', root_activity.id),
+    ...         ])
+    >>> reporting.activity_action
+    'send_email'
+    >>> reporting.record_count
+    1
+    >>> reporting.email_opened
+    1
+    >>> reporting.email_clicked
+    0
+    >>> reporting.email_open_rate
+    1.0
+    >>> reporting.email_click_rate
+    0.0
+    >>> reporting.email_click_through_rate
+    0.0
 
     >>> email_reminder, = RecordActivity.find([
     ...         ('record', '=', record.id),
     ...         ('activity', '=', email_reminder.id),
     ...         ])
     >>> email_reminder.state
     'done'
@@ -210,16 +250,40 @@
     >>> clicked_activity, = RecordActivity.find([
     ...         ('record', '=', record.id),
     ...         ('activity', '=', email_clicked.id),
     ...         ])
     >>> clicked_activity.state
     'done'
     >>> root_activity.reload()
+    >>> root_activity.record_count
+    1
+    >>> root_activity.email_opened
+    1
     >>> root_activity.email_clicked
     1
+    >>> root_activity.email_open_rate
+    1.0
+    >>> root_activity.email_click_rate
+    1.0
+    >>> root_activity.email_click_through_rate
+    1.0
+
+    >>> reporting.reload()
+    >>> reporting.record_count
+    1
+    >>> reporting.email_opened
+    1
+    >>> reporting.email_clicked
+    1
+    >>> reporting.email_open_rate
+    1.0
+    >>> reporting.email_click_rate
+    1.0
+    >>> reporting.email_click_through_rate
+    1.0
 
     >>> not_clicked_activity, = RecordActivity.find([
     ...         ('record', '=', record.id),
     ...         ('activity', '=', email_not_clicked.id),
     ...         ])
     >>> not_clicked_activity.state
     'cancelled'
```

### Comparing `trytond_marketing_automation-7.0.0/tests/scenario_marketing_automation_unsubscribable.rst` & `trytond_marketing_automation-7.2.0/tests/scenario_marketing_automation_unsubscribable.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Marketing Automation Unsubscribable Scenario
 ============================================
 
 Imports::
 
-    >>> import datetime
-    >>> import re
+    >>> from unittest.mock import patch
 
-    >>> from proteus import Model, Wizard
-    >>> from proteus.config import get_config
+    >>> from proteus import Model
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.modules.marketing_automation import marketing_automation
     >>> from trytond.pyson import Eval, PYSONEncoder
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.tests.tools import activate_modules, assertEqual
     >>> from trytond.tools import file_open
 
-Patch sendmail_transactional::
+Patch send_message_transactional::
 
-    >>> from unittest.mock import patch
-    >>> from trytond.modules.marketing_automation import marketing_automation
     >>> smtp_calls = patch.object(
-    ...     marketing_automation, 'sendmail_transactional').start()
+    ...     marketing_automation, 'send_message_transactional').start()
     >>> manager = patch.object(
     ...     marketing_automation, 'SMTPDataManager').start()
 
 Activate modules::
 
     >>> config = activate_modules(['marketing_automation', 'sale'])
 
@@ -80,25 +77,39 @@
 
 Trigger scenario::
 
     >>> cron_trigger.click('run_once')
     >>> cron_process.click('run_once')
 
     >>> record, = Record.find([])
-    >>> record.record == sale
-    True
+    >>> assertEqual(record.record, sale)
+
+    >>> scenario.reload()
+    >>> scenario.record_count
+    1
+    >>> scenario.record_count_blocked
+    0
+    >>> scenario.block_rate
+    0.0
 
 Block and unsubscribe::
 
     >>> record.click('block')
     >>> bool(record.blocked)
     True
     >>> party.reload()
-    >>> party.marketing_scenario_unsubscribed == [scenario]
-    True
+    >>> assertEqual(party.marketing_scenario_unsubscribed, [scenario])
+
+    >>> scenario.reload()
+    >>> scenario.record_count
+    1
+    >>> scenario.record_count_blocked
+    1
+    >>> scenario.block_rate
+    1.0
 
 Create a new sale::
 
     >>> sale = Sale(party=party)
     >>> sale.save()
 
 Trigger scenario::
```

### Comparing `trytond_marketing_automation-7.0.0/tox.ini` & `trytond_marketing_automation-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/trytond_marketing_automation.egg-info/SOURCES.txt` & `trytond_marketing_automation-7.2.0/trytond_marketing_automation.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 empty.gif
 exceptions.py
 ir.py
 ir.xml
 marketing_automation.py
 marketing_automation.xml
+marketing_automation_reporting.py
+marketing_automation_reporting.xml
 message.xml
 mixin.py
 party.py
 party.xml
 routes.py
 sale.py
 setup.py
@@ -25,14 +26,16 @@
 ./__init__.py
 ./empty.gif
 ./exceptions.py
 ./ir.py
 ./ir.xml
 ./marketing_automation.py
 ./marketing_automation.xml
+./marketing_automation_reporting.py
+./marketing_automation_reporting.xml
 ./message.xml
 ./mixin.py
 ./party.py
 ./party.xml
 ./routes.py
 ./sale.py
 ./tryton.cfg
@@ -73,18 +76,28 @@
 ./view/activity_tree.xml
 ./view/ir_email_form.xml
 ./view/party_form.xml
 ./view/record_activity_form.xml
 ./view/record_activity_list.xml
 ./view/record_form.xml
 ./view/record_list.xml
+./view/reporting_activity_graph_count.xml
+./view/reporting_activity_graph_rate.xml
+./view/reporting_activity_list.xml
+./view/reporting_context_form.xml
+./view/reporting_scenario_graph_count.xml
+./view/reporting_scenario_graph_rate.xml
+./view/reporting_scenario_list.xml
 ./view/scenario_form.xml
 ./view/scenario_list.xml
 doc/conf.py
+doc/configuration.rst
+doc/design.rst
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -124,9 +137,16 @@
 view/activity_tree.xml
 view/ir_email_form.xml
 view/party_form.xml
 view/record_activity_form.xml
 view/record_activity_list.xml
 view/record_form.xml
 view/record_list.xml
+view/reporting_activity_graph_count.xml
+view/reporting_activity_graph_rate.xml
+view/reporting_activity_list.xml
+view/reporting_context_form.xml
+view/reporting_scenario_graph_count.xml
+view/reporting_scenario_graph_rate.xml
+view/reporting_scenario_list.xml
 view/scenario_form.xml
 view/scenario_list.xml
```

### Comparing `trytond_marketing_automation-7.0.0/unsubscribe.html` & `trytond_marketing_automation-7.2.0/unsubscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/view/activity_form.xml` & `trytond_marketing_automation-7.2.0/view/activity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/view/record_activity_form.xml` & `trytond_marketing_automation-7.2.0/view/record_activity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/view/scenario_form.xml` & `trytond_marketing_automation-7.2.0/view/scenario_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-7.0.0/web.py` & `trytond_marketing_automation-7.2.0/web.py`

 * *Files identical despite different names*

