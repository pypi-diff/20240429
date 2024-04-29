# Comparing `tmp/trytond_party-7.0.2.tar.gz` & `tmp/trytond_party-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party-7.0.2.tar", last modified: Sun Mar  3 12:22:47 2024, max compression
+gzip compressed data, was "trytond_party-7.2.0.tar", last modified: Mon Apr 29 15:41:54 2024, max compression
```

## Comparing `trytond_party-7.0.2.tar` & `trytond_party-7.2.0.tar`

### file list

```diff
@@ -1,105 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.618681 trytond_party-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:38.000000 trytond_party-7.0.2/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     7073 2024-03-03 12:22:44.000000 trytond_party-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-03-03 12:22:44.000000 trytond_party-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_party-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_party-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-03-03 12:22:47.618681 trytond_party-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-30 17:06:38.000000 trytond_party-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1062 2023-10-30 17:06:38.000000 trytond_party-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16172 2023-10-30 17:06:38.000000 trytond_party-7.0.2/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25257 2024-02-05 16:24:27.000000 trytond_party-7.0.2/address.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1173 2023-10-30 17:06:38.000000 trytond_party-7.0.2/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3658 2023-10-30 17:06:38.000000 trytond_party-7.0.2/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4042 2023-10-30 17:06:38.000000 trytond_party-7.0.2/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2251 2023-10-30 17:06:38.000000 trytond_party-7.0.2/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13151 2023-10-30 17:06:38.000000 trytond_party-7.0.2/contact_mechanism.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-10-30 17:06:38.000000 trytond_party-7.0.2/contact_mechanism.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-30 17:06:38.000000 trytond_party-7.0.2/country.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.612014 trytond_party-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2806 2024-02-05 16:24:27.000000 trytond_party-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-10-30 17:06:38.000000 trytond_party-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-30 17:06:38.000000 trytond_party-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_party-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_party-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-10-30 17:06:38.000000 trytond_party-7.0.2/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-10-30 17:06:38.000000 trytond_party-7.0.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.612014 trytond_party-7.0.2/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_party-7.0.2/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:38.000000 trytond_party-7.0.2/icons/tryton-party.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-10-30 17:06:38.000000 trytond_party-7.0.2/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-10-30 17:06:38.000000 trytond_party-7.0.2/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    31778 2023-10-30 17:06:38.000000 trytond_party-7.0.2/label.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.612014 trytond_party-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    34600 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41677 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33245 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43389 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42097 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33184 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38928 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38349 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33030 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41643 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35922 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33899 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36283 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37727 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39999 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41340 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40052 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36259 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40685 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35113 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41421 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33030 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    49356 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35733 2023-10-30 17:06:38.000000 trytond_party-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3240 2023-10-30 17:06:38.000000 trytond_party-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    41441 2024-02-29 11:47:59.000000 trytond_party-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8099 2023-10-30 17:06:38.000000 trytond_party-7.0.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:22:47.618681 trytond_party-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4647 2023-10-30 17:06:38.000000 trytond_party-7.0.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.615347 trytond_party-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-30 17:06:38.000000 trytond_party-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1638 2024-02-05 16:24:27.000000 trytond_party-7.0.2/tests/scenario_party_erase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-10-30 17:06:38.000000 trytond_party-7.0.2/tests/scenario_party_identifier_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2024-02-05 16:24:27.000000 trytond_party-7.0.2/tests/scenario_party_phone_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2024-02-05 16:24:27.000000 trytond_party-7.0.2/tests/scenario_party_replace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    19513 2023-10-30 17:06:38.000000 trytond_party-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_party-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_party-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-02-15 18:34:57.000000 trytond_party-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.615347 trytond_party-7.0.2/trytond_party.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3012 2024-03-03 12:22:47.000000 trytond_party-7.0.2/trytond_party.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3518 2024-03-03 12:22:47.000000 trytond_party-7.0.2/trytond_party.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:22:47.000000 trytond_party-7.0.2/trytond_party.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2024-03-03 12:22:47.000000 trytond_party-7.0.2/trytond_party.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:52.000000 trytond_party-7.0.2/trytond_party.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-03-03 12:22:47.000000 trytond_party-7.0.2/trytond_party.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:22:47.000000 trytond_party-7.0.2/trytond_party.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:22:47.615347 trytond_party-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1556 2024-02-05 16:24:27.000000 trytond_party-7.0.2/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      999 2024-02-05 16:24:27.000000 trytond_party-7.0.2/view/address_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/address_format_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/address_format_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/address_subdivision_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/address_subdivision_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/check_vies_result.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2024-02-05 16:24:27.000000 trytond_party-7.0.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-02-10 10:25:55.000000 trytond_party-7.0.2/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/erase_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-02-05 16:24:27.000000 trytond_party-7.0.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-10-30 17:06:38.000000 trytond_party-7.0.2/view/replace_ask_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.547119 trytond_party-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7035 2024-04-29 15:20:52.000000 trytond_party-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-04-29 15:20:52.000000 trytond_party-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-29 15:41:54.547119 trytond_party-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1062 2023-04-15 07:12:15.000000 trytond_party-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16172 2024-02-04 18:51:26.000000 trytond_party-7.2.0/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25150 2024-04-27 16:30:39.000000 trytond_party-7.2.0/address.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1173 2024-01-27 09:58:52.000000 trytond_party-7.2.0/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2024-04-27 16:30:39.000000 trytond_party-7.2.0/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4042 2024-02-04 18:51:26.000000 trytond_party-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2205 2024-04-27 16:30:39.000000 trytond_party-7.2.0/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-02-04 18:51:26.000000 trytond_party-7.2.0/contact_mechanism.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-04-15 07:12:15.000000 trytond_party-7.2.0/contact_mechanism.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_party-7.2.0/country.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.540452 trytond_party-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2024-04-27 16:30:39.000000 trytond_party-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:13.000000 trytond_party-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-04-15 07:12:15.000000 trytond_party-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-02-04 18:51:26.000000 trytond_party-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.540452 trytond_party-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_party-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:20.000000 trytond_party-7.2.0/icons/tryton-party.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-04-15 07:12:15.000000 trytond_party-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-15 07:12:15.000000 trytond_party-7.2.0/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    31778 2023-01-16 14:00:20.000000 trytond_party-7.2.0/label.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.543785 trytond_party-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    34600 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41677 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33245 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43389 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42097 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33184 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38928 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38349 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33030 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41643 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35922 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33899 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36283 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37727 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39999 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41340 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40052 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36259 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40658 2024-04-29 13:17:17.000000 trytond_party-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35113 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41421 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33030 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    49356 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35733 2024-04-27 16:43:24.000000 trytond_party-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-02-04 18:51:26.000000 trytond_party-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    42600 2024-04-27 16:30:39.000000 trytond_party-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8099 2023-04-15 07:12:15.000000 trytond_party-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:54.547119 trytond_party-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4638 2024-04-27 16:30:39.000000 trytond_party-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.543785 trytond_party-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_party-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-22 12:14:36.000000 trytond_party-7.2.0/tests/scenario_party_erase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-01-27 09:58:52.000000 trytond_party-7.2.0/tests/scenario_party_identifier_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2024-04-22 12:14:36.000000 trytond_party-7.2.0/tests/scenario_party_phone_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1407 2024-04-22 12:14:36.000000 trytond_party-7.2.0/tests/scenario_party_replace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    19513 2024-04-01 21:57:37.000000 trytond_party-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_party-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:13.000000 trytond_party-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-29 15:20:48.000000 trytond_party-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.547119 trytond_party-7.2.0/trytond_party.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3500 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-14 15:56:20.000000 trytond_party-7.2.0/trytond_party.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:54.000000 trytond_party-7.2.0/trytond_party.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:54.547119 trytond_party-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1579 2024-03-17 11:01:36.000000 trytond_party-7.2.0/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-03-17 11:01:36.000000 trytond_party-7.2.0/view/address_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_format_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_format_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_subdivision_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_subdivision_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/check_vies_result.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-22 12:14:36.000000 trytond_party-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-27 16:30:39.000000 trytond_party-7.2.0/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/erase_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-01-27 09:58:52.000000 trytond_party-7.2.0/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1593 2024-03-17 11:01:36.000000 trytond_party-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_party-7.2.0/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-01-16 14:00:20.000000 trytond_party-7.2.0/view/replace_ask_form.xml
```

### Comparing `trytond_party-7.0.2/CHANGELOG` & `trytond_party-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 
-Version 7.0.2 - 2024-03-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-02-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Use usage from context for default contact mechanism on party
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Autocomplete party from European VAT number
 * Use vat alias for party identifier
