# Comparing `tmp/trytond_company-7.0.0.tar.gz` & `tmp/trytond_company-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_company-7.0.0.tar", last modified: Mon Oct 30 17:28:47 2023, max compression
+gzip compressed data, was "trytond_company-7.2.0.tar", last modified: Mon Apr 29 15:39:21 2024, max compression
```

## Comparing `trytond_company-7.0.0.tar` & `trytond_company-7.2.0.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.095131 trytond_company-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-22 17:23:02.000000 trytond_company-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-10-30 17:05:42.000000 trytond_company-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:05:42.000000 trytond_company-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_company-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_company-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-10-30 17:28:47.095131 trytond_company-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_company-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1078 2023-04-15 07:12:15.000000 trytond_company-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4966 2023-04-15 07:12:15.000000 trytond_company-7.0.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9210 2023-04-15 07:12:15.000000 trytond_company-7.0.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.095131 trytond_company-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-22 17:23:02.000000 trytond_company-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2500 2023-04-15 07:12:15.000000 trytond_company-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_company-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2685 2023-10-24 07:56:52.000000 trytond_company-7.0.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_company-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:02.000000 trytond_company-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_company-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.095131 trytond_company-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_company-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:20.000000 trytond_company-7.0.0/icons/tryton-company.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     3792 2023-10-27 17:38:49.000000 trytond_company-7.0.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2023-04-15 07:12:15.000000 trytond_company-7.0.0/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    39274 2023-04-15 07:12:15.000000 trytond_company-7.0.0/letter.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.091798 trytond_company-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7704 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8085 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6806 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8395 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8184 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6534 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7869 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6806 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8315 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7781 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7676 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7330 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8575 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7334 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8154 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7938 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7973 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8028 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7991 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7888 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6806 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9304 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7724 2023-10-30 16:47:45.000000 trytond_company-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-10-24 07:56:52.000000 trytond_company-7.0.0/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-08-13 15:26:13.000000 trytond_company-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10236 2023-10-27 17:38:49.000000 trytond_company-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:28:47.095131 trytond_company-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4424 2023-10-27 17:38:49.000000 trytond_company-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.091798 trytond_company-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_company-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11088 2023-10-07 15:40:36.000000 trytond_company-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1219 2023-06-10 11:39:56.000000 trytond_company-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_company-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-10-30 17:05:39.000000 trytond_company-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.095131 trytond_company-7.0.0/trytond_company.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-10-30 17:28:46.000000 trytond_company-7.0.0/trytond_company.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2052 2023-10-30 17:28:47.000000 trytond_company-7.0.0/trytond_company.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:28:46.000000 trytond_company-7.0.0/trytond_company.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-10-30 17:28:46.000000 trytond_company-7.0.0/trytond_company.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_company-7.0.0/trytond_company.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-10-30 17:28:46.000000 trytond_company-7.0.0/trytond_company.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:28:46.000000 trytond_company-7.0.0/trytond_company.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:28:47.091798 trytond_company-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_company-7.0.0/view/company_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/employee_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/employee_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-01-16 14:00:20.000000 trytond_company-7.0.0/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/sequence_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_company-7.0.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4545 2024-04-29 15:18:56.000000 trytond_company-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:18:55.000000 trytond_company-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_company-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_company-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-04-29 15:39:21.971109 trytond_company-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-29 13:17:17.000000 trytond_company-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1078 2024-04-29 13:17:17.000000 trytond_company-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7587 2024-04-29 13:17:17.000000 trytond_company-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9118 2024-04-27 16:30:39.000000 trytond_company-7.2.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.967776 trytond_company-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_company-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2500 2023-04-15 07:12:15.000000 trytond_company-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-29 13:17:17.000000 trytond_company-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2685 2024-02-04 18:51:26.000000 trytond_company-7.2.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_company-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:07.000000 trytond_company-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1037 2024-04-13 17:12:23.000000 trytond_company-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.967776 trytond_company-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_company-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:20.000000 trytond_company-7.2.0/icons/tryton-company.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     4009 2024-04-29 13:17:17.000000 trytond_company-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-27 16:30:39.000000 trytond_company-7.2.0/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    39343 2024-04-29 13:17:17.000000 trytond_company-7.2.0/letter.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8064 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8352 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7166 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8651 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8430 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6894 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8171 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8958 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7166 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9095 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8141 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7955 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7690 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8935 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7694 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8402 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8240 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8236 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8371 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8351 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8177 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7166 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9489 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8010 2024-04-29 13:17:17.000000 trytond_company-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2024-02-04 18:51:26.000000 trytond_company-7.2.0/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2814 2024-04-22 12:14:36.000000 trytond_company-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10152 2024-04-22 12:14:36.000000 trytond_company-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:21.971109 trytond_company-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4415 2024-04-29 13:17:17.000000 trytond_company-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_company-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15063 2024-04-27 16:30:39.000000 trytond_company-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1219 2024-01-27 09:58:52.000000 trytond_company-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:07.000000 trytond_company-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2024-04-29 15:18:51.000000 trytond_company-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/trytond_company.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_company-7.2.0/trytond_company.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:21.000000 trytond_company-7.2.0/trytond_company.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:21.971109 trytond_company-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_company-7.2.0/view/company_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-29 13:17:17.000000 trytond_company-7.2.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/employee_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/employee_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-01-16 14:00:20.000000 trytond_company-7.2.0/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/sequence_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_company-7.2.0/view/user_form_preferences.xml
```

### Comparing `trytond_company-7.0.0/CHANGELOG` & `trytond_company-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Activate employee based on dates
+* Use template substitution for company header/footer
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Remove employee and employees from evaluation context of rule domain
 * Define when set or reset employee field
```

### Comparing `trytond_company-7.0.0/LICENSE` & `trytond_company-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/PKG-INFO` & `trytond_company-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_company
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with companies and employees
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-company/
+Project-URL: Documentation, https://docs.tryton.org/modules-company/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton company employee
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,17 +49,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 ##############
 Company Module
 ##############
 
 The *Company Module* allows the business that is using Tryton to be
 represented inside Tryton.
```

### Comparing `trytond_company-7.0.0/__init__.py` & `trytond_company-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/company.xml` & `trytond_company-7.2.0/company.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_company-7.0.0/company.xml` & `trytond_company-7.2.0/company.xml`

```diff
@@ -54,22 +54,22 @@
     <record model="ir.action.act_window.view" id="act_company_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="company_view_form"/>
       <field name="act_window" ref="act_company_list"/>
     </record>
     <menuitem parent="menu_company" action="act_company_list" sequence="10" id="menu_company_list"/>
     <record model="ir.model.access" id="access_company">
