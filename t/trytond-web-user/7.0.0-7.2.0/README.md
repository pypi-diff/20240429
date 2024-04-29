# Comparing `tmp/trytond_web_user-7.0.0.tar.gz` & `tmp/trytond_web_user-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_user-7.0.0.tar", last modified: Mon Oct 30 17:45:45 2023, max compression
+gzip compressed data, was "trytond_web_user-7.2.0.tar", last modified: Mon Apr 29 15:54:37 2024, max compression
```

## Comparing `trytond_web_user-7.0.0.tar` & `trytond_web_user-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:45.936657 trytond_web_user-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      197 2023-10-22 17:23:30.000000 trytond_web_user-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1671 2023-10-30 17:16:47.000000 trytond_web_user-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:16:47.000000 trytond_web_user-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_web_user-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3547 2023-10-30 17:45:45.936657 trytond_web_user-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1147 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:45.936657 trytond_web_user-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2809 2023-10-22 17:23:30.000000 trytond_web_user-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1147 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:30.000000 trytond_web_user-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1483 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/email_validation.html
--rw-r--r--   0 ced       (1000) ced       (1000)      253 2023-10-07 15:40:36.000000 trytond_web_user-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:45.933324 trytond_web_user-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4382 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5065 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4135 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5201 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5170 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3909 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4327 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5507 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4135 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5150 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4828 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4451 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4205 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4906 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4135 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4734 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4028 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4335 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4135 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5668 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4845 2023-10-30 16:47:45.000000 trytond_web_user-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-10-07 15:40:36.000000 trytond_web_user-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:45:45.936657 trytond_web_user-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4316 2023-10-27 17:38:49.000000 trytond_web_user-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:45.933324 trytond_web_user-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6682 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_web_user-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       83 2023-10-30 17:16:42.000000 trytond_web_user-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:45.936657 trytond_web_user-7.0.0/trytond_web_user.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3547 2023-10-30 17:45:45.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-10-30 17:45:45.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:45:45.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-10-30 17:45:45.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:45:45.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:45:45.000000 trytond_web_user-7.0.0/trytond_web_user.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    18273 2023-10-07 15:40:36.000000 trytond_web_user-7.0.0/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2023-04-15 07:12:15.000000 trytond_web_user-7.0.0/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:45.933324 trytond_web_user-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-08-13 15:26:13.000000 trytond_web_user-7.0.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-08-13 15:26:13.000000 trytond_web_user-7.0.0/view/user_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2096 2024-04-29 15:30:21.000000 trytond_web_user-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:30:21.000000 trytond_web_user-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_web_user-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.430499 trytond_web_user-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      946 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1615 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:14:37.000000 trytond_web_user-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:40.000000 trytond_web_user-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1690 2024-04-22 12:14:36.000000 trytond_web_user-7.2.0/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/email_validation.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      253 2024-02-04 18:51:27.000000 trytond_web_user-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4621 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5227 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5355 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5325 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4148 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4528 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5624 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5298 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4993 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4623 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4635 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6395 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4444 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5051 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4904 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5133 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4574 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5225 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4374 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5781 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5031 2024-04-29 13:17:17.000000 trytond_web_user-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-02-04 18:51:27.000000 trytond_web_user-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4475 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_user-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6663 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:40.000000 trytond_web_user-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       83 2024-04-29 15:30:17.000000 trytond_web_user-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/trytond_web_user.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1579 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:37.000000 trytond_web_user-7.2.0/trytond_web_user.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    18214 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4701 2024-04-27 16:30:39.000000 trytond_web_user-7.2.0/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:37.433833 trytond_web_user-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2024-01-27 09:58:52.000000 trytond_web_user-7.2.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-01-27 09:58:52.000000 trytond_web_user-7.2.0/view/user_list.xml
```

### Comparing `trytond_web_user-7.0.0/CHANGELOG` & `trytond_web_user-7.2.0/CHANGELOG`

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
@@ -12,52 +17,64 @@
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add expire delay in reset password email
 
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
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 * Add secondary parties on user
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.0.0 - 2018-10-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 2.7
 * Add remove and reset session methods
 
 Version 4.8.0 - 2018-04-23
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Erase user email when party is erased
 * Require email only for active user
 * Add maximum authentication attempt
 
 Version 4.6.0 - 2017-10-30
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Increase session randomness to 32 bytes
 * Manage email case insensitively
 
 Version 4.4.0 - 2017-05-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.2.0 - 2016-11-28
+--------------------------
 * Initial release
```

### Comparing `trytond_web_user-7.0.0/COPYRIGHT` & `trytond_web_user-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2016-2023 Cédric Krier
-Copyright (C) 2016-2023 B2CK
+Copyright (C) 2016-2024 Cédric Krier
+Copyright (C) 2016-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_web_user-7.0.0/LICENSE` & `trytond_web_user-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/__init__.py` & `trytond_web_user-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/doc/conf.py` & `trytond_web_user-7.2.0/doc/conf.py`

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

### Comparing `trytond_web_user-7.0.0/email_reset_password.html` & `trytond_web_user-7.2.0/email_reset_password.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,29 @@
         <title>Reset Password</title>
     </head>
     <body>
         <py:for each="user in records">
         <div style="display: block; text-align: center">
             <div>
                 <h1>Reset Password</h1>
-                <p i18n:msg="email">We received a request to reset the password for your account: ${user.email}</p>
+                <p i18n:msg="email,url">
+                Hello, we received a request to reset the password for the account associated with <strong>${user.email}</strong>. No changes have been made to your account yet.<br/>
+                You can reset your password by clicking the link below:<br/>
                 <a href="${user.get_email_reset_password_url()}"
