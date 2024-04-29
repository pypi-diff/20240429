# Comparing `tmp/trytond_account_payment_sepa-7.0.0.tar.gz` & `tmp/trytond_account_payment_sepa-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_sepa-7.0.0.tar", last modified: Mon Oct 30 17:23:25 2023, max compression
+gzip compressed data, was "trytond_account_payment_sepa-7.2.0.tar", last modified: Mon Apr 29 15:35:01 2024, max compression
```

## Comparing `trytond_account_payment_sepa-7.0.0.tar` & `trytond_account_payment_sepa-7.2.0.tar`

### file list

```diff
@@ -1,99 +1,98 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.743599 trytond_account_payment_sepa-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:22:53.000000 trytond_account_payment_sepa-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-30 17:02:43.000000 trytond_account_payment_sepa-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:02:43.000000 trytond_account_payment_sepa-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4558 2023-10-30 17:23:25.743599 trytond_account_payment_sepa-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-08-13 15:26:13.000000 trytond_account_payment_sepa-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1056 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.740265 trytond_account_payment_sepa-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:22:53.000000 trytond_account_payment_sepa-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:53.000000 trytond_account_payment_sepa-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.730265 trytond_account_payment_sepa-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14910 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16985 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14377 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17220 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16868 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16064 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17244 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17008 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14691 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14237 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16454 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15217 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14491 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16936 2023-10-30 16:47:45.000000 trytond_account_payment_sepa-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14648 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16059 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13793 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14999 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15931 2023-10-30 16:47:45.000000 trytond_account_payment_sepa-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14512 2023-10-28 12:11:20.000000 trytond_account_payment_sepa-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81515 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/mandate.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3817 2023-10-27 17:38:49.000000 trytond_account_payment_sepa-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    33864 2023-10-27 17:38:49.000000 trytond_account_payment_sepa-7.0.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15511 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/sepa_handler.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:23:25.743599 trytond_account_payment_sepa-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4585 2023-10-27 17:38:49.000000 trytond_account_payment_sepa-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.733599 trytond_account_payment_sepa-7.0.0/template/
--rw-r--r--   0 ced       (1000) ced       (1000)     4112 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/base.003.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/base.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4970 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/pain.001.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/pain.001.001.05.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/pain.001.003.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/pain.008.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4824 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/pain.008.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/template/pain.008.003.02.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.736932 trytond_account_payment_sepa-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.01.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    54208 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.01.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1394 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    63527 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    88220 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    87039 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/camt.054.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    45054 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/pain.001.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    46028 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/pain.001.001.05.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    19631 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/pain.001.003.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    43289 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/pain.008.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    44237 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/pain.008.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    26052 2023-10-24 08:23:41.000000 trytond_account_payment_sepa-7.0.0/tests/pain.008.003.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    15710 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_payment_sepa-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:02:40.000000 trytond_account_payment_sepa-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.740265 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4558 2023-10-30 17:23:25.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3443 2023-10-30 17:23:25.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:23:25.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:23:25.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-10-30 17:23:25.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:23:25.000000 trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:25.740265 trytond_account_payment_sepa-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/view/mandate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/mandate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.0.0/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/party_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1027 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.0.0/view/payment_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2919 2024-04-29 15:15:19.000000 trytond_account_payment_sepa-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:15:18.000000 trytond_account_payment_sepa-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4558 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2024-01-27 09:58:52.000000 trytond_account_payment_sepa-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1056 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.197930 trytond_account_payment_sepa-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_account_payment_sepa-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:57.000000 trytond_account_payment_sepa-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.201263 trytond_account_payment_sepa-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14910 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16985 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14377 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17220 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16868 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16064 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17244 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17008 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14691 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14237 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16454 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15217 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14491 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16936 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14648 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16059 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13893 2024-04-29 13:17:17.000000 trytond_account_payment_sepa-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14999 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15931 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14512 2024-04-27 16:43:21.000000 trytond_account_payment_sepa-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81526 2024-04-29 13:17:17.000000 trytond_account_payment_sepa-7.2.0/mandate.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3817 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    33864 2024-03-17 11:01:36.000000 trytond_account_payment_sepa-7.2.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14944 2024-04-27 16:30:39.000000 trytond_account_payment_sepa-7.2.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/sepa_handler.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4585 2024-03-17 11:01:36.000000 trytond_account_payment_sepa-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.201263 trytond_account_payment_sepa-7.2.0/template/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4112 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/base.003.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/base.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4970 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.001.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.001.001.05.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.001.003.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.008.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4824 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.008.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/template/pain.008.003.02.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.201263 trytond_account_payment_sepa-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    54208 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1394 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    63527 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    88220 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    87039 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    45054 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.001.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    46028 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.001.001.05.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    19631 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.001.003.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    43289 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.008.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    44237 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.008.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    26052 2024-02-04 18:51:26.000000 trytond_account_payment_sepa-7.2.0/tests/pain.008.003.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    15710 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:57.000000 trytond_account_payment_sepa-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-29 15:15:14.000000 trytond_account_payment_sepa-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4558 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3425 2024-04-29 15:35:01.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:00.000000 trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:01.204596 trytond_account_payment_sepa-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/view/mandate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/mandate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-7.2.0/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/party_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-03-08 19:04:12.000000 trytond_account_payment_sepa-7.2.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1027 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-7.2.0/view/payment_list.xml
```

### Comparing `trytond_account_payment_sepa-7.0.0/CHANGELOG` & `trytond_account_payment_sepa-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_account_payment_sepa-7.0.0/COPYRIGHT` & `trytond_account_payment_sepa-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2013-2023 Cédric Krier.
-Copyright (C) 2013-2023 B2CK SPRL.
+Copyright (C) 2013-2024 Cédric Krier.
+Copyright (C) 2013-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_payment_sepa-7.0.0/LICENSE` & `trytond_account_payment_sepa-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/PKG-INFO` & `trytond_account_payment_sepa-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_sepa
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for SEPA payment
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
@@ -52,19 +52,19 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
 Requires-Dist: lxml
 Requires-Dist: python-dateutil
 Requires-Dist: python-stdnum>=1.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Account Payment SEPA Module
 ###########################
 
 The account_payment_sepa module allows to generate SEPA files for a Payment
 Group.