-      <field name="model" search="[('model', '=', 'company.company')]"/>
+      <field name="model">company.company</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_company_admin">
-      <field name="model" search="[('model', '=', 'company.company')]"/>
+      <field name="model">company.company</field>
       <field name="group" ref="group_company_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="user_view_form">
@@ -139,22 +139,22 @@
     </record>
     <record model="ir.action.keyword" id="act_employee_subordinates_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">company.employee,-1</field>
       <field name="action" ref="act_employee_subordinates"/>
     </record>
     <record model="ir.model.access" id="access_employee">
-      <field name="model" search="[('model', '=', 'company.employee')]"/>
+      <field name="model">company.employee</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_employee_admin">
-      <field name="model" search="[('model', '=', 'company.employee')]"/>
+      <field name="model">company.employee</field>
       <field name="group" ref="group_employee_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.report" id="report_letter">
```

### Comparing `trytond_company-7.0.0/doc/conf.py` & `trytond_company-7.2.0/doc/conf.py`

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

### Comparing `trytond_company-7.0.0/doc/design.rst` & `trytond_company-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/doc/reference.rst` & `trytond_company-7.2.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/icons/LICENSE` & `trytond_company-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/ir.py` & `trytond_company-7.2.0/ir.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+
+from trytond import backend
 from trytond.model import ModelSQL, ModelView, dualmethod, fields
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import timezone as tz
 from trytond.transaction import Transaction
 
 
 class Sequence(metaclass=PoolMeta):
@@ -47,18 +49,18 @@
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.domain.help += (
             '\n- "companies" as list of ids from the current user')
 
     @classmethod
-    def _get_cache_key(cls, model_name):
+    def _get_cache_key(cls, model_names):
         pool = Pool()
         User = pool.get('res.user')
-        key = super()._get_cache_key(model_name)
+        key = super()._get_cache_key(model_names)
         return (*key, User.get_companies())
 
     @classmethod
     def _get_context(cls, model_name):
         pool = Pool()
         User = pool.get('res.user')
         context = super()._get_context(model_name)
@@ -87,20 +89,25 @@
         Company = Pool().get('company.company')
         return list(map(int, Company.search([])))
 
 
 class CronCompany(ModelSQL):
     'Cron - Company'
     __name__ = 'ir.cron-company.company'
-    _table = 'cron_company_rel'
     cron = fields.Many2One(
         'ir.cron', "Cron", ondelete='CASCADE', required=True)
     company = fields.Many2One(
         'company.company', "Company", ondelete='CASCADE', required=True)
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename('cron_company_rel', cls._table)
+        super().__register__(module)
+
 
 class EmailTemplate(metaclass=PoolMeta):
     __name__ = 'ir.email.template'
 
     @classmethod
     def email_models(cls):
         return super().email_models() + ['company.employee']
```

### Comparing `trytond_company-7.0.0/ir.xml` & `trytond_company-7.2.0/ir.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_company-7.0.0/ir.xml` & `trytond_company-7.2.0/ir.xml`

```diff
@@ -21,28 +21,28 @@
     <record model="ir.ui.view" id="sequence_strict_view_tree">
       <field name="model">ir.sequence.strict</field>
       <field name="inherit" ref="ir.sequence_view_tree"/>
       <field name="name">sequence_tree</field>
     </record>
     <record model="ir.rule.group" id="rule_group_sequence_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'ir.sequence')]"/>
+      <field name="model">ir.sequence</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sequence_companies1">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sequence_companies"/>
     </record>
     <record model="ir.rule" id="rule_sequence_comapnies2">
       <field name="domain" eval="[('company', '=', None)]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sequence_companies"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sequence_strict_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'ir.sequence.strict')]"/>
+      <field name="model">ir.sequence.strict</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sequence_strict_companies1">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sequence_strict_companies"/>
     </record>
     <record model="ir.rule" id="rule_sequence_strict_companies2">
```

### Comparing `trytond_company-7.0.0/letter.fodt` & `trytond_company-7.2.0/letter.fodt`

 * *Files 1% similar despite different names*

#### Comparing `trytond_company-7.0.0/letter.fodt` & `trytond_company-7.2.0/letter.fodt`

```diff
@@ -356,38 +356,38 @@
       </style:footer-style>
     </style:page-layout>
   </office:automatic-styles>
   <office:master-styles>
     <style:master-page style:name="Standard" style:page-layout-name="pm1">
       <style:header>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;if test=&quot;user.company.header&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;if test=&quot;user.company and user.company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in user.company.header.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in user.company.header_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P3">
-          <text:placeholder text:placeholder-type="text">&lt;user.company.rec_name&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;user.company.rec_name if user.company else ''&gt;</text:placeholder>
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P2">
-          <text:placeholder text:placeholder-type="text">&lt;if test=&quot;user.company.footer&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;if test=&quot;user.company and user.company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in user.company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in user.company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
```

### Comparing `trytond_company-7.0.0/locale/bg.po` & `trytond_company-7.2.0/locale/bg.po`

 * *Files 6% similar despite different names*

```diff
@@ -132,19 +132,39 @@
 msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/ca.po` & `trytond_company-7.2.0/locale/ca.po`

 * *Files 3% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "La moneda principal de l'empresa."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Afegiu empleats a l'empresa."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "El text a mostrar als peus dels informes."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "El text a mostrar a les capcel·leres dels informes."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Utilitzat per calcular la data d'avui."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/cs.po` & `trytond_company-7.2.0/locale/es_419.po`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Employees"
+msgstr ""
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
 msgstr ""
 
 msgctxt "field:company.company,header:"
 msgid "Header"
@@ -47,103 +46,116 @@
 msgid "Subordinates"
 msgstr ""
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr ""
+msgstr "Programador de tareas"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Employees"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Employees"
+msgstr ""
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
 msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