```

### Comparing `trytond_party-7.0.2/COPYRIGHT` & `trytond_party-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/LICENSE` & `trytond_party-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/PKG-INFO` & `trytond_party-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_party
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-party/
+Project-URL: Documentation, https://docs.tryton.org/modules-party/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -50,18 +50,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
 Requires-Dist: python-stdnum>=1.19
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 Requires-Dist: phonenumbers; extra == "test"
 Provides-Extra: vies
 Requires-Dist: python-stdnum[SOAP]; extra == "vies"
 Provides-Extra: phonenumbers
 Requires-Dist: phonenumbers; extra == "phonenumbers"
 
 ############
```

### Comparing `trytond_party-7.0.2/__init__.py` & `trytond_party-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/address.py` & `trytond_party-7.2.0/address.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/address.xml` & `trytond_party-7.2.0/address.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_party-7.0.2/address.xml` & `trytond_party-7.2.0/address.xml`

```diff
@@ -62,22 +62,22 @@
     <record model="ir.action.act_window.view" id="act_address_format_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="address_format_view_form"/>
       <field name="act_window" ref="act_address_format_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_address_format_form" sequence="50" id="menu_address_format_form"/>
     <record model="ir.model.access" id="access_address_format">
-      <field name="model" search="[('model', '=', 'party.address.format')]"/>
+      <field name="model">party.address.format</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_address_format_admin">
-      <field name="model" search="[('model', '=', 'party.address.format')]"/>
+      <field name="model">party.address.format</field>
       <field name="group" ref="group_party_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="address_subdivision_type_view_list">