```

### Comparing `trytond_account_payment_sepa-7.0.0/README.rst` & `trytond_account_payment_sepa-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/__init__.py` & `trytond_account_payment_sepa-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/account.py` & `trytond_account_payment_sepa-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/account.xml` & `trytond_account_payment_sepa-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/doc/conf.py` & `trytond_account_payment_sepa-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_payment_sepa-7.0.0/doc/index.rst` & `trytond_account_payment_sepa-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/bg.po` & `trytond_account_payment_sepa-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/ca.po` & `trytond_account_payment_sepa-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/cs.po` & `trytond_account_payment_sepa-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/de.po` & `trytond_account_payment_sepa-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/es.po` & `trytond_account_payment_sepa-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/es_419.po` & `trytond_account_payment_sepa-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/et.po` & `trytond_account_payment_sepa-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/fa.po` & `trytond_account_payment_sepa-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/fi.po` & `trytond_account_payment_sepa-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/fr.po` & `trytond_account_payment_sepa-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/hu.po` & `trytond_account_payment_sepa-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/id.po` & `trytond_account_payment_sepa-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/it.po` & `trytond_account_payment_sepa-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/lo.po` & `trytond_account_payment_sepa-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/lt.po` & `trytond_account_payment_sepa-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/nl.po` & `trytond_account_payment_sepa-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/pl.po` & `trytond_account_payment_sepa-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/pt.po` & `trytond_account_payment_sepa-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/ro.po` & `trytond_account_payment_sepa-7.2.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:account.configuration,sepa_mandate_sequence:"
 msgid "SEPA Mandate Sequence"
 msgstr ""
 
 msgctxt "field:account.configuration.sepa_mandate_sequence,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt ""
 "field:account.configuration.sepa_mandate_sequence,sepa_mandate_sequence:"
 msgid "SEPA Mandate Sequence"
 msgstr ""
 
 msgctxt "field:account.payment,sepa_end_to_end_id:"
@@ -85,15 +85,15 @@
 
 msgctxt "field:account.payment.sepa.mandate,account_number:"
 msgid "Account Number"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,has_payments:"
 msgid "Has Payments"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,identification:"
 msgid "Identification"
@@ -105,15 +105,15 @@
 
 msgctxt "field:account.payment.sepa.mandate,is_first_payment:"
 msgid "Is First Payment"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,payments:"
 msgid "Payments"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,scheme:"
 msgid "Scheme"