@@ -212,78 +224,73 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Employees"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Configure Company"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Employees"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
 msgstr ""
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Letter"
+msgstr ""
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Companies"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Companies"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Employees"
+msgstr ""
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
 msgstr ""
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Companies"
+msgstr ""
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
 msgstr ""
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
```

### Comparing `trytond_company-7.0.0/locale/de.po` & `trytond_company-7.2.0/locale/de.po`

 * *Files 6% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "Die Standardwährung des Unternehmens."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Dem Unternehmen Mitarbeiter hinzufügen."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Der anzuzeigende Text in der Fußzeile der Berichte."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Der anzuzeigende Text in der Kopfzeile der Berichte."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Wird zum berechnen des heutigen Datums verwendet."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/es.po` & `trytond_company-7.2.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "La moneda principal de la empresa."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Añade empleados a la empresa."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "El texto a mostrar en los pies de página de los informes."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "El texto a mostrar en los las cabeceras de los informes."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Utilizado para calcular la fecha de hoy."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/es_419.po` & `trytond_company-7.2.0/locale/pl.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,321 +1,349 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Waluta"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr ""
+msgstr "Pracownicy"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr ""
+msgstr "Stopka"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr ""
+msgstr "Nagłówek"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr ""
+msgstr "Strona"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr ""
+msgstr "Strefa czasowa"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data zakończenia"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr ""
+msgstr "Strona"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data rozpoczęcia"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr ""
+msgstr "Podwładni"
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr ""
+msgstr "Przełożony"
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr ""
+msgstr "Firmy"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Programador de tareas"
+msgstr "Cron"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
+#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr ""
+msgstr "Firmy"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr ""
+msgstr "Obecna firma"
 
+#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr ""
+msgstr "Firmy"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr ""
+msgstr "Obecny pracownik"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr ""
+msgstr "Pracownicy"
 
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr ""
+msgstr "Użytkownik"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Pracownik"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr ""
+msgstr "Użytkownik"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr ""
+msgstr "Główna waluta firmy."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr ""
+msgstr "Dodaj pracowników do firmy."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr ""
+msgstr "Służy do wyznaczenia dzisiejszej daty."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr ""
+msgstr "Firma, do której należą pracownicy."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr ""
+msgstr "Data opuszczenia firmy przez pracownika."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr ""
+msgstr "Strona reprezentująca pracownika."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr ""
+msgstr "Data przyjęcia pracownika do firmy."
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr ""
+msgstr "Pracownicy nadzorowani przez tego pracownika."
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr ""
+msgstr "Pracownik nadzorujący tego pracownika."
 
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr ""
+msgstr "Firmy zarejestrowane dla crona."
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
 
+#, fuzzy
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr ""
+msgstr "Ograniczenie użycia sekwencji do firmy."
 
+#, fuzzy
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr ""
+msgstr "Ograniczenie użycia sekwencji do firmy."
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr ""
+msgstr "Firmy, do których użytkownik ma dostęp."
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr ""
+msgstr "Wybór firmy, w której pracuje użytkownik."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
 msgstr ""
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr ""
+msgstr "Wybierz pracownika, który będzie użytkownikiem systemu."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr ""
+msgstr "Dodaj pracowników, do których użytkownik będzie miał dostęp."
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr ""
+msgstr "Konfiguracja ustawień firmy"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr ""
+msgstr "Pracownik"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr ""
+msgstr "Konfiguruj ustawienia firmy"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr ""
+msgstr "Firmy"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr ""
+msgstr "Pracownicy"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr ""
+msgstr "Nadzorowani przez"
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr ""
+msgstr "Letter"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr ""
+msgstr "Cron - Firma"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Użytkownik w firmie"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Użytkownik w firmie"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr ""
+msgstr "Firmy"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr ""
+msgstr "Firmy"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr ""
+msgstr "Pracownicy"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr ""
+msgstr "Administracja ustawieniami firmy"
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr ""
+msgstr "Administracja ustawieniami pracowników"
 
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr ""
+msgstr "Użytkownik - Firma"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr ""
+msgstr "Użytkownik - Pracownik"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr ""
+msgstr "Z pozdrowieniami,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr ""
+msgstr "Data:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr ""
+msgstr "Szanowni Państwo,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr ""
+msgstr "Temat:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr ""
+msgstr "Waluta"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr ""
+msgstr "Możesz dodać swoją firmę do systemu."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr ""
+msgstr "Raporty"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr ""
+msgstr "Dodaj"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anuluj"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anuluj"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_company-7.0.0/locale/et.po` & `trytond_company-7.2.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -127,20 +127,40 @@
 msgstr "Ettevõtte peamine valuuta"
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Lisa ettevõtte töötajad"
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Aruande jaluses kuvatav tekst"
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Aruande päises kuvatav tekst"
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Kasutatakse tänase kuupäeva tekitamiseks"
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/fa.po` & `trytond_company-7.2.0/locale/fa.po`

 * *Files 6% similar despite different names*

```diff
@@ -127,20 +127,40 @@
 msgstr "واحد ارز اصلی در شرکت."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "اضافه کردن کارمندان درشرکت."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "متن انتخابی برای نمایش در پانویس گزارش"
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "متن انتخابی برای نمایش در راس گزارش."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "برای محاسبه تاریخ امروز استفاده شده."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/fi.po` & `trytond_company-7.2.0/locale/cs.po`

 * *Files 7% similar despite different names*