@@ -102,22 +102,22 @@
     <record model="ir.action.act_window.view" id="act_address_subdivision_type_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="address_subdivision_type_view_form"/>
       <field name="act_window" ref="act_address_subdivision_type_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_address_subdivision_type_form" sequence="50" id="menu_address_subdivision_type_form"/>
     <record model="ir.model.access" id="access_address_subdivision_type">
-      <field name="model" search="[('model', '=', 'party.address.subdivision_type')]"/>
+      <field name="model">party.address.subdivision_type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_address_subdivision_type_admin">
-      <field name="model" search="[('model', '=', 'party.address.subdivision_type')]"/>
+      <field name="model">party.address.subdivision_type</field>
       <field name="group" ref="group_party_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
@@ -134,15 +134,14 @@
     </record>
     <record model="party.address.format" id="address_format_au">
       <field name="country_code">AU</field>
       <field name="format_">${party_name}
 ${attn}
 ${name}
 ${street}
-${subdivision}
 ${CITY} ${SUBDIVISION} ${POSTAL_CODE}
 ${COUNTRY}</field>
     </record>
     <record model="party.address.format" id="address_format_at">
       <field name="country_code">AT</field>
       <field name="format_">${party_name}
 ${attn}
```

### Comparing `trytond_party-7.0.2/category.py` & `trytond_party-7.2.0/category.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/category.xml` & `trytond_party-7.2.0/category.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_party-7.0.2/category.xml` & `trytond_party-7.2.0/category.xml`

```diff
@@ -48,22 +48,22 @@
     <record model="ir.action.act_window.view" id="act_category_list_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="category_view_form"/>
       <field name="act_window" ref="act_category_list"/>
     </record>
     <menuitem parent="menu_category_tree" sequence="10" action="act_category_list" id="menu_category_list"/>
     <record model="ir.model.access" id="access_party_category">
-      <field name="model" search="[('model', '=', 'party.category')]"/>
+      <field name="model">party.category</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_party_category_admin">
-      <field name="model" search="[('model', '=', 'party.category')]"/>
+      <field name="model">party.category</field>
       <field name="group" ref="group_party_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_party-7.0.2/configuration.py` & `trytond_party-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/configuration.xml` & `trytond_party-7.2.0/configuration.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_party-7.0.2/configuration.xml` & `trytond_party-7.2.0/configuration.xml`