-                   style="display: block; text-decoration: none; width: max-content; margin: 0 auto; padding: 0.5em 1em; font-size:2em; border: 1px solid #2E6DA4; border-radius: 4px; color: #FFF; background-color: #337AB7;">
+                   style="display: block; text-decoration: none; width: max-content; margin: 0.5em auto; padding: 0.5em 1em; font-size:1em; border: 1px solid #2E6DA4; border-radius: 4px; color: #FFF; background-color: #337AB7;">
                     Reset Password
                 </a>
+                </p>
             </div>
             <hr style="margin-top: 20px; border-style: solid none none; border-color: #EEE"></hr>
             <div style="font-size: 80%; color: #777">
                 <p i18n:msg="datetime,expire_delay">
                 The link will expire in <time datetime="${record.reset_password_token_expire.isoformat()}">${format_timedelta(expire_delay)}</time>.
                 </p>
-                <p>Button is not working? Paste this into your browser:</p>
+                <p>Button not working? Paste this into your browser:</p>
                 <p>${user.get_email_reset_password_url()}</p>
                 <p>If you didn't make this request, you can ignore this email.</p>
             </div>
         </div>
         </py:for>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
 ************ RReesseett PPaasssswwoorrdd ************
-We received a request to reset the password for your account: ${user.email}
+Hello, we received a request to reset the password for the account associated
+with $${{uusseerr..eemmaaiill}}. No changes have been made to your account yet.
+You can reset your password by clicking the link below:
 _R_e_s_e_t_ _P_a_s_s_w_o_r_d
 ===============================================================================
 The link will expire in ${format_timedelta(expire_delay)}.
-Button is not working? Paste this into your browser:
+Button not working? Paste this into your browser:
 ${user.get_email_reset_password_url()}
 If you didn't make this request, you can ignore this email.
```

### Comparing `trytond_web_user-7.0.0/email_validation.html` & `trytond_web_user-7.2.0/email_validation.html`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/ir.py` & `trytond_web_user-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/locale/bg.po` & `trytond_web_user-7.2.0/locale/it.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:web.user,email:"
 msgid "E-mail"
-msgstr ""
+msgstr "E-mail"
 
+#, fuzzy
 msgctxt "field:web.user,email_token:"
 msgid "E-mail Token"
-msgstr ""
+msgstr "_E-Mail..."
 
+#, fuzzy
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
-msgstr ""
+msgstr "_E-Mail..."
 
-#, fuzzy
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Управление на партньор"
+msgstr "Controparte"
 
 #, fuzzy
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr "Парола"
+msgstr "Password"
 
+#, fuzzy
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
-msgstr ""
+msgstr "Hash della Password"
 
+#, fuzzy
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
-msgstr ""
+msgstr "Reset Password"
 
+#, fuzzy
 msgctxt "field:web.user,reset_password_token_expire:"
 msgid "Reset Password Token Expire"
-msgstr ""
+msgstr "Reset Password"
 
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Управление на партньор"
+msgstr "Controparte"
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Потребител"
+msgstr "Utente"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr ""
+msgstr "Indirizzo IP"
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
-msgstr "Потребителско име"
+msgstr "Login"
 
 #, fuzzy
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr "Ключ"
+msgstr "Chiave"
 
 #, fuzzy
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr "Потребител"
+msgstr "Utente"
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
 msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
@@ -119,28 +123,39 @@
 msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
 msgstr "Web Users"
 
+#, fuzzy
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
-msgstr ""
+msgstr "Sessione"
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
+msgstr "Sessione"
+
+msgctxt "report:web.user.email_reset_password:"
+msgid "Button not working? Paste this into your browser:"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 
 #, fuzzy
@@ -148,19 +163,14 @@
 msgid "Reset Password"
 msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
@@ -174,18 +184,17 @@
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
-#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
-msgstr "Проверка"
+msgstr "Verifica"
 
 #, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
 msgstr "Reset Password"
 
 #, fuzzy
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_web_user-7.0.0/locale/ca.po` & `trytond_web_user-7.2.0/locale/ca.po`

 * *Files 5% similar despite different names*

```diff
@@ -122,37 +122,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Intent d'autenticació usuari web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Sessió usuari web"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "El botó no funciona? Empega això al teu navegador:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Si no heu fet aquesta petició, podeu ignorar aquest correu."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Restableix la contrasenya"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "L'enllaç caducarà en [1:%(datetime)s]."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-"Hem rebut una petició per restablir la contrasenya del vostre compte: "
-"%(email)s"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "El botó no funciona? Empega això al teu navegador:"
```

### Comparing `trytond_web_user-7.0.0/locale/cs.po` & `trytond_web_user-7.2.0/locale/es_419.po`

 * *Files 11% similar despite different names*

```diff
@@ -38,18 +38,17 @@
 msgid "Secondary Parties"
 msgstr ""
 
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Web Users"
+msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
@@ -69,28 +68,27 @@
 
 msgctxt "field:web.user.session,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
-msgstr "Web Users"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
-msgstr "Web Users"
+msgstr ""
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr ""
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
-msgstr "Email Validation"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_unique"
 msgid "E-mail of active web user must be unique."
@@ -98,90 +96,89 @@
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
-msgstr "Validate E-mail"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
-msgstr "Web Users"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
-msgstr "Web Users"
+msgstr ""
 
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
 msgstr ""
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "If you didn't make this request, you can ignore this email."
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid "If you didn't make this request, you can ignore this email."
+msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "The link will expire in [1:%(datetime)s]."
+msgid "Reset Password"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
+msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Email Validation"
-msgstr "Email Validation"
+msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:web.user:"
 msgid "Validate E-mail"
-msgstr "Validate E-mail"
+msgstr ""
```