```diff
@@ -131,19 +131,39 @@
 msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/fr.po` & `trytond_company-7.2.0/locale/ru.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,325 +1,361 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Валюта"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Employés"
+msgstr "Сотрудники"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Pied de Page"
+msgstr "Нижний колонтитул"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Entête"
+msgstr "Верхний колонтитул"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Контрагент"
 
+#, fuzzy
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Fuseau Horaire"
+msgstr "Зона времени"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Date de fin"
+msgstr ""
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Контрагент"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Date de début"
+msgstr ""
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "Subordonnés"
+msgstr ""
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr "Superviseur"
+msgstr ""
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Sociétés"
+msgstr "Организация"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Tâche planifiée"
+msgstr "Планировщик"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Sociétés"
+msgstr "Организация"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Société actuelle"
+msgstr "Текущая организация"
 
+#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Filtre de société"
+msgstr "Организация"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Employé actuel"
+msgstr "Сотрудник"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Employés"
+msgstr "Сотрудники"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Utilisateur"
+msgstr "Пользователь"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Employé"
+msgstr "Сотрудник"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Utilisateur"
+msgstr "Пользователь"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "La devise principale pour la société."
+msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Ajouter des employés à la société."
+msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Le texte à afficher en pied de rapport."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Le texte à afficher en entête de rapport."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Utilisé pour calculer la date du jour."
+msgstr ""
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "La société à qui l'employé appartient."
+msgstr ""
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Quand l'employé quitte la société."
+msgstr ""
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "Le tiers qui représente l'employé."
+msgstr ""
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Quand l'employé rejoins la société."
+msgstr ""
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "Les employés devant être supervisés par cet employé."
+msgstr ""
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "L'employé qui supervise cet employé."
+msgstr ""
 
+#, fuzzy
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Les sociétés enregistrées pour cette action planifiée."
+msgstr "Организации зарегистрированные для этого планировщика"
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
-"\n"
-"- « companies » comme liste d'identifiants de l'utilisateur actuel"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restreint l'utilisation de la séquence à la société."
+msgstr ""
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restreint l'utilisation de la séquence à la société."
+msgstr ""
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "Les sociétés auxquelles l'utilisateur a accès."
+msgstr ""
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Sélectionner la société pour laquelle travailler."
+msgstr ""
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr "Définit les enregistrements de quelles sociétés sont affichés."
+msgstr ""
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
 msgstr ""
-"Sélectionner l'employé pour lequel l'utilisateur se comportera en tant que "
-"tel."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Ajouter les employés dont l'utilisateur en aura l'accès."
+msgstr ""
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Société"
+msgstr "Организация"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Configuration société"
+msgstr "Настройка организации"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Employé"
+msgstr "Сотрудник"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Configuration société"
+msgstr "Configure Company"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Sociétés"
+msgstr "Companies"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Employés"
+msgstr "Employees"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "Supervisé par"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Lettre"
+msgstr "Letter"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Tâche planifiée - Société"
+msgstr "Планировщик - Организация"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Utilisateur dans les sociétés"
+msgstr "Планировщик - Организация"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Utilisateur dans les sociétés"
+msgstr "Планировщик - Организация"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Sociétés"
+msgstr "Организация"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Sociétés"
+msgstr "Companies"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Employés"
+msgstr "Employees"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "Administration des sociétés"
+msgstr ""
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "Administration des employés"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Utilisateur - société"
+msgstr "Планировщик - Организация"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Utilisateur - Employé"
+msgstr "Пользователь - Сотрудник"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "Bien cordialement,"
+msgstr "С уважением,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Date :"
+msgstr "Дата:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Chère madame, cher monsieur,"
+msgstr "Уважаемые дамы и годпода,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Sujet :"
+msgstr "Тема:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr "Toutes"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Actuelle"
+msgstr "Валюта"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Vous pouvez maintenant ajouter votre société au système."
+msgstr "Теперь вы можете добавить организации."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Rapports"
+msgstr "Отчеты"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Ajouter"
+msgstr "Добавить"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Отменить"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "OK"
+msgstr "Ок"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Отменить"
```

### Comparing `trytond_company-7.0.0/locale/hu.po` & `trytond_company-7.2.0/locale/hu.po`

 * *Files 6% similar despite different names*

```diff
@@ -126,19 +126,39 @@
 msgstr "A cég fő pénzneme."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Alkalmazottak hozzáadása a céghez."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/id.po` & `trytond_company-7.2.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -124,20 +124,40 @@
 msgstr "Mata uang utama untuk perusahaan."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Tambahkan karyawan ke perusahaan."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Teks yang ditampilkan pada kaki laporan."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Teks yang ditampilkan pada tajuk laporan."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/it.po` & `trytond_company-7.2.0/locale/it.po`

 * *Files 8% similar despite different names*

```diff
@@ -127,19 +127,39 @@
 msgstr "La valuta principale per l'azienda."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/lo.po` & `trytond_company-7.2.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -130,19 +130,39 @@
 msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/lt.po` & `trytond_company-7.2.0/locale/lt.po`

 * *Files 10% similar despite different names*

```diff
@@ -127,19 +127,39 @@
 msgstr "Organizacijos pagrindinė valiuta."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/nl.po` & `trytond_company-7.2.0/locale/nl.po`

 * *Files 5% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "De hoofd-valuta voor het bedrijf."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Voeg medewerkers toe aan het bedrijf."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "De tekst die wordt weergegeven op voetteksten van rapporten."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "De tekst die wordt weergegeven in de rapport aanhef."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Gebruikt om de datum van vandaag te berekenen."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/pl.po` & `trytond_company-7.2.0/locale/pt.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,329 +1,356 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Waluta"
+msgstr "Moeda"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Pracownicy"
+msgstr "Empregados"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Stopka"
+msgstr "Rodapé"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Nagłówek"
+msgstr "Cabeçalho"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Strona"
+msgstr "Pessoa"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Strefa czasowa"
+msgstr "Fuso Horário"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Data zakończenia"
+msgstr "Data de término"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Strona"
+msgstr "Pessoa"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Data rozpoczęcia"
+msgstr "Data de início"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "Podwładni"
+msgstr ""
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr "Przełożony"
+msgstr ""
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Firmy"
+msgstr "Empresas"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
 msgstr "Cron"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 #, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Firmy"
+msgstr "Empresas"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Obecna firma"
+msgstr "Empresa Atual"
 
 #, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Firmy"
+msgstr "Empresas"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Obecny pracownik"
+msgstr "Empregado Atual"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Pracownicy"
+msgstr "Empregados"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Użytkownik"
+msgstr "Usuário"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr "Empregado"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Użytkownik"
+msgstr "Usuário"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "Główna waluta firmy."
+msgstr "A principal moeda para a empresa."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Dodaj pracowników do firmy."
+msgstr "Adicione empregados à empresa."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Tekst w stopkach raportów."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Tekst w nagłówkach raportów."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Służy do wyznaczenia dzisiejszej daty."
+msgstr "Usado para computar a data de hoje."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "Firma, do której należą pracownicy."
+msgstr "A empresa a qual o empregado pertence."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Data opuszczenia firmy przez pracownika."
+msgstr "Quando o empregado sai da empresa."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "Strona reprezentująca pracownika."
+msgstr "A pessoa que representa o empregado."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Data przyjęcia pracownika do firmy."
+msgstr "Quando o empregado entra na empresa."
 
+#, fuzzy
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "Pracownicy nadzorowani przez tego pracownika."
+msgstr "A pessoa que representa o empregado."
 
+#, fuzzy
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "Pracownik nadzorujący tego pracownika."
+msgstr "A pessoa que representa o empregado."
 
+#, fuzzy
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Firmy zarejestrowane dla crona."
+msgstr "Empresas registradas para este cron"
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
 
 #, fuzzy
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Ograniczenie użycia sekwencji do firmy."
+msgstr "Restringe a sequência usada pela empresa."
 
 #, fuzzy
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Ograniczenie użycia sekwencji do firmy."
+msgstr "Restringe a sequência usada pela empresa."
 