```diff
@@ -15,22 +15,22 @@
     <record model="ir.action.act_window.view" id="act_party_configuration_view1">
       <field name="sequence" eval="1"/>
       <field name="view" ref="party_configuration_view_form"/>
       <field name="act_window" ref="act_party_configuration_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_party_configuration_form" sequence="10" id="menu_party_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_party_configuration">
-      <field name="model" search="[('model', '=', 'party.configuration')]"/>
+      <field name="model">party.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_party_configuration_party_admin">
-      <field name="model" search="[('model', '=', 'party.configuration')]"/>
+      <field name="model">party.configuration</field>
       <field name="group" ref="group_party_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_party-7.0.2/contact_mechanism.py` & `trytond_party-7.2.0/contact_mechanism.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/contact_mechanism.xml` & `trytond_party-7.2.0/contact_mechanism.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/country.py` & `trytond_party-7.2.0/country.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/doc/conf.py` & `trytond_party-7.2.0/doc/conf.py`

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

### Comparing `trytond_party-7.0.2/doc/design.rst` & `trytond_party-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/doc/usage.rst` & `trytond_party-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/exceptions.py` & `trytond_party-7.2.0/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/icons/LICENSE` & `trytond_party-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/ir.py` & `trytond_party-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/label.fodt` & `trytond_party-7.2.0/label.fodt`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/bg.po` & `trytond_party-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/ca.po` & `trytond_party-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/cs.po` & `trytond_party-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/de.po` & `trytond_party-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/es.po` & `trytond_party-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/es_419.po` & `trytond_party-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/et.po` & `trytond_party-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/fa.po` & `trytond_party-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/fi.po` & `trytond_party-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/fr.po` & `trytond_party-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/hu.po` & `trytond_party-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/id.po` & `trytond_party-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/it.po` & `trytond_party-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/lo.po` & `trytond_party-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/lt.po` & `trytond_party-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/nl.po` & `trytond_party-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/pl.po` & `trytond_party-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/pt.po` & `trytond_party-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/ro.po` & `trytond_party-7.2.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -679,18 +679,17 @@
 msgid "Party Administration"
 msgstr "Administrare Parte"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Albanian VAT Number"
 msgstr "Albania, Cod TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Algerian Tax Number"
-msgstr "Germania, Cod Fiscal"
+msgstr "Cod Fiscal Algerian"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Andorra Tax Number"
 msgstr "Andorra, Cod Fiscal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Argentinian National Identity Number"
@@ -728,27 +727,25 @@
 msgid "Austrian Umsatzsteuer-Identifikationsnummer"
 msgstr "Austria, Nr Umsatzsteuer de identificare"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belarus VAT Number"
 msgstr "Belarus, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belgian BIS Number"
-msgstr "Bulgaria, Număr TVA"
+msgstr "Numar TVA Belgian (BIS)"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belgian Enterprise Number"
 msgstr "Belgia, Număr de Companie"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Belgian National Number"
-msgstr "Chile, Cod Fiscal"
+msgstr "Numar National Belgian"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Brazillian Company Identifier"
 msgstr "Brazilia, Identificator Companie"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Brazillian National Identifier"
@@ -862,18 +859,17 @@
 msgid "Ecuadorian Personal Identity Code"
 msgstr "Ecuador, Cod Numeric Personal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Ecuadorian Tax Identification"
 msgstr "Ecuador, Cod Fiscal"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Egyptian Tax Registration Number"
-msgstr "Ucraina, Cod Contribuabil Individual"
+msgstr "Număr de înregistrare fiscală egipteană"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "English Unique Pupil Number"
 msgstr "Anglia, Număr Unic de Elev"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Estonian Organisation Registration Code"
@@ -889,20 +885,19 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "European VAT Number"
 msgstr "Europa, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "European VAT on e-Commerce - One Stop Shop"
-msgstr ""
+msgstr "TVA european pentru Comerț electronic - Ghișeu unic"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Faroese Tax Number"
-msgstr "Malta, Număr TVA"
+msgstr "Cod Fiscal Feroez"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish Association Identifier"
 msgstr "Finlanda, Identificator de Asociaţie"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish Business Identifier"
@@ -952,35 +947,33 @@
 msgid "German Tax Number"
 msgstr "Germania, Cod Fiscal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "German VAT Number"
 msgstr "Germania, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Ghanaian Taxpayer Identification Number"
-msgstr "SUA, Număr de Identificare al Contribuabilului"
+msgstr "Număr de Identificare al Contribuabilului Ghanez"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Greek Social Security Number"
 msgstr "Grecia, Cod Numeric Personal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Greek VAT Number"
 msgstr "Grecia, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Guatemala Tax Number"
 msgstr "Guatemala, Cod Fiscal"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Guinean Tax Number"