### Comparing `trytond_web_user-7.0.0/locale/de.po` & `trytond_web_user-7.2.0/locale/de.po`

 * *Files 5% similar despite different names*

```diff
@@ -124,41 +124,44 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Webbenutzer Authentifizierungsversuch"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Webbenutzer Sitzung"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr ""
 "Wenn der Button nicht funktioniert, kopieren Sie bitte die folgende Zeile in"
 " die Adresszeile Ihres Browsers:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Ignorieren Sie bitte diese E-Mail, wenn Sie nicht der Urheber dieser Anfrage"
 " sind."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Passwort zurücksetzen"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "Der Hyperlink wird in [1:%(datetime)s] ablaufen."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-"Wir haben eine Anfrage zur Rücksetzung des Passworts für Ihr Konto erhalten:"
-" %(email)s"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
```

### Comparing `trytond_web_user-7.0.0/locale/es.po` & `trytond_web_user-7.2.0/locale/es.po`

 * *Files 6% similar despite different names*

```diff
@@ -122,39 +122,42 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Intento de identificación usuario web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Sesión usuario web"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "¿El botón no funciona? Pega esto en tu navegador:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Si no habéis realizado esta petición, podéis ignorar este correo "
 "electrónico."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Restablecer contraseña"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "El enlace caducará en [1:%(datetime)s]."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-"Hemos recibido una solicitud para reiniciar la contraseña de vuestra cuenta:"
-" %(email)s"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "¿El botón no funciona? Pega esto en tu navegador:"
```

### Comparing `trytond_web_user-7.0.0/locale/es_419.po` & `trytond_web_user-7.2.0/locale/cs.po`

 * *Files 18% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 msgid "Secondary Parties"
 msgstr ""
 
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr ""
+msgstr "Web Users"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
@@ -68,27 +69,28 @@
 
 msgctxt "field:web.user.session,user:"
 msgid "User"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
-msgstr ""
+msgstr "Web Users"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
-msgstr ""
+msgstr "Web Users"
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr ""
+msgstr "Reset Password"
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
-msgstr ""
+msgstr "Email Validation"
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_unique"
 msgid "E-mail of active web user must be unique."
@@ -96,85 +98,94 @@
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr ""
+msgstr "Reset Password"
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
-msgstr ""
+msgstr "Validate E-mail"
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
-msgstr ""
+msgstr "Web Users"
 
+#, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
-msgstr ""
+msgstr "Web Users"
 
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
 msgstr ""
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "If you didn't make this request, you can ignore this email."
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Reset Password"
+msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "The link will expire in [1:%(datetime)s]."
-msgstr ""
+msgid "Reset Password"
+msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
+msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Email Validation"
-msgstr ""
+msgstr "Email Validation"
 
 msgctxt "report:web.user.email_validation:"
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
-msgstr ""
+msgstr "Reset Password"
 
+#, fuzzy
 msgctxt "view:web.user:"
 msgid "Validate E-mail"
-msgstr ""
+msgstr "Validate E-mail"
```

### Comparing `trytond_web_user-7.0.0/locale/et.po` & `trytond_web_user-7.2.0/locale/fi.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,96 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:web.user,email:"
 msgid "E-mail"
-msgstr "E-kiri"
+msgstr ""
 
 msgctxt "field:web.user,email_token:"
 msgid "E-mail Token"
 msgstr ""
 
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
 msgstr ""
 
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr ""
 
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr "Salasõna"
+msgstr ""
 
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
-msgstr "Salasõna räsi"
+msgstr ""
 
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
 msgstr ""
 
 msgctxt "field:web.user,reset_password_token_expire:"
 msgid "Reset Password Token Expire"
 msgstr ""
 
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Kasutaja"
+msgstr "Web Users"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr "IP-aadress"
+msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
-msgstr "IP-võrk"
+msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
-msgstr "Logi sisse"
+msgstr ""
 
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr "Võti"
+msgstr ""
 
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr "Kasutaja"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
-msgstr ""
+msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
-msgstr "Muutja"
+msgstr "Web Users"
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr "Lähtesta salasõna"
+msgstr "Reset Password"
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
-msgstr ""
+msgstr "Email Validation"
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_unique"
 msgid "E-mail of active web user must be unique."
@@ -99,86 +98,94 @@
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr "Lähtesta salasõna"
+msgstr "Reset Password"
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
-msgstr ""
+msgstr "Validate E-mail"
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
-msgstr ""
+msgstr "Web Users"
 
+#, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
-msgstr ""
+msgstr "Web Users"
 
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
 msgstr ""
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
-msgstr "Nupp ei tööta? Aseta see link brauseri aadressreale:"
+msgid "Button not working? Paste this into your browser:"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
-msgstr "Kui sa ei teinud seda päringut, siis ignoreeri seda e-kirja."
+msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
-msgstr "Lähtesta salasõna"
+msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-#, fuzzy
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "Saime teate salasõna lähtestamiseks,"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
-msgstr "Nupp ei tööta? Aseta see link brauseri aadressreale:"
+msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Email Validation"
-msgstr ""
+msgstr "Email Validation"
 
 msgctxt "report:web.user.email_validation:"
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
-msgstr "Lähtesta salasõna"
+msgstr "Reset Password"
 
+#, fuzzy
 msgctxt "view:web.user:"
 msgid "Validate E-mail"