@@ -133,15 +133,15 @@
 
 msgctxt "field:account.payment.sepa.mandate,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.payment.sepa.message,filename:"
 msgid "Filename"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,message:"
 msgid "Message"
@@ -149,15 +149,15 @@
 
 msgctxt "field:account.payment.sepa.message,message_file_id:"
 msgid "Message File ID"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:account.payment.sepa.message,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,type:"
 msgid "Type"
@@ -381,19 +381,19 @@
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "BIC"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "City"
-msgstr "Oraș"
+msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Country"
-msgstr "Țară"
+msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Creditor identifier"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Creditor name"
@@ -401,15 +401,15 @@
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Creditor's name"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Location"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Name of the debtor"
@@ -567,15 +567,15 @@
 
 msgctxt "view:account.payment.journal:"
 msgid "SEPA"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Information"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Return Reason"
```

### Comparing `trytond_account_payment_sepa-7.0.0/locale/ru.po` & `trytond_account_payment_sepa-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/sl.po` & `trytond_account_payment_sepa-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/tr.po` & `trytond_account_payment_sepa-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/locale/uk.po` & `trytond_account_payment_sepa-7.2.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:account.configuration,sepa_mandate_sequence:"
 msgid "SEPA Mandate Sequence"
 msgstr ""
 
 msgctxt "field:account.configuration.sepa_mandate_sequence,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt ""
 "field:account.configuration.sepa_mandate_sequence,sepa_mandate_sequence:"
 msgid "SEPA Mandate Sequence"
 msgstr ""
 
 msgctxt "field:account.payment,sepa_end_to_end_id:"
@@ -65,15 +65,15 @@
 
 msgctxt "field:account.payment.journal,sepa_charge_bearer:"
 msgid "Charge Bearer"
 msgstr ""
 
 msgctxt "field:account.payment.journal,sepa_payable_flavor:"
 msgid "Payable Flavor"
-msgstr ""
+msgstr "Varianta Plata"
 
 msgctxt "field:account.payment.journal,sepa_payable_initiator_id:"
 msgid "SEPA Payable Initiator Identifier"
 msgstr ""
 
 msgctxt "field:account.payment.journal,sepa_receivable_flavor:"
 msgid "Receivable Flavor"
@@ -85,15 +85,15 @@
 
 msgctxt "field:account.payment.sepa.mandate,account_number:"
 msgid "Account Number"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.payment.sepa.mandate,has_payments:"
 msgid "Has Payments"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,identification:"
 msgid "Identification"
@@ -105,15 +105,15 @@
 
 msgctxt "field:account.payment.sepa.mandate,is_first_payment:"
 msgid "Is First Payment"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:account.payment.sepa.mandate,payments:"
 msgid "Payments"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.mandate,scheme:"
 msgid "Scheme"
@@ -133,15 +133,15 @@
 
 msgctxt "field:account.payment.sepa.mandate,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.payment.sepa.message,filename:"
 msgid "Filename"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,message:"
 msgid "Message"
@@ -149,15 +149,15 @@
 
 msgctxt "field:account.payment.sepa.message,message_file_id:"
 msgid "Message File ID"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:account.payment.sepa.message,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.payment.sepa.message,type:"
 msgid "Type"
@@ -254,15 +254,15 @@
 "model:ir.action.act_window.domain,name:act_message_form_domain_waiting"
 msgid "Waiting"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_move_line_form_domain_receivable_mandate"
 msgid "Receivable with Mandate"
-msgstr ""
+msgstr "Client cu Mandat"
 
 msgctxt "model:ir.message,text:msg_mandate_authorisation_statement"
 msgid ""
 "By signing this mandate form, you authorise (A) %(creditor)s to send "
 "instructions to your bank to debit your account and (B) your bank to debit "
 "your account in accordance with the instructions from %(creditor)s."
 msgstr ""
@@ -381,19 +381,19 @@
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "BIC"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "City"
-msgstr ""
+msgstr "Oraș"
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Country"
-msgstr ""
+msgstr "Țară"
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Creditor identifier"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Creditor name"
@@ -401,15 +401,15 @@
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Creditor's name"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Location"
 msgstr ""
 
 msgctxt "report:account.payment.sepa.mandate:"
 msgid "Name of the debtor"
@@ -479,23 +479,23 @@
 
 msgctxt "selection:account.payment.journal,sepa_charge_bearer:"
 msgid "Shared"
 msgstr ""
 
 msgctxt "selection:account.payment.journal,sepa_payable_initiator_id:"
 msgid "Belgian Enterprise Number"