-msgstr "Germania, Cod Fiscal"
+msgstr "Cod Fiscal Guineea"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Hungarian VAT Number"
 msgstr "Ungaria, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Icelandic Personal and Organisation Identity Code"
@@ -994,22 +987,21 @@
 msgid "Indian Digital Resident Personal Identity Number"
 msgstr "India, Cod Numeric Personal Digital"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Income Tax Identifier"
 msgstr "India, Cod Împozitare Venit"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian VAT number"
-msgstr "Indonezia, Număr TVA"
+msgstr "Număr TVA Indian"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Voter ID"
-msgstr ""
+msgstr "Indian, Carte de Alegator"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indonesian VAT Number"
 msgstr "Indonezia, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish Personal Number"
@@ -1051,18 +1043,17 @@
 msgid "Lithuanian VAT Number"
 msgstr "Lituania, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Luxembourgian VAT Number"
 msgstr "Luxemburg, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Macedonian Tax Number"
-msgstr "Mexico, Cod Fiscal"
+msgstr "Cod Fiscal Macedonean"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Malaysian National Registration Identity Card Number"
 msgstr "Malaysia, Număr Naţional de card de Înregistrare"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Maltese VAT Number"
@@ -1080,18 +1071,17 @@
 msgid "Moldavian Company Identification Number"
 msgstr "Moldova, Numpr de Identificare Companie"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Monacan VAT Number"
 msgstr "Monaco, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Moroccan Tax Number"
-msgstr "Mexico, Cod Fiscal"
+msgstr "Cod Fiscal Marocan"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "New Zealand Inland Revenue Department Number"
 msgstr "Noua Zeelandă, Cod Fiscal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Norwegian Birth Number, the National Identity Number"
@@ -1101,18 +1091,17 @@
 msgid "Norwegian Organisation Number"
 msgstr "Norvegia, Număt de Organizaţie"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Norwegian VAT Number"
 msgstr "Norvegia, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Pakistani Computerised National Identity Card Number"
-msgstr "Malaysia, Număr Naţional de card de Înregistrare"
+msgstr "Numărul cărții naționale de identitate computerizate pakistanez"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Paraguay Tax Number"
 msgstr "Paraguai, Cod Fiscal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Peruvian Company Tax Number"
@@ -1130,18 +1119,17 @@
 msgid "Polish Register of Economic Units"
 msgstr "Polonia, Registru de Unitaţi Economice"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Polish VAT Number"
 msgstr "Polonia, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Portuguese Identity Number"
-msgstr "Portugalia, Număr TVA"
+msgstr "Numar de Identitate Portughez"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Portuguese VAT Number"
 msgstr "Portugalia, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Romanian Numerical Personal Code"
@@ -1175,23 +1163,21 @@
 msgid "Slovak Birth Number"
 msgstr "Slovacia, Număr de Naştere"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Slovak VAT Number"
 msgstr "Slovacia, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Slovenian Corporate Registration Number"
-msgstr "Korea de Sud, Număr de Inregistrare Companie"
+msgstr "Număr de înregistrare corporativă slovenă"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Slovenian Unique Master Citizen Number"
-msgstr "Danemarcă, Număr Cetaţean"
+msgstr "CNP Sloven"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Slovenian VAT Number"
 msgstr "Slovenia, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "South African Identity Document Number"
@@ -1247,30 +1233,27 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Swiss VAT Number"
 msgstr "Elveţia, Număr TVA"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Thai Memorandum of Association Number"
-msgstr ""
+msgstr "Tailandez, Număr Memorandum de Asociere"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Thai Personal Identification Number"
-msgstr "Turcia, Cod Numeric Personal"
+msgstr "CNP Thailandez"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Thai Taxpayer Identification Number"
-msgstr "SUA, Număr de Identificare al Contribuabilului"
+msgstr "Număr de Identificare al Contribuabilului Thailandez"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Tunisian Tax Number"
-msgstr "Argentina, Cod Fiscal"
+msgstr "Cod Fiscal Tunisian"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Turkish Personal Identification Number"
 msgstr "Turcia, Cod Numeric Personal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "U.S. Adoption Taxpayer Identification Number"