-msgstr ""
+msgstr "Validate E-mail"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_web_user-7.0.0/locale/fa.po` & `trytond_web_user-7.2.0/locale/fa.po`

 * *Files 6% similar despite different names*

```diff
@@ -126,36 +126,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "تلاش برای هوّیت سنجی کاربر وب"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "جلسه کاری کاربر وب"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "دکمه کار نمی کند؟ این آدرس را در مرورگر خود مرور کنید:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "اگراین درخواست را نکرده باشید، می توانید این ایمیل را نادیده بگیرید."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "بازنشانی کلمه عبور"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-#, fuzzy
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "مایک درخواست برای بازنشانی کلمه عبور حساب کاربری شما دریافت کردیم،"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "دکمه کار نمی کند؟ این آدرس را در مرورگر خود مرور کنید:"
```

### Comparing `trytond_web_user-7.0.0/locale/fi.po` & `trytond_web_user-7.2.0/locale/pl.po`

 * *Files 12% similar despite different names*

```diff
@@ -126,15 +126,24 @@
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 
 #, fuzzy
@@ -142,19 +151,14 @@
 msgid "Reset Password"
 msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
```

### Comparing `trytond_web_user-7.0.0/locale/fr.po` & `trytond_web_user-7.2.0/locale/fr.po`

 * *Files 8% similar despite different names*

```diff
@@ -122,38 +122,41 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Tentative d'authentification d'utilisateur web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Session d'utilisateur web"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "Le bouton ne fonctionne pas ? Copier ceci dans votre navigateur :"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Si vous n'avez pas fait cette demande, vous pouvez ignorer cet E-mail."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Réinitialiser le mot de passe"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "Le lien expirera dans [1:%(datetime)s]."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-"Nous avons reçu une demande de réinitialisation du mot de passe de votre "
-"compte : %(email)s"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "Le bouton ne fonctionne pas ? Copier ceci dans votre navigateur :"
```

### Comparing `trytond_web_user-7.0.0/locale/hu.po` & `trytond_web_user-7.2.0/locale/hu.po`

 * *Files 4% similar despite different names*

```diff
@@ -123,38 +123,42 @@
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "A gomb nem működik? Másolja be ezt a böngészőjébe:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 "Ha nem Ön küldte ezt a kérés, akkor nyugodtan hagyja figyelmen kívül ezt az "
 "e-mailt."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Jelszó visszaállítása"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-#, fuzzy
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "Kaptunk egy kérést, hogy állítsuk vissza a felhasználója jelszavát,"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "A gomb nem működik? Másolja be ezt a böngészőjébe:"
```

### Comparing `trytond_web_user-7.0.0/locale/id.po` & `trytond_web_user-7.2.0/locale/lt.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:web.user,email:"
 msgid "E-mail"
-msgstr "E-mail"
+msgstr ""
 
 msgctxt "field:web.user,email_token:"
 msgid "E-mail Token"
 msgstr ""
 
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
 msgstr ""
 
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Pihak"
+msgstr "Kontrahentas"
 
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr "Kata sandi"
+msgstr ""
 
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
 msgstr ""
 
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
@@ -37,61 +37,61 @@
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Pihak"
+msgstr "Kontrahentas"
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Pengguna"
+msgstr "Naudotojas"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr "Alamat IP"
+msgstr "IP adresas"
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
 msgstr ""
 
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr "Kunci"
+msgstr ""
 
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr "Pengguna"
+msgstr "Naudotojas"
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
-msgstr "Pengguna Web"
+msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
-msgstr "Pengguna Web"
+msgstr "Web Users"
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr "Atur Ulang Kata Sandi"
+msgstr "Atstatyti slaptažodį"
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
-msgstr ""
+msgstr "Email Validation"
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_unique"
 msgid "E-mail of active web user must be unique."
@@ -99,86 +99,94 @@
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr "Atur Ulang Kata Sandi"
+msgstr "Atstatyti slaptažodį"
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
-msgstr ""
+msgstr "Validate E-mail"
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
-msgstr ""
+msgstr "Web Users"
 
+#, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
-msgstr ""
+msgstr "Web Users"
 
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
 msgstr ""
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
-msgstr "Tombol tidak berfungsi? Lekatkan ini pada browser Anda:"
+msgid "Button not working? Paste this into your browser:"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
-msgstr "Jika bukan Anda yang membuat permintaan ini, abaikan email ini."
+msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
-msgstr "Atur Ulang Kata Sandi"
+msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-#, fuzzy
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "Kami menerima permintaan untuk mengatur ulang kata sandi akun Anda,"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
-msgstr "Tombol tidak berfungsi? Lekatkan ini pada browser Anda:"
+msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Email Validation"
-msgstr "Validasi Email"
+msgstr "Email Validation"
 
 msgctxt "report:web.user.email_validation:"
 msgid "If you received this email by mistake, just ignore it."
-msgstr "Jika Anda menerima email ini karena kesalahan, abaikan saja."
+msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
-msgstr "Tinggal satu langkah lagi..."
+msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
-msgstr "Atur Ulang Kata Sandi"
+msgstr "Reset Password"
 
+#, fuzzy
 msgctxt "view:web.user:"
 msgid "Validate E-mail"
-msgstr ""
+msgstr "Validate E-mail"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_web_user-7.0.0/locale/it.po` & `trytond_web_user-7.2.0/locale/bg.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,85 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:web.user,email:"
 msgid "E-mail"
-msgstr "E-mail"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user,email_token:"
 msgid "E-mail Token"
-msgstr "_E-Mail..."
+msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
-msgstr "_E-Mail..."
+msgstr ""
 
+#, fuzzy
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Управление на партньор"
 
 #, fuzzy
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr "Password"
+msgstr "Парола"
 
-#, fuzzy
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
-msgstr "Hash della Password"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
-msgstr "Reset Password"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user,reset_password_token_expire:"
 msgid "Reset Password Token Expire"