+#, fuzzy
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "Firmy, do których użytkownik ma dostęp."
+msgstr "Adicione empregados para que os usuários tenham acesso a eles."
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Wybór firmy, w której pracuje użytkownik."
+msgstr "Selecione a empresa a trabalhar para."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
 msgstr ""
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "Wybierz pracownika, który będzie użytkownikiem systemu."
+msgstr "Selecione o empregado para fazer com que o usuário o represente."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Dodaj pracowników, do których użytkownik będzie miał dostęp."
+msgstr "Adicione empregados para que os usuários tenham acesso a eles."
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Empresa"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Konfiguracja ustawień firmy"
+msgstr "Configuração da Empresa"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr "Empregado"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Konfiguruj ustawienia firmy"
+msgstr "Configurar Empresa"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Firmy"
+msgstr "Empresas"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Pracownicy"
+msgstr "Empregados"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "Nadzorowani przez"
+msgstr ""
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Letter"
+msgstr "Carta"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Cron - Firma"
+msgstr "Cron - Empresa"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Użytkownik w firmie"
+msgstr "Cron - Empresa"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Użytkownik w firmie"
+msgstr "Cron - Empresa"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Firmy"
+msgstr "Empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Firmy"
+msgstr "Empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Pracownicy"
+msgstr "Empregados"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "Administracja ustawieniami firmy"
+msgstr ""
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "Administracja ustawieniami pracowników"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Użytkownik - Firma"
+msgstr "Cron - Empresa"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Użytkownik - Pracownik"
+msgstr "Usuário - Empregado"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "Z pozdrowieniami,"
+msgstr "Atenciosamente,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
 msgstr "Data:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Szanowni Państwo,"
+msgstr "Caros senhores e senhoras,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Temat:"
+msgstr "Assunto:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Waluta"
+msgstr "Moeda"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Możesz dodać swoją firmę do systemu."
+msgstr "Você pode agora adicionar sua empresa ao sistema."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Raporty"
+msgstr "Relatórios"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Dodaj"
+msgstr "Adicionar"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Anuluj"
+msgstr "Cancelar"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
 msgstr "OK"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Anuluj"
+msgstr "Cancelar"
```

### Comparing `trytond_company-7.0.0/locale/pt.po` & `trytond_company-7.2.0/locale/zh_CN.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,336 +1,343 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr "货币"
 
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "Empregados"
+msgstr "雇员"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "Rodapé"
+msgstr "页脚"
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "Cabeçalho"
+msgstr "页眉"
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "Pessoa"
+msgstr "参与者"
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "Fuso Horário"
+msgstr "时区"
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "Data de término"
+msgstr "离职日期"
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "Pessoa"
+msgstr "参与者"
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "Data de início"
+msgstr "入职日期"
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr ""
+msgstr "下级"
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr ""
+msgstr "监督者"
 
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "公司"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "Cron"
+msgstr "计划任务"
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "公司"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "Empresa Atual"
+msgstr "当前公司"
 
-#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "Empresas"
+msgstr "公司过滤器"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "Empregado Atual"
+msgstr "现任员工"
 
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "Empregados"
+msgstr "雇员"
 
-#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
-#, fuzzy
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "Usuário"
+msgstr "用户"
 
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "Empregado"
+msgstr "雇员"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "Usuário"
+msgstr "用户"
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "A principal moeda para a empresa."
+msgstr "这个公司使用的主要货币."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "Adicione empregados à empresa."
+msgstr "为当前公司添加雇员."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Texto a ser exibido no rodapé dos relatórios."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Texto a ser exibido no cabeçalho dos relatórios."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "Usado para computar a data de hoje."
+msgstr "用于计算当前日期."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "A empresa a qual o empregado pertence."
+msgstr "员工所属的公司."
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "Quando o empregado sai da empresa."
+msgstr "当员工离开公司的时间."
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "A pessoa que representa o empregado."
+msgstr "代表雇员的参与者."
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "Quando o empregado entra na empresa."
+msgstr "雇员加入公司的时候."
 
-#, fuzzy
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "A pessoa que representa o empregado."
+msgstr "代表雇员的参与者."
 
-#, fuzzy
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "A pessoa que representa o empregado."
+msgstr "代表雇员的参与者."
 
-#, fuzzy
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "Empresas registradas para este cron"
+msgstr "此计划任务记录的公司。"
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
+"\n"
+"-“公司”作为当前用户的ID列表"
 
-#, fuzzy
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restringe a sequência usada pela empresa."
+msgstr "将序列使用限制为公司。"
 
-#, fuzzy
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "Restringe a sequência usada pela empresa."
+msgstr "将序列使用限制为公司。"
 
-#, fuzzy
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "Adicione empregados para que os usuários tenham acesso a eles."
+msgstr "用户需要访问的公司。"
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "Selecione a empresa a trabalhar para."
+msgstr "选择要为其工作的公司."
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr ""
+msgstr "定义显示的公司的记录。"
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "Selecione o empregado para fazer com que o usuário o represente."
+msgstr "选择一个雇员，好让这个用户对应."
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "Adicione empregados para que os usuários tenham acesso a eles."
+msgstr "添加员工，授予用户访问权限。"
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "公司"
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "Configuração da Empresa"
+msgstr "公司配置"
 
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "Empregado"
+msgstr "雇员"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "Configurar Empresa"
+msgstr "设置公司"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "公司"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "Empregados"
+msgstr "雇员"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr ""
+msgstr "监督者"
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "Carta"
+msgstr "信"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "Cron - Empresa"
+msgstr "计划任务 - 公司"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "Cron - Empresa"
+msgstr "公司中的用户"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "Cron - Empresa"
+msgstr "公司中的用户"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "公司"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "Empresas"
+msgstr "公司"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "Empregados"
+msgstr "雇员"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr ""
+msgstr "公司管理"
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr ""
+msgstr "员工管理"
 
-#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "Cron - Empresa"
+msgstr "用户 - 公司"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "Usuário - Empregado"
+msgstr "用户 - 雇员"
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "Atenciosamente,"
+msgstr "真挚的问候,"
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "Data:"
+msgstr "日期:"
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "Caros senhores e senhoras,"
+msgstr "尊敬的女士们、先生们,"
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "Assunto:"
+msgstr "主题:"
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr ""
+msgstr "所有"
 