```

### Comparing `trytond_party-7.0.2/locale/ru.po` & `trytond_party-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/sl.po` & `trytond_party-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/tr.po` & `trytond_party-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/uk.po` & `trytond_party-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/locale/zh_CN.po` & `trytond_party-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/message.xml` & `trytond_party-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/party.py` & `trytond_party-7.2.0/party.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import stdnum.exceptions
 from sql import Column, Literal
 from sql.aggregate import Min
 from sql.functions import CharLength
 from stdnum import get_cc_module
 from stdnum.eu.vat import MEMBER_STATES as EU_MEMBER_STATES
 
+from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, MultiValueMixin, Unique,
     ValueMixin, convert_from, fields, sequence_ordered)
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval
@@ -137,73 +138,92 @@
         Configuration = Pool().get('party.configuration')
         config = Configuration(1)
         return bool(config.get_multivalue('party_sequence', **pattern))
 
     def get_code_readonly(self, name):
         return True
 
-    @classmethod
-    def tax_identifier_types(cls):
-        return TAX_IDENTIFIER_TYPES
-
-    def get_tax_identifier(self, name):
-        types = self.tax_identifier_types()
+    def _get_identifier(self, name, types):
         for identifier in self.identifiers:
             if identifier.type in types:
                 return identifier.id
 
     @classmethod
-    def search_tax_identifier(cls, name, clause):
+    def _search_identifier(cls, name, clause, types):
         _, operator, value = clause
         nested = clause[0][len(name) + 1:]
-        types = cls.tax_identifier_types()
         domain = [
             ('identifiers', 'where', [
                     (nested or 'rec_name', operator, value),
                     ('type', 'in', types),
                     ]),
             ]
-        # Add party without tax identifier
+        # Add party without identifier
         if ((operator == '=' and value is None)
                 or (operator == 'in' and None in value)):
             domain = ['OR',
                 domain, [
                     ('identifiers', 'not where', [
                             ('type', 'in', types),
                             ]),
                     ],
                 ]
         return domain
 
+    @classmethod
+    def tax_identifier_types(cls):
+        return TAX_IDENTIFIER_TYPES
+
+    def get_tax_identifier(self, name):
+        types = self.tax_identifier_types()
+        return self._get_identifier(name, types)
+
+    @classmethod
+    def search_tax_identifier(cls, name, clause):
+        types = cls.tax_identifier_types()
+        return cls._search_identifier(name, clause, types)
+
     def get_full_name(self, name):
         return self.name
 
     def get_contact_mechanism(self, name):
-        for mechanism in self.contact_mechanisms:
-            if mechanism.type == name:
-                return mechanism.value
-        return ''
+        usage = Transaction().context.get('party_contact_mechanism_usage')
+        mechanism = self.contact_mechanism_get(name, usage)
+        return mechanism.value if mechanism else ''
 
     @classmethod
     def set_contact_mechanism(cls, parties, name, value):
         pool = Pool()
         ContactMechanism = pool.get('party.contact_mechanism')
+        usage = Transaction().context.get('party_contact_mechanism_usage')
         contact_mechanisms = []
         for party in parties:
             if getattr(party, name):
                 type_string = cls.fields_get([name])[name]['string']
                 raise AccessError(gettext(
                         'party.msg_party_set_contact_mechanism',
                         party=party.rec_name,
                         field=type_string))
             if value:
-                contact_mechanisms.append(ContactMechanism(
+                contact_mechanism = None
+                if usage:
+                    for contact_mechanism in party.contact_mechanisms:
+                        if (contact_mechanism.type == name
+                                and contact_mechanism.value == value):
+                            break
+                    else:
+                        contact_mechanism = None
+                if not contact_mechanism:
+                    contact_mechanism = ContactMechanism(
                         party=party,
                         type=name,
-                        value=value))
+                        value=value)
+                if usage:
+                    setattr(contact_mechanism, usage, True)
+                contact_mechanisms.append(contact_mechanism)
         ContactMechanism.save(contact_mechanisms)
 
     @classmethod
     def _distance_query(cls, usages=None, party=None, depth=None):
         context = Transaction().context
         if party is None:
             party = context.get('related_party')
@@ -416,20 +436,25 @@
         'party.party', "Party", ondelete='CASCADE')
     lang = fields.Many2One('ir.lang', "Language")
 
 
 class PartyCategory(ModelSQL):
     'Party - Category'
     __name__ = 'party.party-party.category'