-msgstr "Reset Password"
+msgstr ""
 
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Управление на партньор"
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Utente"
+msgstr "Потребител"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr "Indirizzo IP"
+msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
-msgstr "Login"
+msgstr "Потребителско име"
 
 #, fuzzy
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr "Chiave"
+msgstr "Ключ"
 
 #, fuzzy
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr "Utente"
+msgstr "Потребител"
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
 msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
@@ -123,30 +119,37 @@
 msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
 msgstr "Web Users"
 
-#, fuzzy
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
-msgstr "Sessione"
+msgstr ""
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
-msgstr "Sessione"
+msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 
 #, fuzzy
@@ -154,19 +157,14 @@
 msgid "Reset Password"
 msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
@@ -180,17 +178,18 @@
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
-msgstr "Verifica"
+msgstr "Проверка"
 
 #, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
 msgstr "Reset Password"
 
 #, fuzzy
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_web_user-7.0.0/locale/lo.po` & `trytond_web_user-7.2.0/locale/lo.po`

 * *Files 4% similar despite different names*

```diff
@@ -130,36 +130,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "ພະຍາຍາມກວດສອບສິດທີ່ຖືກຕ້ອງຂອງຜູ້ໃຊ້ງານເວັບ"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "ເທື່ອເຂົ້າໃຊ້ຂອງຜູ້ໃຊ້ງານເວັບ"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "ປຸ່ມບໍ່ເຮັດວຽກບໍ? ໃຫ້ ວາງ ອັນນີ້ລົງໃສ່ ໂຕທ່ອງເວັບຂອງທ່ານ:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "ຖ້າຫາກທ່ານບໍ່ໄດ້ຮ້ອງຂໍ ອ-ເມວລ໌ ນີ້, ທ່ານບໍ່ຕ້ອງຮັບຮູ້ ອີ-ເມວລ໌ ນີ້."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "ຕັ້ງຄ່າລະຫັດຜ່ານຄືນໃໝ່"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-#, fuzzy
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "ພວກເຮົາໄດ້ຮັບຄຳຮ້ອງຂໍໃຫ້ຕັ້ງຄ່າລະຫັດຜ່ານບັນຊີໃຊ້ງານຂອງທ່ານຄືນໃໝ່,"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "ປຸ່ມບໍ່ເຮັດວຽກບໍ? ໃຫ້ ວາງ ອັນນີ້ລົງໃສ່ ໂຕທ່ອງເວັບຂອງທ່ານ:"
```

### Comparing `trytond_web_user-7.0.0/locale/lt.po` & `trytond_web_user-7.2.0/locale/tr.po`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
 msgstr ""
 
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Kontrahentas"
+msgstr ""
 
 msgctxt "field:web.user,password:"
 msgid "Password"
 msgstr ""
 
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
@@ -34,31 +34,30 @@
 msgid "Reset Password Token Expire"
 msgstr ""
 
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Kontrahentas"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Naudotojas"
+msgstr "Web Users"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr "IP adresas"
+msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
@@ -66,28 +65,28 @@
 
 msgctxt "field:web.user.session,key:"
 msgid "Key"
 msgstr ""
 
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr "Naudotojas"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
 msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
 msgstr "Web Users"
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr "Atstatyti slaptažodį"
+msgstr "Reset Password"
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
 msgstr "Email Validation"
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
@@ -99,15 +98,15 @@
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr "Atstatyti slaptažodį"
+msgstr "Reset Password"
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
 msgstr "Validate E-mail"
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
@@ -127,15 +126,24 @@
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 
 #, fuzzy
@@ -143,19 +151,14 @@
 msgid "Reset Password"
 msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_web_user-7.0.0/locale/nl.po` & `trytond_web_user-7.2.0/locale/nl.po`

 * *Files 3% similar despite different names*

```diff
@@ -122,37 +122,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Inlog poging webgebruikers"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Webgebruikerssessie"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "Knop werkt niet? Plak dit in uw browser:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Indien u dit verzoek niet hebt gedaan, kunt u deze e-mail negeren."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Reset wachtwoord"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "De link vervalt in [1:%(datetime)s]."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-"We hebben het verzoek ontvangen om het wachtwoord voor uw account %(email)s "
-"opnieuw in te stellen"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "Knop werkt niet? Plak dit in uw browser:"
```

### Comparing `trytond_web_user-7.0.0/locale/pl.po` & `trytond_web_user-7.2.0/locale/ru.po`

 * *Files 22% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 msgid "E-mail Token"
 msgstr ""
 
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr ""
+msgstr "Организации"
 
+#, fuzzy
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr ""
+msgstr "Пароль"
 
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
 msgstr ""
 
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
@@ -34,46 +36,50 @@
 msgid "Reset Password Token Expire"
 msgstr ""
 
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr ""
+msgstr "Организации"
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Web Users"
+msgstr "Пользователь"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
-msgstr ""
+msgstr "Логин"
 
+#, fuzzy
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr ""
+msgstr "Ключ"
 
+#, fuzzy
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr ""
+msgstr "Пользователь"
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
 msgstr "Web Users"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
@@ -126,15 +132,24 @@
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr ""
 
 #, fuzzy
@@ -142,19 +157,14 @@
 msgid "Reset Password"
 msgstr "Reset Password"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr ""
@@ -168,17 +178,18 @@
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
-msgstr ""
+msgstr "Утвержденный"
 
 #, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
 msgstr "Reset Password"
 
 #, fuzzy
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_web_user-7.0.0/locale/pt.po` & `trytond_web_user-7.2.0/locale/pt.po`

 * *Files 3% similar despite different names*

```diff
@@ -130,36 +130,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Tentativa de autenticação do usuário Web"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Sessão de Usuário Web"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "O botão não está funcionando? Cole isso em seu navegador:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Se você não fez esta solicitação, você pode ignorar esse email."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Redefinir senha"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-#, fuzzy
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "Nós recebemos uma solicitação para redefinir a senha da sua conta,"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "Botão não está funcionando? Cole isso no seu navegador:"
```

### Comparing `trytond_web_user-7.0.0/locale/ro.po` & `trytond_web_user-7.2.0/locale/id.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:web.user,email:"
 msgid "E-mail"