-msgstr ""
+msgstr "Belgia, Număr Intreprindere"
 
 msgctxt "selection:account.payment.journal,sepa_payable_initiator_id:"
 msgid "SEPA Creditor Identifier"
-msgstr ""
+msgstr "SEPA Identificator Creditor"
 
 msgctxt "selection:account.payment.journal,sepa_payable_initiator_id:"
 msgid "Spanish VAT Number"
-msgstr ""
+msgstr "Spania, Nr. TVA"
 
 msgctxt "selection:account.payment.journal,sepa_receivable_initiator_id:"
 msgid "Belgian Enterprise Number"
 msgstr ""
 
 msgctxt "selection:account.payment.journal,sepa_receivable_initiator_id:"
 msgid "SEPA Creditor Identifier"
@@ -567,15 +567,15 @@
 
 msgctxt "view:account.payment.journal:"
 msgid "SEPA"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Code"
-msgstr ""
+msgstr "Cod"
 
 msgctxt "view:account.payment:"
 msgid "Information"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Return Reason"
```

### Comparing `trytond_account_payment_sepa-7.0.0/locale/zh_CN.po` & `trytond_account_payment_sepa-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/mandate.fodt` & `trytond_account_payment_sepa-7.2.0/mandate.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_account_payment_sepa-7.0.0/mandate.fodt` & `trytond_account_payment_sepa-7.2.0/mandate.fodt`

```diff
@@ -565,15 +565,15 @@
   <office:master-styles>
     <style:master-page style:name="Standard" style:page-layout-name="pm1">
       <style:header>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -585,15 +585,15 @@
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
```

### Comparing `trytond_account_payment_sepa-7.0.0/message.xml` & `trytond_account_payment_sepa-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/party.py` & `trytond_account_payment_sepa-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/party.xml` & `trytond_account_payment_sepa-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/payment.py` & `trytond_account_payment_sepa-7.2.0/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/payment.xml` & `trytond_account_payment_sepa-7.2.0/payment.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account_payment_sepa-7.0.0/payment.xml` & `trytond_account_payment_sepa-7.2.0/payment.xml`

```diff
@@ -77,64 +77,64 @@
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_mandate_form"/>
     </record>
     <menuitem parent="bank.menu_banking" action="act_mandate_form" sequence="30" id="menu_mandate_form"/>
     <record model="ir.rule.group" id="rule_group_mandate_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_mandate_companies"/>
     </record>
     <record model="ir.model.access" id="access_mandate">
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_mandate_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_mandate_account_payment">
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="group" ref="account_payment.group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="mandate_cancel_button">
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
       <field name="confirm">Are you sure you want to cancel the mandate?</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
     </record>
     <record model="ir.model.button" id="mandate_draft_button">
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
     </record>
     <record model="ir.model.button" id="mandate_validate_mandate_button">
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="name">validate_mandate</field>
       <field name="string">Validate</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
     </record>
     <record model="ir.model.button" id="mandate_request_button">
+      <field name="model">account.payment.sepa.mandate</field>
       <field name="name">request</field>
       <field name="string">Request</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.mandate')]"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_mandate">
       <field name="name">SEPA Mandate</field>
     </record>
     <record model="ir.sequence.type-res.group" id="sequence_type_mandate_group_admin">
       <field name="sequence_type" ref="sequence_type_mandate"/>
       <field name="group" ref="res.group_admin"/>
@@ -197,70 +197,70 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="act_window" ref="act_message_form"/>
     </record>
     <menuitem parent="account_payment.menu_payments" action="act_message_form" sequence="50" id="menu_message_form"/>
     <record model="ir.rule.group" id="rule_group_message_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
+      <field name="model">account.payment.sepa.message</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_message_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_message_companies"/>
     </record>
     <record model="ir.model.access" id="access_message">
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
+      <field name="model">account.payment.sepa.message</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_message_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
+      <field name="model">account.payment.sepa.message</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_mmessage_account_payment">
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
+      <field name="model">account.payment.sepa.message</field>
       <field name="group" ref="account_payment.group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="message_cancel_button">
+      <field name="model">account.payment.sepa.message</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
       <field name="confirm">Are you sure you want to cancel the messages?</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
     </record>
     <record model="ir.model.button" id="message_draft_button">
+      <field name="model">account.payment.sepa.message</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
     </record>
     <record model="ir.model.button" id="message_wait_button">