-#, fuzzy
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "Moeda"
+msgstr "当前"
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "Você pode agora adicionar sua empresa ao sistema."
+msgstr "现在可以将你的公司添加到系统中了."
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "Relatórios"
+msgstr "报告"
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "Adicionar"
+msgstr "添加"
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "取消"
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "OK"
+msgstr "确定"
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "取消"
```

### Comparing `trytond_company-7.0.0/locale/ro.po` & `trytond_company-7.2.0/locale/ro.po`

 * *Files 3% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "Valută principală al companiei."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Adăugați angajați la companie."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Textul de afișat pe subsolele raportului."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Textul de afișat pe anteturile raportului."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Utilizat pentru calcularea datei de astăzi."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
@@ -167,14 +187,16 @@
 msgstr "Companii înregistrate pentru acest cron."
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
+"\n"
+"-\"companii\" ca o lista de id-uri de la utilizatorul curent"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
 msgstr "Restricționează utilizarea secvenței la companie."
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
```

### Comparing `trytond_company-7.0.0/locale/sl.po` & `trytond_company-7.2.0/locale/sl.po`

 * *Files 5% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "Glavna valuta družbe."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Dodaj družbi zaposlence."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Besedilo za prikaz v nogi poročil."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Besedilo za prikaz v glavi poročil."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Se uporablja za izračun današnjega datuma."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/tr.po` & `trytond_company-7.2.0/locale/fi.po`

 * *Files 7% similar despite different names*

```diff
@@ -131,19 +131,39 @@
 msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
 msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr ""
 
 msgctxt "help:company.employee,company:"
```

### Comparing `trytond_company-7.0.0/locale/uk.po` & `trytond_company-7.2.0/locale/uk.po`

 * *Files 5% similar despite different names*

```diff
@@ -123,20 +123,40 @@
 msgstr "Основна валюта компанії."
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
 msgstr "Додайте працівників до компанії."
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "Текст для відображення в нижніх колонтитулах звіту."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "Текст для відображення в заголовках звітів."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
 msgstr "Використовується для обчислення поточної дати."
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
```

### Comparing `trytond_company-7.0.0/locale/zh_CN.po` & `trytond_company-7.2.0/locale/tr.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,323 +1,354 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:company.company,currency:"
 msgid "Currency"
-msgstr "货币"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:company.company,employees:"
 msgid "Employees"
-msgstr "雇员"
+msgstr "Employees"
 
 msgctxt "field:company.company,footer:"
 msgid "Footer"
-msgstr "页脚"
+msgstr ""
 
 msgctxt "field:company.company,header:"
 msgid "Header"
-msgstr "页眉"
+msgstr ""
 
 msgctxt "field:company.company,party:"
 msgid "Party"
-msgstr "参与者"
+msgstr ""
 
 msgctxt "field:company.company,timezone:"
 msgid "Timezone"
-msgstr "时区"
+msgstr ""
 
 msgctxt "field:company.employee,company:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
 msgctxt "field:company.employee,end_date:"
 msgid "End Date"
-msgstr "离职日期"
+msgstr ""
 
 msgctxt "field:company.employee,party:"
 msgid "Party"
-msgstr "参与者"
+msgstr ""
 
 msgctxt "field:company.employee,start_date:"
 msgid "Start Date"
-msgstr "入职日期"
+msgstr ""
 
 msgctxt "field:company.employee,subordinates:"
 msgid "Subordinates"
-msgstr "下级"
+msgstr ""
 
 msgctxt "field:company.employee,supervisor:"
 msgid "Supervisor"
-msgstr "监督者"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:ir.cron,companies:"
 msgid "Companies"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "field:ir.cron-company.company,company:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
 msgctxt "field:ir.cron-company.company,cron:"
 msgid "Cron"
-msgstr "计划任务"
+msgstr ""
 
 msgctxt "field:ir.sequence,company:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
 msgctxt "field:ir.sequence.strict,company:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
 msgctxt "field:party.configuration.party_lang,company:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:party.contact_mechanism.language,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "field:party.party.lang,company:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:res.user,companies:"
 msgid "Companies"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "field:res.user,company:"
 msgid "Current Company"
-msgstr "当前公司"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:res.user,company_filter:"
 msgid "Company Filter"
-msgstr "公司过滤器"
+msgstr "Companies"
 
 msgctxt "field:res.user,employee:"
 msgid "Current Employee"
-msgstr "现任员工"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:res.user,employees:"
 msgid "Employees"
-msgstr "雇员"
+msgstr "Employees"
 
+#, fuzzy
 msgctxt "field:res.user-company.company,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "field:res.user-company.company,user:"
 msgid "User"
-msgstr "用户"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:res.user-company.employee,employee:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Employees"
 
 msgctxt "field:res.user-company.employee,user:"
 msgid "User"
-msgstr "用户"
+msgstr ""
 
 msgctxt "help:company.company,currency:"
 msgid "The main currency for the company."
-msgstr "这个公司使用的主要货币."
+msgstr ""
 
 msgctxt "help:company.company,employees:"
 msgid "Add employees to the company."
-msgstr "为当前公司添加雇员."
+msgstr ""
 
 msgctxt "help:company.company,footer:"
-msgid "The text to display on report footers."
-msgstr "要在报告页脚上显示的文本."
+msgid ""
+"The text to display on report footers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,header:"
-msgid "The text to display on report headers."
-msgstr "要在报告页眉上显示的文本."
+msgid ""
+"The text to display on report headers.\n"
+"The following placeholders can be used:\n"
+"- ${name}\n"
+"- ${phone}\n"
+"- ${mobile}\n"
+"- ${fax}\n"
+"- ${email}\n"
+"- ${website}\n"
+"- ${address}\n"
+"- ${tax_identifier}\n"
+msgstr ""
 
 msgctxt "help:company.company,timezone:"
 msgid "Used to compute the today date."
-msgstr "用于计算当前日期."
+msgstr ""
 
 msgctxt "help:company.employee,company:"
 msgid "The company to which the employee belongs."
-msgstr "员工所属的公司."
+msgstr ""
 
 msgctxt "help:company.employee,end_date:"
 msgid "When the employee leaves the company."
-msgstr "当员工离开公司的时间."
+msgstr ""
 
 msgctxt "help:company.employee,party:"
 msgid "The party which represents the employee."
-msgstr "代表雇员的参与者."
+msgstr ""
 
 msgctxt "help:company.employee,start_date:"
 msgid "When the employee joins the company."
-msgstr "雇员加入公司的时候."
+msgstr ""
 
 msgctxt "help:company.employee,subordinates:"
 msgid "The employees to be overseen by this employee."
-msgstr "代表雇员的参与者."
+msgstr ""
 
 msgctxt "help:company.employee,supervisor:"
 msgid "The employee who oversees this employee."