-msgstr ""
+msgstr "E-mail"
 
 msgctxt "field:web.user,email_token:"
 msgid "E-mail Token"
 msgstr ""
 
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
 msgstr ""
 
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Pihak"
 
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr "Parola"
+msgstr "Kata sandi"
 
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
 msgstr ""
 
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
@@ -37,75 +37,77 @@
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr "Pihak"
 
+#, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr ""
+msgstr "Pengguna"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr ""
+msgstr "Alamat IP"
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
 msgstr ""
 
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr ""
+msgstr "Kunci"
 
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr ""
+msgstr "Pengguna"
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
-msgstr ""
+msgstr "Pengguna Web"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
-msgstr ""
+msgstr "Pengguna Web"
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr "Resetare parola"
+msgstr "Atur Ulang Kata Sandi"
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
-msgstr "Adresa de email \"%(email)s\" pentru \"%(user)s\" nu este valid."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_unique"
 msgid "E-mail of active web user must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr "Resetare Parola"
+msgstr "Atur Ulang Kata Sandi"
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
@@ -123,59 +125,64 @@
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
+msgstr "Tombol tidak berfungsi? Lekatkan ini pada browser Anda:"
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
-msgstr ""
+msgstr "Jika bukan Anda yang membuat permintaan ini, abaikan email ini."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
-msgstr ""
+msgstr "Atur Ulang Kata Sandi"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
-msgstr ""
+msgstr "Tombol tidak berfungsi? Lekatkan ini pada browser Anda:"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Email Validation"
-msgstr ""
+msgstr "Validasi Email"
 
 msgctxt "report:web.user.email_validation:"
 msgid "If you received this email by mistake, just ignore it."
-msgstr ""
+msgstr "Jika Anda menerima email ini karena kesalahan, abaikan saja."
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
-msgstr ""
+msgstr "Tinggal satu langkah lagi..."
 
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
 msgstr ""
 
 msgctxt "view:web.user:"
 msgid "Reset Password"
-msgstr ""
+msgstr "Atur Ulang Kata Sandi"
 
 msgctxt "view:web.user:"
 msgid "Validate E-mail"
 msgstr ""
```

### Comparing `trytond_web_user-7.0.0/locale/ru.po` & `trytond_web_user-7.2.0/locale/et.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:web.user,email:"
 msgid "E-mail"
-msgstr ""
+msgstr "E-kiri"
 
 msgctxt "field:web.user,email_token:"
 msgid "E-mail Token"
 msgstr ""
 
 msgctxt "field:web.user,email_valid:"
 msgid "E-mail Valid"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:web.user,party:"
 msgid "Party"
-msgstr "Организации"
+msgstr "Osapool"
 
-#, fuzzy
 msgctxt "field:web.user,password:"
 msgid "Password"
-msgstr "Пароль"
+msgstr "Salasõna"
 
 msgctxt "field:web.user,password_hash:"
 msgid "Password Hash"
-msgstr ""
+msgstr "Salasõna räsi"
 
 msgctxt "field:web.user,reset_password_token:"
 msgid "Reset Password Token"
 msgstr ""
 
 msgctxt "field:web.user,reset_password_token_expire:"
 msgid "Reset Password Token Expire"
@@ -39,64 +37,61 @@
 msgctxt "field:web.user,secondary_parties:"
 msgid "Secondary Parties"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,party:"
 msgid "Party"
-msgstr "Организации"
+msgstr "Osapool"
 
 #, fuzzy
 msgctxt "field:web.user-party.party.secondary,user:"
 msgid "User"
-msgstr "Пользователь"
+msgstr "Kasutaja"
 
 msgctxt "field:web.user.authenticate.attempt,device_cookie:"
 msgid "Device Cookie"
 msgstr ""
 
 msgctxt "field:web.user.authenticate.attempt,ip_address:"
 msgid "IP Address"
-msgstr ""
+msgstr "IP-aadress"
 
 msgctxt "field:web.user.authenticate.attempt,ip_network:"
 msgid "IP Network"
-msgstr ""
+msgstr "IP-võrk"
 
-#, fuzzy
 msgctxt "field:web.user.authenticate.attempt,login:"
 msgid "Login"
-msgstr "Логин"
+msgstr "Logi sisse"
 
-#, fuzzy
 msgctxt "field:web.user.session,key:"
 msgid "Key"
-msgstr "Ключ"
+msgstr "Võti"
 
-#, fuzzy
 msgctxt "field:web.user.session,user:"
 msgid "User"
-msgstr "Пользователь"
+msgstr "Kasutaja"
 
 msgctxt "model:ir.action,name:act_user_form"
 msgid "Web Users"
-msgstr "Web Users"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_user_form_party"
 msgid "Web Users"
-msgstr "Web Users"
+msgstr "Muutja"
 
 msgctxt "model:ir.action,name:report_email_reset_password"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr "Lähtesta salasõna"
 
 msgctxt "model:ir.action,name:report_email_validation"
 msgid "Email Validation"
-msgstr "Email Validation"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_invalid"
 msgid "The email address \"%(email)s\" for \"%(user)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_user_email_unique"
 msgid "E-mail of active web user must be unique."
@@ -104,91 +99,90 @@
 
 msgctxt "model:ir.message,text:msg_user_session_key_unique"
 msgid "Web user session key must be unique."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:user_reset_password_button"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr "Lähtesta salasõna"
 
 msgctxt "model:ir.model.button,string:user_validate_email_button"
 msgid "Validate E-mail"