+      <field name="model">account.payment.sepa.message</field>
       <field name="name">wait</field>
       <field name="string">Wait</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
     </record>
     <record model="ir.model.button" id="message_do_button">
+      <field name="model">account.payment.sepa.message</field>
       <field name="name">do</field>
       <field name="string">Do</field>
       <field name="confirm">Are you sure you want to process the messages?</field>
-      <field name="model" search="[('model', '=', 'account.payment.sepa.message')]"/>
     </record>
     <record model="ir.model.button" id="group_generate_message_button">
+      <field name="model">account.payment.group</field>
       <field name="name">sepa_generate_message</field>
       <field name="string">Generate SEPA Message</field>
-      <field name="model" search="[('model', '=', 'account.payment.group')]"/>
     </record>
     <record model="ir.action.report" id="report_mandate">
       <field name="name">Mandate</field>
       <field name="model">account.payment.sepa.mandate</field>
       <field name="report_name">account.payment.sepa.mandate</field>
       <field name="report">account_payment_sepa/mandate.fodt</field>
     </record>
```

### Comparing `trytond_account_payment_sepa-7.0.0/sepa_handler.py` & `trytond_account_payment_sepa-7.2.0/sepa_handler.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/setup.py` & `trytond_account_payment_sepa-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/base.003.xml` & `trytond_account_payment_sepa-7.2.0/template/base.003.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/base.xml` & `trytond_account_payment_sepa-7.2.0/template/base.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/pain.001.001.03.xml` & `trytond_account_payment_sepa-7.2.0/template/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/pain.001.001.05.xml` & `trytond_account_payment_sepa-7.2.0/template/pain.001.001.05.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/pain.001.003.03.xml` & `trytond_account_payment_sepa-7.2.0/template/pain.001.003.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/pain.008.001.02.xml` & `trytond_account_payment_sepa-7.2.0/template/pain.008.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/pain.008.001.04.xml` & `trytond_account_payment_sepa-7.2.0/template/pain.008.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/template/pain.008.003.02.xml` & `trytond_account_payment_sepa-7.2.0/template/pain.008.003.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.01.xml` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.01.xsd` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.01.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.02.xml` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.02.xsd` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.03.xml` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.03.xsd` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.04.xml` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/camt.054.001.04.xsd` & `trytond_account_payment_sepa-7.2.0/tests/camt.054.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/pain.001.001.03.xsd` & `trytond_account_payment_sepa-7.2.0/tests/pain.001.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/pain.001.001.05.xsd` & `trytond_account_payment_sepa-7.2.0/tests/pain.001.001.05.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/pain.001.003.03.xsd` & `trytond_account_payment_sepa-7.2.0/tests/pain.001.003.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/pain.008.001.02.xsd` & `trytond_account_payment_sepa-7.2.0/tests/pain.008.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/pain.008.001.04.xsd` & `trytond_account_payment_sepa-7.2.0/tests/pain.008.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/pain.008.003.02.xsd` & `trytond_account_payment_sepa-7.2.0/tests/pain.008.003.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tests/test_module.py` & `trytond_account_payment_sepa-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/tox.ini` & `trytond_account_payment_sepa-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/PKG-INFO` & `trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-payment-sepa
-Version: 7.0.0
+Name: trytond_account_payment_sepa
+Version: 7.2.0
 Summary: Tryton module for SEPA payment
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
@@ -52,19 +52,19 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
 Requires-Dist: lxml
 Requires-Dist: python-dateutil
 Requires-Dist: python-stdnum>=1.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Account Payment SEPA Module
 ###########################
 
 The account_payment_sepa module allows to generate SEPA files for a Payment
 Group.
```

### Comparing `trytond_account_payment_sepa-7.0.0/trytond_account_payment_sepa.egg-info/SOURCES.txt` & `trytond_account_payment_sepa-7.2.0/trytond_account_payment_sepa.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_payment_sepa-7.0.0/view/mandate_form.xml` & `trytond_account_payment_sepa-7.2.0/view/mandate_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/view/message_form.xml` & `trytond_account_payment_sepa-7.2.0/view/message_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/view/payment_form.xml` & `trytond_account_payment_sepa-7.2.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-7.0.0/view/payment_journal_form.xml` & `trytond_account_payment_sepa-7.2.0/view/payment_journal_form.xml`

 * *Files identical despite different names*