-msgstr "代表雇员的参与者."
+msgstr ""
 
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
-msgstr "此计划任务记录的公司。"
+msgstr ""
 
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
-"\n"
-"-“公司”作为当前用户的ID列表"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "将序列使用限制为公司。"
+msgstr ""
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
-msgstr "将序列使用限制为公司。"
+msgstr ""
 
 msgctxt "help:res.user,companies:"
 msgid "The companies that the user has access to."
-msgstr "用户需要访问的公司。"
+msgstr ""
 
 msgctxt "help:res.user,company:"
 msgid "Select the company to work for."
-msgstr "选择要为其工作的公司."
+msgstr ""
 
 msgctxt "help:res.user,company_filter:"
 msgid "Define records of which companies are shown."
-msgstr "定义显示的公司的记录。"
+msgstr ""
 
 msgctxt "help:res.user,employee:"
 msgid "Select the employee to make the user behave as such."
-msgstr "选择一个雇员，好让这个用户对应."
+msgstr ""
 
 msgctxt "help:res.user,employees:"
 msgid "Add employees to grant the user access to them."
-msgstr "添加员工，授予用户访问权限。"
+msgstr ""
 
 msgctxt "model:company.company,name:"
 msgid "Company"
-msgstr "公司"
+msgstr ""
 
 msgctxt "model:company.company.config.start,name:"
 msgid "Company Config"
-msgstr "公司配置"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:company.employee,name:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Employees"
 
 msgctxt "model:ir.action,name:act_company_config"
 msgid "Configure Company"
-msgstr "设置公司"
+msgstr "Configure Company"
 
 msgctxt "model:ir.action,name:act_company_list"
 msgid "Companies"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "model:ir.action,name:act_employee_form"
 msgid "Employees"
-msgstr "雇员"
+msgstr "Employees"
 
 msgctxt "model:ir.action,name:act_employee_subordinates"
 msgid "Supervised by"
-msgstr "监督者"
+msgstr ""
 
 msgctxt "model:ir.action,name:report_letter"
 msgid "Letter"
-msgstr "信"
+msgstr "Letter"
 
 msgctxt "model:ir.cron-company.company,name:"
 msgid "Cron - Company"
-msgstr "计划任务 - 公司"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Companies"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Companies"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
-msgstr "公司"
+msgstr "Companies"
 
 msgctxt "model:ir.ui.menu,name:menu_employee_form"
 msgid "Employees"
-msgstr "雇员"
+msgstr "Employees"
 
 msgctxt "model:res.group,name:group_company_admin"
 msgid "Company Administration"
-msgstr "公司管理"
+msgstr ""
 
 msgctxt "model:res.group,name:group_employee_admin"
 msgid "Employee Administration"
-msgstr "员工管理"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:res.user-company.company,name:"
 msgid "User - Company"
-msgstr "用户 - 公司"
+msgstr "Companies"
 
 msgctxt "model:res.user-company.employee,name:"
 msgid "User - Employee"
-msgstr "用户 - 雇员"
+msgstr ""
 
 msgctxt "report:party.letter:"
 msgid "Best Regards,"
-msgstr "真挚的问候,"
+msgstr ""
 
 msgctxt "report:party.letter:"
 msgid "Date:"
-msgstr "日期:"
+msgstr ""
 
 msgctxt "report:party.letter:"
 msgid "Dear Madams and Sirs,"
-msgstr "尊敬的女士们、先生们,"
+msgstr ""
 
 msgctxt "report:party.letter:"
 msgid "Subject:"
-msgstr "主题:"
+msgstr ""
 
 msgctxt "selection:res.user,company_filter:"
 msgid "All"
-msgstr "所有"
+msgstr ""
 
 msgctxt "selection:res.user,company_filter:"
 msgid "Current"
-msgstr "当前"
+msgstr ""
 
 msgctxt "view:company.company.config.start:"
 msgid "You can now add your company into the system."
-msgstr "现在可以将你的公司添加到系统中了."
+msgstr ""
 
 msgctxt "view:company.company:"
 msgid "Reports"
-msgstr "报告"
+msgstr ""
 
 msgctxt "wizard_button:company.company.config,company,add:"
 msgid "Add"
-msgstr "添加"
+msgstr ""
 
 msgctxt "wizard_button:company.company.config,company,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr ""
 
 msgctxt "wizard_button:company.company.config,start,company:"
 msgid "OK"
-msgstr "确定"
+msgstr ""
 
 msgctxt "wizard_button:company.company.config,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_company-7.0.0/model.py` & `trytond_company-7.2.0/model.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/party.py` & `trytond_company-7.2.0/party.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,19 @@
     def check_erase(self, party):
         pool = Pool()
         Party = pool.get('party.party')
         Company = pool.get('company.company')
 
         super().check_erase(party)
 
-        with Transaction().set_user(0):
-            companies = Company.search([])
-            for company in companies:
-                with Transaction().set_context(company=company.id):
-                    party = Party(party.id)
-                    self.check_erase_company(party, company)
+        companies = Company.search([])
+        for company in companies:
+            with Transaction().set_context(company=company.id):
+                party = Party(party.id)
+                self.check_erase_company(party, company)
 
     def check_erase_company(self, party, company):
         pass
 
 
 class ContactMechanism(CompanyMultiValueMixin, metaclass=PoolMeta):
     __name__ = 'party.contact_mechanism'
```

### Comparing `trytond_company-7.0.0/res.py` & `trytond_company-7.2.0/res.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,16 +193,15 @@
         Return an ordered tuple of company ids for the user
         '''
         transaction = Transaction()
         user_id = transaction.user
         companies = cls._get_companies_cache.get(user_id)
         if companies is not None:
             return companies
-        with transaction.set_user(0):
-            user = cls(user_id)
+        user = cls(user_id)
         if user.company_filter == 'one':
             companies = [user.company.id] if user.company else []
         elif user.company_filter == 'all':
             companies = [c.id for c in user.companies]
         else:
             companies = []
         companies = tuple(companies)
@@ -215,16 +214,15 @@
         Return an ordered tuple of employee ids for the user
         '''
         transaction = Transaction()
         user_id = transaction.user
         employees = cls._get_employees_cache.get(user_id)
         if employees is not None:
             return employees
-        with transaction.set_user(0):
-            user = cls(user_id)
+        user = cls(user_id)
         if user.company_filter == 'one':
             employees = [user.employee.id] if user.employee else []
         elif user.company_filter == 'all':
             employees = [e.id for e in user.employees]
         else:
             employees = []
         employees = tuple(employees)