-msgstr "Validate E-mail"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_user_form"
 msgid "Web Users"
-msgstr "Web Users"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:web.user,name:"
 msgid "Web User"
-msgstr "Web Users"
+msgstr ""
 
 msgctxt "model:web.user-party.party.secondary,name:"
 msgid "Web User - Secondary Party"
 msgstr ""
 
 msgctxt "model:web.user.authenticate.attempt,name:"
 msgid "Web User Authenticate Attempt"
 msgstr ""
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
+msgstr "Nupp ei tööta? Aseta see link brauseri aadressreale:"
+
+msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
 msgstr ""
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
-msgstr ""
+msgstr "Kui sa ei teinud seda päringut, siis ignoreeri seda e-kirja."
 
-#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr "Lähtesta salasõna"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr ""
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
-msgstr ""
+msgstr "Nupp ei tööta? Aseta see link brauseri aadressreale:"
 
-#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Email Validation"
-msgstr "Email Validation"
+msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "If you received this email by mistake, just ignore it."
 msgstr ""
 
 msgctxt "report:web.user.email_validation:"
 msgid "Just one more step.."
 msgstr ""
 
-#, fuzzy
 msgctxt "report:web.user.email_validation:"
 msgid "Validate"
-msgstr "Утвержденный"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:web.user:"
 msgid "Reset Password"
-msgstr "Reset Password"
+msgstr "Lähtesta salasõna"
 
-#, fuzzy
 msgctxt "view:web.user:"
 msgid "Validate E-mail"
-msgstr "Validate E-mail"
+msgstr ""
```

### Comparing `trytond_web_user-7.0.0/locale/sl.po` & `trytond_web_user-7.2.0/locale/sl.po`

 * *Files 6% similar despite different names*

```diff
@@ -122,35 +122,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Poskus overjanja spletnega uporabnika"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Seja spletnega uporabnika"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "Gumb ne deluje? Prilepite sledeče v vaš brskalnik:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Če niste zahtevali tega sporočila, ga preprosto prezrite."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Ponastavitev gesla"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "Povezava bo potekla čez [1:%(datetime)s]."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "Prejeli smo zahtevek za ponastavitev gesla vašega računa: %(email)s"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "Gumb ne deluje? Prilepite to povezavo v vaš brskalnik:"
```

### Comparing `trytond_web_user-7.0.0/locale/uk.po` & `trytond_web_user-7.2.0/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -122,36 +122,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Спроба автентифікації веб-користувача"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "Сеанс веб-користувача"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "Кнопка не працює? Вставте це у свій браузер:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "Якщо ви не робили цей запит, можете проігнорувати цей ел.лист."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "Скинути пароль"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "Термін посилання завершиться через [1:%(datetime)s]."
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr ""
-"Ми отримали запит на скидання пароля для вашого облікового запису: %(email)s"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "Кнопка не працює? Вставте це у свій браузер:"
```

### Comparing `trytond_web_user-7.0.0/locale/zh_CN.po` & `trytond_web_user-7.2.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -122,35 +122,40 @@
 msgid "Web User Authenticate Attempt"
 msgstr "Web用户验证尝试"
 
 msgctxt "model:web.user.session,name:"
 msgid "Web User Session"
 msgstr "web 用户会话"
 
+#, fuzzy
 msgctxt "report:web.user.email_reset_password:"
-msgid "Button is not working? Paste this into your browser:"
+msgid "Button not working? Paste this into your browser:"
 msgstr "按钮不起作用？ 将此粘贴到浏览器的地址栏中:"
 
 msgctxt "report:web.user.email_reset_password:"
+msgid ""
+"Hello, we received a request to reset the password for the account associated with [1:%(email)s]. No changes have been made to your account yet.[2:]\n"
+"                You can reset your password by clicking the link below:[3:]\n"
+"                [4:\n"
+"                    Reset Password\n"
+"                ]"
+msgstr ""
+
+msgctxt "report:web.user.email_reset_password:"
 msgid "If you didn't make this request, you can ignore this email."
 msgstr "如果你没有发出过此请求，就忽略此电子邮件."
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "Reset Password"
 msgstr "重置密码"
 
 msgctxt "report:web.user.email_reset_password:"
 msgid "The link will expire in [1:%(datetime)s]."
 msgstr "链接过期时间： [1:%(datetime)s]。"
 
-msgctxt "report:web.user.email_reset_password:"
-msgid ""
-"We received a request to reset the password for your account: %(email)s"
-msgstr "我们收到了重置你的帐户 %(email)s 的密码的请求"
-
 msgctxt "report:web.user.email_validation:"
 msgid "%(email)s"
 msgstr "%(email)s"
 
 msgctxt "report:web.user.email_validation:"
 msgid "Button is not working? Paste this into your browser:"
 msgstr "按钮不起作用？ 将此粘贴到浏览器的地址栏中:"
```

### Comparing `trytond_web_user-7.0.0/message.xml` & `trytond_web_user-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/party.py` & `trytond_web_user-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/setup.py` & `trytond_web_user-7.2.0/setup.py`

 * *Files 6% similar despite different names*

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
@@ -55,15 +58,17 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": (
+            'https://docs.tryton.org/'
+            'modules-web-user'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='web user',
     package_dir={'trytond.modules.web_user': '.'},
     packages=(
         ['trytond.modules.web_user']
```