-    _table = 'party_category_rel'
     party = fields.Many2One(
         'party.party', "Party", ondelete='CASCADE', required=True)
     category = fields.Many2One(
         'party.category', "Category", ondelete='CASCADE', required=True)
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename('party_category_rel', cls._table)
+        super().__register__(module)
+
 
 IDENTIFIER_VAT = [
     'ad_nrt',
     'al_nipt',
     'ar_cuit',
     'at_uid',
     'au_abn',
@@ -905,26 +930,30 @@
                 eu_vat = get_cc_module('eu', 'vat')
                 try:
                     if not eu_vat.check_vies(identifier.code)['valid']:
                         parties_failed.append(party.id)
                     else:
                         parties_succeed.append(party.id)
                 except Exception as e:
-                    if hasattr(e, 'faultstring') \
-                            and hasattr(e.faultstring, 'find'):
-                        if e.faultstring.find('INVALID_INPUT'):
+                    for msg in e.args:
+                        if msg == 'INVALID_INPUT':
                             parties_failed.append(party.id)
-                            continue
-                        if e.faultstring.find('SERVICE_UNAVAILABLE') \
-                                or e.faultstring.find('MS_UNAVAILABLE') \
-                                or e.faultstring.find('TIMEOUT') \
-                                or e.faultstring.find('SERVER_BUSY'):
+                            break
+                        elif msg in {
+                                'SERVICE_UNAVAILABLE',
+                                'MS_UNAVAILABLE',
+                                'MS_MAX_CONCURRENT_REQ',
+                                'GLOBAL_MS_MAX_CONCURRENT_REQ',
+                                'TIMEOUT',
+                                'SERVER_BUSY',
+                                }:
                             raise VIESUnavailable(
                                 gettext('party.msg_vies_unavailable')) from e
-                    raise
+                    else:
+                        raise
         self.result.parties_succeed = parties_succeed
         self.result.parties_failed = parties_failed
         return 'result'
 
     def default_result(self, fields):
         return {
             'parties_succeed': [p.id for p in self.result.parties_succeed],
```

### Comparing `trytond_party-7.0.2/party.xml` & `trytond_party-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/setup.py` & `trytond_party-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-party/',
+        "Documentation": 'https://docs.tryton.org/modules-party/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton party',
     package_dir={'trytond.modules.party': '.'},
     packages=(
         ['trytond.modules.party']
```

### Comparing `trytond_party-7.0.2/tests/scenario_party_erase.rst` & `trytond_party-7.2.0/tests/scenario_party_erase.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ====================
 Party Erase Scenario
 ====================
 
 Imports::
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('party')
 
 Create a party::
 
@@ -29,29 +29,27 @@
     >>> attachment.resource = party
     >>> attachment.name = "Attachment"
     >>> attachment.save()
 
 Try erase active party::
 
     >>> erase = Wizard('party.erase', models=[party])
-    >>> erase.form.party == party
-    True
-    >>> erase.execute('erase')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> assertEqual(erase.form.party, party)
+    >>> erase.execute('erase')
     Traceback (most recent call last):
         ...
     EraseError: ...
 
 Erase inactive party::
 
     >>> party.active = False
     >>> party.save()
 
     >>> erase = Wizard('party.erase', models=[party])
-    >>> erase.form.party == party
-    True
+    >>> assertEqual(erase.form.party, party)
     >>> erase.execute('erase')
 
 Check fields have been erased::
 
     >>> party.name
     >>> identifier.reload()
     >>> identifier.code
```

### Comparing `trytond_party-7.0.2/tests/scenario_party_identifier_notifications.rst` & `trytond_party-7.2.0/tests/scenario_party_identifier_notifications.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/tests/scenario_party_phone_number.rst` & `trytond_party-7.2.0/tests/scenario_party_phone_number.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ===========================
 Party Phone Number Scenario
 ===========================
 
 Imports::
 
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('party')
 
 Create a country::
```

### Comparing `trytond_party-7.0.2/tests/scenario_party_replace.rst` & `trytond_party-7.2.0/tests/scenario_party_replace.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ======================
 Party Replace Scenario
 ======================
 
 Imports::
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertFalse
 
 Activate modules::
 
     >>> config = activate_modules('party')
 
 Create a party::
 
@@ -31,27 +31,22 @@
     >>> party2.save()
     >>> address2, = party2.addresses
     >>> identifier2, = party2.identifiers
 
 Replace the second by the first party::
 
     >>> replace = Wizard('party.replace', models=[party2])
-    >>> replace.form.source == party2
-    True
+    >>> assertEqual(replace.form.source, party2)
     >>> replace.form.destination = party1
     >>> replace.execute('replace')
 
     >>> party2.reload()
     >>> bool(party2.active)
     False
 
     >>> identifier2.reload()
-    >>> identifier2.party == party1
-    True
-    >>> bool(identifier2.active)
-    False
+    >>> assertEqual(identifier2.party, party1)
+    >>> assertFalse(identifier2.active)
 
     >>> address2.reload()
-    >>> address2.party == party1
-    True
-    >>> bool(address2.active)
-    False
+    >>> assertEqual(address2.party, party1)
+    >>> assertFalse(address2.active)
```

### Comparing `trytond_party-7.0.2/tests/test_module.py` & `trytond_party-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/tox.ini` & `trytond_party-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/trytond_party.egg-info/PKG-INFO` & `trytond_party-7.2.0/trytond_party.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_party
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-party/
+Project-URL: Documentation, https://docs.tryton.org/modules-party/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -50,18 +50,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
 Requires-Dist: python-stdnum>=1.19
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 Requires-Dist: phonenumbers; extra == "test"
 Provides-Extra: vies
 Requires-Dist: python-stdnum[SOAP]; extra == "vies"
 Provides-Extra: phonenumbers
 Requires-Dist: phonenumbers; extra == "phonenumbers"
 
 ############
```

### Comparing `trytond_party-7.0.2/trytond_party.egg-info/SOURCES.txt` & `trytond_party-7.2.0/trytond_party.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 address.py
```

### Comparing `trytond_party-7.0.2/view/address_form.xml` & `trytond_party-7.2.0/view/address_form.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_party-7.0.2/view/address_form.xml` & `trytond_party-7.2.0/view/address_form.xml`

```diff
@@ -14,16 +14,16 @@
     <field name="sequence"/>
   </group>
   <notebook colspan="6">
     <page string="General" id="general">
       <label name="name"/>
       <field name="name"/>
       <newline/>
-      <label name="street"/>
-      <field name="street" colspan="3"/>
+      <label name="street" yalign="0"/>
+      <field name="street" colspan="3" height="80"/>
       <newline/>
       <label name="postal_code"/>
       <field name="postal_code"/>
       <label name="city"/>
       <field name="city"/>
       <newline/>
       <label name="country"/>
```

### Comparing `trytond_party-7.0.2/view/address_form_simple.xml` & `trytond_party-7.2.0/view/address_form_simple.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_party-7.0.2/view/address_form_simple.xml` & `trytond_party-7.2.0/view/address_form_simple.xml`

```diff
@@ -13,16 +13,16 @@
     <label name="sequence"/>
     <field name="sequence"/>
   </group>
   <newline/>
   <label name="name"/>
   <field name="name"/>
   <newline/>
-  <label name="street"/>
-  <field name="street" colspan="3"/>
+  <label name="street" yalign="0"/>
+  <field name="street" colspan="3" height="80"/>
   <newline/>
   <label name="postal_code"/>
   <field name="postal_code"/>
   <label name="city"/>
   <field name="city"/>
   <newline/>
   <label name="country"/>
```

### Comparing `trytond_party-7.0.2/view/address_tree_sequence.xml` & `trytond_party-7.2.0/view/address_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/view/contact_mechanism_form.xml` & `trytond_party-7.2.0/view/contact_mechanism_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/view/contact_mechanism_tree_sequence.xml` & `trytond_party-7.2.0/view/contact_mechanism_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/view/identifier_form.xml` & `trytond_party-7.2.0/view/identifier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-7.0.2/view/party_form.xml` & `trytond_party-7.2.0/view/party_form.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_party-7.0.2/view/party_form.xml` & `trytond_party-7.2.0/view/party_form.xml`

```diff
@@ -3,15 +3,15 @@
 this repository contains the full copyright notices and license terms. -->
 <form col="6">
   <group col="6" colspan="5" id="header" yalign="0">
     <label name="name"/>
     <field name="name" xexpand="1"/>
     <label name="code"/>
     <field name="code"/>
-    <group col="-1" colspan="2" id="checkboxes">
+    <group col="-1" colspan="2" id="checkboxes" xexpand="0">
       <label name="active"/>
       <field name="active" xexpand="0" width="25"/>
       <!-- Add here some checkboxes ! -->
     </group>
     <label name="replaced_by"/>
     <field name="replaced_by"/>
   </group>
```