```

### Comparing `trytond_company-7.0.0/setup.py` & `trytond_company-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-company/',
+        "Documentation": 'https://docs.tryton.org/modules-company/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton company employee',
     package_dir={'trytond.modules.company': '.'},
     packages=(
         ['trytond.modules.company']
```

### Comparing `trytond_company-7.0.0/tests/test_module.py` & `trytond_company-7.2.0/tests/test_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
+import datetime as dt
 from collections import defaultdict
 from contextlib import contextmanager
 
 from trytond.model import ModelStorage, ModelView
 from trytond.modules.company.model import CompanyMultiValueMixin
 from trytond.modules.currency.tests import add_currency_rate, create_currency
 from trytond.modules.party.tests import PartyCheckEraseMixin
@@ -126,22 +127,22 @@
                 if (field._type == 'many2one'
                         and issubclass(field.get_target(), Company)):
                     to_check[fname].add(mname)
 
         for fname, models in to_check.items():
             rules = Rule.search([
                     ('rule_group', 'where', [
-                            ('model.model', 'in', list(models)),
+                            ('model', 'in', list(models)),
                             ('global_p', '=', True),
                             ('perm_read', '=', True),
                             ]),
                     ('domain', '=', PYSONEncoder(sort_keys=True).encode(
                             [(fname, 'in', Eval('companies', []))])),
                     ])
-            with_rules = {r.rule_group.model.model for r in rules}
+            with_rules = {r.rule_group.model for r in rules}
             self.assertGreaterEqual(with_rules, models,
                 msg='Models %(models)s are missing a global rule '
                 'for field "%(field)s"' % {
                     'models': ', '.join(
                         f'"{m}"' for m in (models - with_rules)),
                     'field': fname,
                     })
@@ -301,9 +302,114 @@
         root.save()
 
         with transaction.set_user(0):
             with Transaction().set_context(employee=employee.id):
                 root = User(0)
                 self.assertEqual(root.employee, employee)
 
+    @with_transaction()
+    def test_company_header(self):
+        "Test company header"
+        company = create_company()
+        company.party.email = 'company@example.com'
+        company.party.save()
+        company.header = "${name} - ${email}"
+        company.save()
+
+        self.assertEqual(
+            company.header_used, "Dunder Mifflin - company@example.com")
+
+    @with_transaction()
+    def test_company_footer(self):
+        "Test company footer"
+        company = create_company()
+        company.party.email = 'company@example.com'
+        company.party.save()
+        company.footer = "${name} - ${email}"
+        company.save()
+
+        self.assertEqual(
+            company.footer_used, "Dunder Mifflin - company@example.com")
+
+    @with_transaction()
+    def test_employee_active_no_dates(self):
+        "Test employee active with dates"
+        pool = Pool()
+        Employee = pool.get('company.employee')
+
+        company = create_company()
+        employee = create_employee(company, "Jim Halper")
+
+        self.assertEqual(employee.active, True)
+        self.assertEqual(Employee.search([
+                    ('active', '=', True),
+                    ]), [employee])
+        self.assertEqual(Employee.search([
+                    ('active', '!=', False),
+                    ]), [employee])
+        self.assertEqual(Employee.search([
+                    ('active', '=', False),
+                    ]), [])
+        self.assertEqual(Employee.search([
+                    ('active', '!=', True),
+                    ]), [])
+
+    @with_transaction()
+    def test_employee_active_start_date(self):
+        "Test employee active with start date"
+        pool = Pool()
+        Employee = pool.get('company.employee')
+
+        company = create_company()
+        employee = create_employee(company, "Jim Halper")
+        employee.start_date = dt.date.today()
+        employee.save()
+
+        with Transaction().set_context(date=employee.start_date):
+            self.assertEqual(Employee(employee).active, True)
+            self.assertEqual(Employee.search([
+                        ('active', '=', True),
+                        ]), [employee])
+        with Transaction().set_context(
+                date=employee.start_date - dt.timedelta(days=1)):
+            self.assertEqual(Employee(employee).active, False)
+            self.assertEqual(Employee.search([
+                        ('active', '=', True),
+                        ]), [])
+        with Transaction().set_context(
+                date=employee.start_date + dt.timedelta(days=1)):
+            self.assertEqual(Employee(employee).active, True)
+            self.assertEqual(Employee.search([
+                        ('active', '=', True),
+                        ]), [employee])
+
+    @with_transaction()
+    def test_employee_active_end_date(self):
+        "Test employee active with end date"
+        pool = Pool()
+        Employee = pool.get('company.employee')
+
+        company = create_company()
+        employee = create_employee(company, "Jim Halper")
+        employee.end_date = dt.date.today()
+        employee.save()
+
+        with Transaction().set_context(date=employee.end_date):
+            self.assertEqual(Employee(employee).active, True)
+            self.assertEqual(Employee.search([
+                        ('active', '=', True),
+                        ]), [employee])
+        with Transaction().set_context(
+                date=employee.end_date - dt.timedelta(days=1)):
+            self.assertEqual(Employee(employee).active, True)
+            self.assertEqual(Employee.search([
+                        ('active', '=', True),
+                        ]), [employee])
+        with Transaction().set_context(
+                date=employee.end_date + dt.timedelta(days=1)):
+            self.assertEqual(Employee(employee).active, False)
+            self.assertEqual(Employee.search([
+                        ('active', '=', True),
+                        ]), [])
+
 
 del ModuleTestCase
```

### Comparing `trytond_company-7.0.0/tests/tools.py` & `trytond_company-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/tox.ini` & `trytond_company-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/trytond_company.egg-info/PKG-INFO` & `trytond_company-7.2.0/trytond_company.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-company
-Version: 7.0.0
+Name: trytond_company
+Version: 7.2.0
 Summary: Tryton module with companies and employees
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-company/
+Project-URL: Documentation, https://docs.tryton.org/modules-company/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton company employee
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,17 +49,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 ##############
 Company Module
 ##############
 
 The *Company Module* allows the business that is using Tryton to be
 represented inside Tryton.
```

### Comparing `trytond_company-7.0.0/trytond_company.egg-info/SOURCES.txt` & `trytond_company-7.2.0/trytond_company.egg-info/SOURCES.txt`

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
 company.py
```

### Comparing `trytond_company-7.0.0/view/company_form.xml` & `trytond_company-7.2.0/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/view/user_form.xml` & `trytond_company-7.2.0/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-7.0.0/view/user_form_preferences.xml` & `trytond_company-7.2.0/view/user_form_preferences.xml`

 * *Files identical despite different names*