### Comparing `trytond_web_user-7.0.0/tests/test_module.py` & `trytond_web_user-7.2.0/tests/test_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-from unittest.mock import ANY, patch
+from unittest.mock import patch
 
 from trytond.config import config
 from trytond.modules.party.tests import PartyCheckEraseMixin
 from trytond.modules.web_user import user as user_module
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 
@@ -97,17 +97,18 @@
         User = pool.get('web.user')
 
         user = User(email='user@example.com')
         user.save()
         self.assertFalse(user.email_valid)
         self.assertFalse(user.email_token)
 
-        with patch.object(user_module, 'sendmail_transactional') as sendmail:
+        with patch.object(
+                user_module, 'send_message_transactional') as send_message:
             User.validate_email([user])
-            sendmail.assert_called_once_with(FROM, ['user@example.com'], ANY)
+            send_message.assert_called_once()
 
         token = user.email_token
         self.assertTrue(token)
 
         self.assertEqual(
             user.get_email_validation_url(),
             '%s?token=%s' % (VALIDATION_URL, token))
@@ -129,17 +130,18 @@
         pool = Pool()
         User = pool.get('web.user')
 
         user = User(email='user@example.com', email_valid=True)
         user.save()
         self.assertFalse(user.password_hash)
 
-        with patch.object(user_module, 'sendmail_transactional') as sendmail:
+        with patch.object(
+                user_module, 'send_message_transactional') as send_message:
             User.reset_password([user])
-            sendmail.assert_called_once_with(FROM, ['user@example.com'], ANY)
+            send_message.assert_called_once()
 
         token = user.reset_password_token
         self.assertTrue(token)
         self.assertTrue(user.reset_password_token_expire)
 
         self.assertEqual(
             user.get_email_reset_password_url(),
```

### Comparing `trytond_web_user-7.0.0/tox.ini` & `trytond_web_user-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/trytond_web_user.egg-info/SOURCES.txt` & `trytond_web_user-7.2.0/trytond_web_user.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 email_reset_password.html
@@ -51,15 +50,18 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/user_form.xml
 ./view/user_list.xml
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
```

### Comparing `trytond_web_user-7.0.0/user.py` & `trytond_web_user-7.2.0/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import hashlib
 import logging
 import random
 import string
 import time
 import urllib.parse
 import warnings
-from email.header import Header
 from secrets import token_hex
 
 try:
     import bcrypt
 except ImportError:
     bcrypt = None
 try:
@@ -30,32 +29,32 @@
 from trytond.model import (
     DeactivableMixin, Exclude, Index, ModelSQL, ModelView, Unique,
     avatar_mixin, fields)
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.report import Report, get_email
 from trytond.res.user import CRYPT_CONTEXT, LoginAttempt
-from trytond.sendmail import sendmail_transactional
+from trytond.sendmail import send_message_transactional
 from trytond.tools.email_ import (
     EmailNotValidError, normalize_email, set_from_header, validate_email)
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 from .exceptions import UserValidationError
 
 logger = logging.getLogger(__name__)
 
 
 def _send_email(from_, users, email_func):
     from_cfg = config.get('email', 'from')
     for user in users:
         msg, title = email_func(user)
         set_from_header(msg, from_cfg, from_ or from_cfg)
         msg['To'] = user.email
-        msg['Subject'] = Header(title, 'utf-8')
-        sendmail_transactional(from_cfg, [user.email], msg)
+        msg['Subject'] = title
+        send_message_transactional(msg)
 
 
 def _add_params(url, **params):
     parts = urllib.parse.urlsplit(url)
     query = urllib.parse.parse_qsl(parts.query)
     for key, value in sorted(params.items()):
         query.append((key, value))
@@ -213,16 +212,16 @@
         users = cls.search([('email', '=', email)])
         if users:
             user, = users
             valid, new_hash = cls.check_password(password, user.password_hash)
             if valid:
                 if new_hash:
                     logger.info("Update password hash for %s", user.id)
-                    with Transaction().new_transaction() as transaction:
-                        with transaction.set_user(0):
+                    with Transaction().new_transaction():
+                        with without_check_access():
                             cls.write([cls(user.id)], {
                                     'password_hash': new_hash,
                                     })
                 Attempt.remove(email)
                 return user
         Attempt.add(email)
```

### Comparing `trytond_web_user-7.0.0/user.xml` & `trytond_web_user-7.2.0/user.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_web_user-7.0.0/user.xml` & `trytond_web_user-7.2.0/user.xml`

```diff
@@ -45,37 +45,37 @@
     </record>
     <record model="ir.action.keyword" id="act_user_form_party_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">party.party,-1</field>
       <field name="action" ref="act_user_form_party"/>
     </record>
     <record model="ir.model.access" id="access_user">
-      <field name="model" search="[('model', '=', 'web.user')]"/>
+      <field name="model">web.user</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_user_admin">
-      <field name="model" search="[('model', '=', 'web.user')]"/>
+      <field name="model">web.user</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="user_validate_email_button">
+      <field name="model">web.user</field>
       <field name="name">validate_email</field>
       <field name="string">Validate E-mail</field>
-      <field name="model" search="[('model', '=', 'web.user')]"/>
     </record>
     <record model="ir.model.button" id="user_reset_password_button">
+      <field name="model">web.user</field>
       <field name="name">reset_password</field>
       <field name="string">Reset Password</field>
-      <field name="model" search="[('model', '=', 'web.user')]"/>
     </record>
     <record model="ir.action.report" id="report_email_validation">
       <field name="name">Email Validation</field>
       <field name="model">web.user</field>
       <field name="report_name">web.user.email_validation</field>
       <field name="report">web_user/email_validation.html</field>
       <field name="template_extension">html</field>
```

### Comparing `trytond_web_user-7.0.0/view/user_form.xml` & `trytond_web_user-7.2.0/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-7.0.0/view/user_list.xml` & `trytond_web_user-7.2.0/view/user_list.xml`

 * *Files identical despite different names*

