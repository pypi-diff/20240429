# Comparing `tmp/trytond_country-7.0.0.tar.gz` & `tmp/trytond_country-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_country-7.0.0.tar", last modified: Mon Oct 30 17:29:02 2023, max compression
+gzip compressed data, was "trytond_country-7.2.0.tar", last modified: Mon Apr 29 15:39:36 2024, max compression
```

## Comparing `trytond_country-7.0.0.tar` & `trytond_country-7.2.0.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.725206 trytond_country-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-22 17:23:02.000000 trytond_country-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-10-30 17:05:52.000000 trytond_country-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-10-30 17:05:52.000000 trytond_country-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_country-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_country-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3056 2023-10-30 17:29:02.725206 trytond_country-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_country-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20545 2023-08-13 15:26:13.000000 trytond_country-7.0.0/country.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13472 2023-04-15 07:12:15.000000 trytond_country-7.0.0/country.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.721872 trytond_country-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-22 17:23:02.000000 trytond_country-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2738 2023-04-15 07:12:15.000000 trytond_country-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_country-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:02.000000 trytond_country-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1114 2023-08-13 15:26:13.000000 trytond_country-7.0.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_country-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.721872 trytond_country-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_country-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-01-16 14:00:20.000000 trytond_country-7.0.0/icons/tryton-country.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.718539 trytond_country-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    25666 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25651 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22688 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25659 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25807 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22530 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24628 2023-10-28 12:11:21.000000 trytond_country-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25889 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22571 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25743 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23696 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21710 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22889 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25695 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25164 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25469 2023-10-30 16:47:45.000000 trytond_country-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25421 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25039 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23473 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26709 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24710 2023-10-30 16:47:45.000000 trytond_country-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22475 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    27230 2023-10-28 12:11:22.000000 trytond_country-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23032 2023-10-30 16:47:45.000000 trytond_country-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-04-15 07:12:15.000000 trytond_country-7.0.0/organization.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8410 2023-04-15 07:12:15.000000 trytond_country-7.0.0/region.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.718539 trytond_country-7.0.0/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-7.0.0/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)    19896 2023-10-07 15:40:36.000000 trytond_country-7.0.0/scripts/import_countries.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4041 2023-10-07 15:40:36.000000 trytond_country-7.0.0/scripts/import_postal_codes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:29:02.725206 trytond_country-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4909 2023-10-27 17:38:49.000000 trytond_country-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.718539 trytond_country-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_country-7.0.0/tests/scenario_country_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3259 2023-04-15 07:12:15.000000 trytond_country-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_country-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_country-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-10-30 17:05:48.000000 trytond_country-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.721872 trytond_country-7.0.0/trytond_country.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3056 2023-10-30 17:29:02.000000 trytond_country-7.0.0/trytond_country.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2438 2023-10-30 17:29:02.000000 trytond_country-7.0.0/trytond_country.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:02.000000 trytond_country-7.0.0/trytond_country.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-10-30 17:29:02.000000 trytond_country-7.0.0/trytond_country.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_country-7.0.0/trytond_country.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-10-30 17:29:02.000000 trytond_country-7.0.0/trytond_country.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:29:02.000000 trytond_country-7.0.0/trytond_country.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:29:02.721872 trytond_country-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/country_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/organization_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/organization_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/organization_member_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/organization_member_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/postal_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/postal_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/region_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/region_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/subdivision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-04-15 07:12:15.000000 trytond_country-7.0.0/view/subdivision_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.910719 trytond_country-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3959 2024-04-29 15:19:06.000000 trytond_country-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:19:05.000000 trytond_country-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_country-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_country-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3047 2024-04-29 15:39:36.910719 trytond_country-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_country-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20545 2024-01-27 09:58:52.000000 trytond_country-7.2.0/country.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13242 2024-04-27 16:30:39.000000 trytond_country-7.2.0/country.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.904052 trytond_country-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_country-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2738 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:08.000000 trytond_country-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1114 2024-01-27 09:58:52.000000 trytond_country-7.2.0/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_country-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.904052 trytond_country-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_country-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-01-16 14:00:20.000000 trytond_country-7.2.0/icons/tryton-country.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.907385 trytond_country-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    25666 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25651 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22688 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25659 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25807 2024-04-27 16:43:22.000000 trytond_country-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22530 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24628 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25889 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22571 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25743 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23696 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21710 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22889 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25695 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25164 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25469 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25421 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25039 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26032 2024-04-29 13:17:17.000000 trytond_country-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26709 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24710 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22475 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27230 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23032 2024-04-27 16:43:23.000000 trytond_country-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-04-15 07:12:15.000000 trytond_country-7.2.0/organization.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8410 2023-04-15 07:12:15.000000 trytond_country-7.2.0/region.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.907385 trytond_country-7.2.0/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-7.2.0/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)    19896 2024-02-04 18:51:26.000000 trytond_country-7.2.0/scripts/import_countries.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4041 2024-02-04 18:51:26.000000 trytond_country-7.2.0/scripts/import_postal_codes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:36.910719 trytond_country-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4900 2024-04-27 16:30:39.000000 trytond_country-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.907385 trytond_country-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2024-04-22 12:14:36.000000 trytond_country-7.2.0/tests/scenario_country_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3259 2023-04-15 07:12:15.000000 trytond_country-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_country-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:08.000000 trytond_country-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2024-04-29 15:19:01.000000 trytond_country-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.910719 trytond_country-7.2.0/trytond_country.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3047 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_country-7.2.0/trytond_country.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:36.000000 trytond_country-7.2.0/trytond_country.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:36.910719 trytond_country-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/country_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_member_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/organization_member_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/postal_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/postal_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/region_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/region_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/subdivision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-04-15 07:12:15.000000 trytond_country-7.2.0/view/subdivision_tree.xml
```

### Comparing `trytond_country-7.0.0/CHANGELOG` & `trytond_country-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_country-7.0.0/COPYRIGHT` & `trytond_country-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2023 Cédric Krier.
+Copyright (C) 2008-2024 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 B2CK SPRL.
 Copyright (C) 2004-2008 Tiny SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_country-7.0.0/LICENSE` & `trytond_country-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/PKG-INFO` & `trytond_country-7.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_country
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with countries
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-country/
+Project-URL: Documentation, https://docs.tryton.org/modules-country/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton country
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: data
 Requires-Dist: pycountry; extra == "data"
-Requires-Dist: proteus<7.1,>=7.0; extra == "data"
+Requires-Dist: proteus<7.3,>=7.2; extra == "data"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 Requires-Dist: pycountry; extra == "test"
 Provides-Extra: geonames
-Requires-Dist: proteus<7.1,>=7.0; extra == "geonames"
+Requires-Dist: proteus<7.3,>=7.2; extra == "geonames"
 Provides-Extra: completion
 Requires-Dist: argcomplete; extra == "completion"
 
 ##############
 Country Module
 ##############
```

### Comparing `trytond_country-7.0.0/country.py` & `trytond_country-7.2.0/country.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/country.xml` & `trytond_country-7.2.0/country.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_country-7.0.0/country.xml` & `trytond_country-7.2.0/country.xml`

```diff
@@ -34,22 +34,22 @@
     <record model="ir.action.act_window.view" id="act_organization_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="organization_view_form"/>
       <field name="act_window" ref="act_organization_form"/>
     </record>
     <menuitem parent="menu_country" action="act_organization_form" sequence="20" id="menu_organization_form"/>
     <record model="ir.model.access" id="access_organization">
-      <field name="model" search="[('model', '=', 'country.organization')]"/>
+      <field name="model">country.organization</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_organization_admin">
-      <field name="model" search="[('model', '=', 'country.organization')]"/>
+      <field name="model">country.organization</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="organization_member_view_form">
@@ -108,22 +108,22 @@
     <record model="ir.action.act_window.view" id="act_region_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="region_view_form"/>
       <field name="act_window" ref="act_region_form"/>
     </record>
     <menuitem parent="menu_region_tree" action="act_region_form" sequence="10" id="menu_region_form"/>
     <record model="ir.model.access" id="access_region">
-      <field name="model" search="[('model', '=', 'country.region')]"/>
+      <field name="model">country.region</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_region_admin">
-      <field name="model" search="[('model', '=', 'country.region')]"/>
+      <field name="model">country.region</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="country_view_form">
@@ -158,22 +158,22 @@
     </record>
     <record model="ir.action.keyword" id="act_country_by_region_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">country.region,-1</field>
       <field name="action" ref="act_country_by_region"/>
     </record>
     <record model="ir.model.access" id="access_country">
-      <field name="model" search="[('model', '=', 'country.country')]"/>
+      <field name="model">country.country</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_country_admin">
-      <field name="model" search="[('model', '=', 'country.country')]"/>
+      <field name="model">country.country</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="subdivision_view_form">
@@ -183,22 +183,22 @@
     </record>
     <record model="ir.ui.view" id="subdivision_view_tree">
       <field name="model">country.subdivision</field>
       <field name="type">tree</field>
       <field name="name">subdivision_tree</field>
     </record>
     <record model="ir.model.access" id="access_subdivision">
-      <field name="model" search="[('model', '=', 'country.subdivision')]"/>
+      <field name="model">country.subdivision</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_subdivision_admin">
-      <field name="model" search="[('model', '=', 'country.subdivision')]"/>
+      <field name="model">country.subdivision</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="postal_code_view_form">
@@ -228,22 +228,22 @@
     </record>
     <record model="ir.action.keyword" id="act_postal_code_form_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">country.country,-1</field>
       <field name="action" ref="act_postal_code_form"/>
     </record>
     <record model="ir.model.access" id="access_postal_code">
-      <field name="model" search="[('model', '=', 'country.postal_code')]"/>
+      <field name="model">country.postal_code</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_postal_code_admin">
-      <field name="model" search="[('model', '=', 'country.postal_code')]"/>
+      <field name="model">country.postal_code</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_country-7.0.0/doc/conf.py` & `trytond_country-7.2.0/doc/conf.py`

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

### Comparing `trytond_country-7.0.0/doc/design.rst` & `trytond_country-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/doc/setup.rst` & `trytond_country-7.2.0/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/icons/LICENSE` & `trytond_country-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/bg.po` & `trytond_country-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/ca.po` & `trytond_country-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/cs.po` & `trytond_country-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/de.po` & `trytond_country-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/es.po` & `trytond_country-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/es_419.po` & `trytond_country-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/et.po` & `trytond_country-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/fa.po` & `trytond_country-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/fi.po` & `trytond_country-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/fr.po` & `trytond_country-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/hu.po` & `trytond_country-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/id.po` & `trytond_country-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/it.po` & `trytond_country-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/lo.po` & `trytond_country-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/lt.po` & `trytond_country-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/nl.po` & `trytond_country-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/pl.po` & `trytond_country-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/pt.po` & `trytond_country-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/ro.po` & `trytond_country-7.2.0/locale/ro.po`

 * *Files 5% similar despite different names*

```diff
@@ -12,76 +12,73 @@
 
 msgctxt "field:country.country,code_numeric:"
 msgid "Numeric Code"
 msgstr "Cod Numeric"
 
 msgctxt "field:country.country,flag:"
 msgid "Flag"
-msgstr ""
+msgstr "Steag"
 
 msgctxt "field:country.country,members:"
 msgid "Members"
-msgstr ""
+msgstr "Membri"
 
 msgctxt "field:country.country,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:country.country,organizations:"
 msgid "Organizations"
-msgstr ""
+msgstr "Organizații"
 
-#, fuzzy
 msgctxt "field:country.country,region:"
 msgid "Region"
 msgstr "Regiune"
 
 msgctxt "field:country.country,subdivisions:"
 msgid "Subdivisions"
 msgstr "Subdiviziune"
 
-#, fuzzy
 msgctxt "field:country.organization,code:"
 msgid "Code"
 msgstr "Cod"
 
-#, fuzzy
 msgctxt "field:country.organization,countries:"
 msgid "Countries"
 msgstr "Țări"
 
 msgctxt "field:country.organization,members:"
 msgid "Members"
-msgstr ""
+msgstr "Membri"
 
 #, fuzzy
 msgctxt "field:country.organization,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:country.organization.member,active:"
 msgid "Active"
-msgstr ""
+msgstr "Activ"
 
-#, fuzzy
 msgctxt "field:country.organization.member,country:"
 msgid "Country"
 msgstr "Țară"
 
 msgctxt "field:country.organization.member,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "De la Data"
 
 msgctxt "field:country.organization.member,organization:"
 msgid "Organization"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:country.organization.member,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Până la Data"
 
 msgctxt "field:country.postal_code,city:"
 msgid "City"
 msgstr "Oraș"
 
 msgctxt "field:country.postal_code,country:"
 msgid "Country"
@@ -91,20 +88,18 @@
 msgid "Postal Code"
 msgstr "Cod Poștal"
 
 msgctxt "field:country.postal_code,subdivision:"
 msgid "Subdivision"
 msgstr "Subdiviziune"
 
-#, fuzzy
 msgctxt "field:country.region,code_numeric:"
 msgid "Numeric Code"
 msgstr "Cod Numeric"
 
-#, fuzzy
 msgctxt "field:country.region,countries:"
 msgid "Countries"
 msgstr "Țări"
 
 #, fuzzy
 msgctxt "field:country.region,name:"
 msgid "Name"
@@ -114,27 +109,27 @@
 msgctxt "field:country.region,parent:"
 msgid "Parent"
 msgstr "Parinte"
 
 #, fuzzy
 msgctxt "field:country.region,subregions:"
 msgid "Subregions"
-msgstr "Subdiviziune"
+msgstr "Subregiuni"
 
 msgctxt "field:country.subdivision,code:"
 msgid "Code"
 msgstr "Cod"
 
 msgctxt "field:country.subdivision,country:"
 msgid "Country"
 msgstr "Țară"
 
 msgctxt "field:country.subdivision,flag:"
 msgid "Flag"
-msgstr ""
+msgstr "Steag"
 
 msgctxt "field:country.subdivision,name:"
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:country.subdivision,parent:"
 msgid "Parent"
@@ -168,17 +163,18 @@
 msgid "The country that contains the postal code."
 msgstr "Țara care conține codul poștal."
 
 msgctxt "help:country.postal_code,subdivision:"
 msgid "The subdivision where the postal code is."
 msgstr "Subdiviziunea în care se află codul poștal."
 
+#, fuzzy
 msgctxt "help:country.region,code_numeric:"
 msgid "UN M49 region code."
-msgstr ""
+msgstr "Cod de regiune ONU M49."
 
 msgctxt "help:country.subdivision,code:"
 msgid "The ISO code of the subdivision."
 msgstr "Codul ISO al subdiviziuni."
 
 msgctxt "help:country.subdivision,country:"
 msgid "The country where this subdivision is."
@@ -194,293 +190,302 @@
 
 msgctxt "model:country.country,name:"
 msgid "Country"
 msgstr "Țară"
 
 msgctxt "model:country.organization,name:"
 msgid "Organization"
-msgstr ""
+msgstr "Organizație"
 
 msgctxt "model:country.organization,name:organization_amu"
 msgid "Arab Maghreb Union"
-msgstr ""
+msgstr "Uniunea Maghrebului Arab"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_apec"
 msgid "Asia-Pacific Economic Cooperation"
-msgstr ""
+msgstr "Cooperarea Economică Asia-Pacific"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_asean"
 msgid "Association of Southeast Asian Nations"
-msgstr ""
+msgstr "Asociația Națiunilor din Asia de Sud-Est"
 
 msgctxt "model:country.organization,name:organization_benelux"
 msgid "Benelux Union"
-msgstr ""
+msgstr "Uniunea Benelux"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_can"
 msgid "Andean Community"
-msgstr "Comunitatea autonomă"
+msgstr "Comunitatea Andină"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_caricom"
 msgid "Caribbean Community"
-msgstr "Comunitatea autonomă"
+msgstr "Comunitatea Caraibelor"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_cemac"
 msgid "Economic and Monetary Community of Central Africa"
-msgstr ""
+msgstr "Comunitatea Economică și Monetară a Africii Centrale"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_cen-sad"
 msgid "Community of Sahel–Saharan States"
-msgstr ""
+msgstr "Comunitatea Statelor Sahel-Sahariene"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_comesa"
 msgid "Common Market for Eastern and Southern Africa"
-msgstr ""
+msgstr "Piața comună pentru Africa de Est și de Sud"
 
 #, fuzzy
 msgctxt "model:country.organization,name:organization_eac"
 msgid "East African Community"
-msgstr "Comunitatea autonomă"
+msgstr "Comunitatea Est-Africană"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_eccas"
 msgid "Economic Community of Central African States"
-msgstr ""
+msgstr "Comunitatea Economică a Statelor Africii Centrale"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_ecowas"
 msgid "Economic Community of West African States"
-msgstr ""
+msgstr "Comunitatea Economică a Statelor Africii de Vest"
 
 msgctxt "model:country.organization,name:organization_eu"
 msgid "European Union"
-msgstr ""
+msgstr "Uniunea Europeană"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_gcc"
 msgid "Cooperation Council for the Arab States of the Gulf"
-msgstr ""
+msgstr "Consiliul de Cooperare pentru Statele Arabe din Golf"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_igad"
 msgid "Intergovernmental Authority on Development"
-msgstr ""
+msgstr "Autoritatea Interguvernamentală pentru Dezvoltare"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_mercosur"
 msgid "Southern Common Market"
-msgstr ""
+msgstr "Piața comună de sud"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_nafta"
 msgid "North American Free Trade Agreement"
-msgstr ""
+msgstr "Acordul de Liber Schimb din America de Nord"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_sadc"
 msgid "Southern African Development Community"
-msgstr ""
+msgstr "Comunitatea de Dezvoltare a Africii de Sud"
 
+#, fuzzy
 msgctxt "model:country.organization,name:organization_safta"
 msgid "South Asian Free Trade Area"
-msgstr ""
+msgstr "Zona de schimb liber din Asia de Sud"
 
 msgctxt "model:country.organization.member,name:"
 msgid "Organization Member"
-msgstr ""
+msgstr "Membru al organizației"
 
 msgctxt "model:country.postal_code,name:"
 msgid "Postal Code"
 msgstr "Cod Poștal"
 
-#, fuzzy
 msgctxt "model:country.region,name:"
 msgid "Region"
 msgstr "Regiune"
 
 msgctxt "model:country.region,name:region_africa"
 msgid "Africa"
-msgstr ""
+msgstr "Africa"
 
 msgctxt "model:country.region,name:region_americas"
 msgid "Americas"
 msgstr ""
 
 msgctxt "model:country.region,name:region_antarctica"
 msgid "Antarctica"
-msgstr ""
+msgstr "Antarctica"
 
 msgctxt "model:country.region,name:region_asia"
 msgid "Asia"
-msgstr ""
+msgstr "Asia"
 
 msgctxt "model:country.region,name:region_australia_new_zealand"
 msgid "Australia and New Zealand"
-msgstr ""
+msgstr "Australia și Noua Zeelandă"
 
 msgctxt "model:country.region,name:region_caribbean"
 msgid "Caribbean"
-msgstr ""
+msgstr "Caraibe"
 
 msgctxt "model:country.region,name:region_central_america"
 msgid "Central America"
-msgstr ""
+msgstr "America Centrală"
 
 msgctxt "model:country.region,name:region_central_asia"
 msgid "Central Asia"
-msgstr ""
+msgstr "Asia Centrala"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_channel_islands"
 msgid "Channel Islands"
-msgstr ""
+msgstr "Insulele Canalului"
 
 msgctxt "model:country.region,name:region_eastern_africa"
 msgid "Eastern Africa"
-msgstr ""
+msgstr "Africa de Est"
 
 msgctxt "model:country.region,name:region_eastern_asia"
 msgid "Eastern Asia"
-msgstr ""
+msgstr "Asia de Est"
 
 msgctxt "model:country.region,name:region_eastern_europe"
 msgid "Eastern Europe"
-msgstr ""
+msgstr "Europa de Est"
 
 msgctxt "model:country.region,name:region_europe"
 msgid "Europe"
-msgstr ""
+msgstr "Europa"
 
 msgctxt "model:country.region,name:region_latin_america_caribbean"
 msgid "Latin America and the Caribbean"
-msgstr ""
+msgstr "America Latină și Caraibe"
 
 msgctxt "model:country.region,name:region_melanesia"
 msgid "Melanesia"
-msgstr ""
+msgstr "Melanezia"
 
 msgctxt "model:country.region,name:region_micronesia"
 msgid "Micronesia"
-msgstr ""
+msgstr "Micronezia"
 
+#, fuzzy
 msgctxt "model:country.region,name:region_middle_africa"
 msgid "Middle Africa"
-msgstr ""
+msgstr "Africa Centrală"
 
 msgctxt "model:country.region,name:region_north_america"
 msgid "North America"
-msgstr ""
+msgstr "America de Nord"
 
 msgctxt "model:country.region,name:region_northern_africa"
 msgid "Northern Africa"
-msgstr ""
+msgstr "Africa de Nord"
 
 msgctxt "model:country.region,name:region_northern_america"
 msgid "Northern America"
-msgstr ""
+msgstr "America de Nord"
 
 msgctxt "model:country.region,name:region_northern_europe"
 msgid "Northern Europe"
-msgstr ""
+msgstr "Europa de Nord"
 
 msgctxt "model:country.region,name:region_oceania"
 msgid "Oceania"
-msgstr ""
+msgstr "Oceania"
 
 msgctxt "model:country.region,name:region_polynesia"
 msgid "Polynesia"
-msgstr ""
+msgstr "Polinezia"
 
 msgctxt "model:country.region,name:region_south-eastern_asia"
 msgid "South-eastern Asia"
-msgstr ""
+msgstr "Asia de Sud-Est"
 
 msgctxt "model:country.region,name:region_south_america"
 msgid "South America"
-msgstr ""
+msgstr "America de Sud"
 
 msgctxt "model:country.region,name:region_southern_africa"
 msgid "Southern Africa"
-msgstr ""
+msgstr "Africa de Sud"
 
 msgctxt "model:country.region,name:region_southern_asia"
 msgid "Southern Asia"
-msgstr ""
+msgstr "Asia de Sud"
 
 msgctxt "model:country.region,name:region_southern_europe"
 msgid "Southern Europe"
-msgstr ""
+msgstr "Europa de Sud"
 
 msgctxt "model:country.region,name:region_sub-saharan_africa"
 msgid "Sub-Saharan Africa"
-msgstr ""
+msgstr "Africa Sub-Sahariană"
 
 msgctxt "model:country.region,name:region_western_africa"
 msgid "Western Africa"
-msgstr ""
+msgstr "Africa de Vest"
 
 msgctxt "model:country.region,name:region_western_asia"
 msgid "Western Asia"
-msgstr ""
+msgstr "Asia de Vest"
 
 msgctxt "model:country.region,name:region_western_europe"
 msgid "Western Europe"
-msgstr ""
+msgstr "Europa de Vest"
 
 msgctxt "model:country.region,name:region_world"
 msgid "World"
-msgstr ""
+msgstr "Lume"
 
 msgctxt "model:country.subdivision,name:"
 msgid "Subdivision"
 msgstr "Subdiviziune"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_country_by_region"
 msgid "Countries by Region"
-msgstr "Țări"
+msgstr "Țări după regiune"
 
 msgctxt "model:ir.action,name:act_country_form"
 msgid "Countries"
 msgstr "Țări"
 
 msgctxt "model:ir.action,name:act_organization_form"
 msgid "Organizations"
-msgstr ""
+msgstr "Organizații"
 
 msgctxt "model:ir.action,name:act_postal_code_form"
 msgid "Postal Codes"
 msgstr "Coduri Poștale"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_region_form"
 msgid "Regions"
-msgstr "Regiune"
+msgstr "Regiuni"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_region_tree"
 msgid "Areas"
-msgstr "Zonă"
+msgstr "Zone"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_country"
 msgid "Countries"
 msgstr "Țări"
 
 msgctxt "model:ir.ui.menu,name:menu_country_form"
 msgid "Countries"
 msgstr "Țări"
 
 msgctxt "model:ir.ui.menu,name:menu_organization_form"
 msgid "Organizations"
-msgstr ""
+msgstr "Organizații"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_form"
 msgid "Regions"
-msgstr "Regiune"
+msgstr "Regiuni"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_region_tree"
 msgid "Areas"
-msgstr "Zonă"
+msgstr "Zone"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administration"
 msgstr "Administrare"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative Region"
@@ -492,15 +497,15 @@
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative area"
 msgstr "Zona administrativă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative atoll"
-msgstr ""
+msgstr "Atol administrativ"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Administrative precinct"
 msgstr "Regiunea administrativă"
 
 msgctxt "selection:country.subdivision,type:"
@@ -531,18 +536,17 @@
 msgid "Autonomous Province"
 msgstr "Provincia autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous Region"
 msgstr "Regiune autonomă"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous city in north africa"
-msgstr "District autonom"
+msgstr "Oraș autonom din Africa de Nord"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous communities"
 msgstr "Comunitățile autonome"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous community"
@@ -550,15 +554,15 @@
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous island"
 msgstr "Insula autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous monastic state"
-msgstr ""
+msgstr "Stat monahal autonom"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous municipality"
 msgstr "Municipalitate autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Autonomous republic"
@@ -580,83 +584,91 @@
 msgid "Borough"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Canton"
 msgstr "Canton"
 
-#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital"
 msgstr "Capitala"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital District"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Metropolitan City"
-msgstr ""
+msgstr "Capitala Metropolitană"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital Territory"
-msgstr ""
+msgstr "Teritoriul Capitalei"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Capital city"
 msgstr "Capitala"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chain (of islands)"
-msgstr ""
+msgstr "Lanț (de insule)"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Chains (of islands)"
-msgstr ""
+msgstr "Lanțuri (de insule)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "City"
 msgstr "Oraș"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City corporation"
-msgstr ""
+msgstr "Corporația orașului"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City municipality"
-msgstr "Municipalitatea specială"
+msgstr "Municipiul orașului"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "City with county rights"
-msgstr ""
+msgstr "Oraș cu drepturi județene"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Commune"
 msgstr "Comună"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Constitutional province"
-msgstr ""
+msgstr "Provincie constituțională"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Council area"
-msgstr ""
+msgstr "zona Consiliului"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Country"
 msgstr "Țară"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "County"
 msgstr "Județ"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Decentralized regional entity"
-msgstr ""
+msgstr "Entitate regională descentralizată"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Department"
 msgstr "Departament"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Dependency"
@@ -675,21 +687,23 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District municipality"
 msgstr "Municipalitate autonomă"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "District with special status"
-msgstr ""
+msgstr "District cu statut special"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Districts under republic administration"
-msgstr ""
+msgstr "Districte aflate în administrarea republicii"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Division"
 msgstr "Divizia"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Economic Prefecture"
@@ -703,66 +717,73 @@
 msgid "Emirate"
 msgstr "Emirat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Entity"
 msgstr "Entitate"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Dependency"
-msgstr ""
+msgstr "Dependență federală"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal District"
-msgstr ""
+msgstr "District federal"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territories"
-msgstr ""
+msgstr "Teritoriile Federale"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal Territory"
-msgstr "Teritoriu"
+msgstr "Teritoriu federal"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Federal capital territory"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Free municipal consortium"
-msgstr ""
+msgstr "Consorțiu municipal gratuit"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical entity"
 msgstr "Entitate geografică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical region"
 msgstr "Regiunea geografică"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Geographical unit"
 msgstr "Unitate geografică"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Governorate"
-msgstr ""
+msgstr "Guvernorat"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Group of islands (20 inhabited islands)"
-msgstr ""
+msgstr "Grup de insule (20 de insule locuite)"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Included for completeness"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Indigenous region"
-msgstr ""
+msgstr "Regiune indigenă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island"
 msgstr "Insulă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Island council"
@@ -771,85 +792,94 @@
 msgctxt "selection:country.subdivision,type:"
 msgid "Island group"
 msgstr "Grup de insule"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Islands, groups of islands"
-msgstr "Grup de insule"
+msgstr "Insule, grupuri de insule"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Land"
-msgstr ""
+msgstr "Teren"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Local council"
 msgstr "Consiliu Local"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "London borough"
-msgstr ""
+msgstr "Cartier Londonez"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan administration"
-msgstr "Orașe metropolitane"
+msgstr "Administrația metropolitană"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan cities"
 msgstr "Orașe metropolitane"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan city"
-msgstr "Orașe metropolitane"
+msgstr "Oraș metropolitan"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan collectivity with special status"
-msgstr ""
+msgstr "Colectivitate metropolitană cu statut special"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan department"
-msgstr ""
+msgstr "Departament metropolitan"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan district"
-msgstr ""
+msgstr "District Metropolitan"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Metropolitan region"
-msgstr ""
+msgstr "Regiune metropolitană"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipalities"
-msgstr ""
+msgstr "Municipalități"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Municipality"
-msgstr ""
+msgstr "Municipiu"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Nation"
-msgstr ""
+msgstr "Naţiune"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Oblast"
-msgstr ""
+msgstr "Oblast"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Outlying area"
 msgstr "Zona periferică"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity"
-msgstr ""
+msgstr "Colectivitatea de peste mări"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas collectivity with special status"
-msgstr ""
+msgstr "Colectivitate de peste mări cu statut special"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas department"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas region"
@@ -866,19 +896,19 @@
 msgctxt "selection:country.subdivision,type:"
 msgid "Overseas territory"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Pakistan administered area"
-msgstr "Zona administrativă"
+msgstr "Zonă administrată de Pakistan"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Parish"
-msgstr ""
+msgstr "Parohie"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularate"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Popularates"
@@ -886,57 +916,59 @@
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Prefecture"
 msgstr "Prefectură"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Principality"
-msgstr ""
+msgstr "Principat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Province"
 msgstr "Provincie"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Quarter"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Rayon"
-msgstr ""
+msgstr "Raion"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Region"
 msgstr "Regiune"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional council"
 msgstr "Consiliul regional"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Regional state"
-msgstr "Consiliul regional"
+msgstr "Stat regional"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Republic"
 msgstr "Republică"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Republican City"
-msgstr ""
+msgstr "Oraș Republican"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Rural municipality"
-msgstr "Municipalitatea specială"
+msgstr "Municipalitate rurală"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Self-governed part"
-msgstr ""
+msgstr "Parte autonomă"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special District"
 msgstr "District special"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Municipality"
@@ -945,36 +977,38 @@
 msgctxt "selection:country.subdivision,type:"
 msgid "Special Region"
 msgstr "Regiunea specială"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative city"
-msgstr "Regiunea administrativă specială"
+msgstr "Oraș administrativ special"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special administrative region"
 msgstr "Regiunea administrativă specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special city"
 msgstr "Oraș special"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special island authority"
-msgstr ""
+msgstr "Autoritate specială insulară"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing city"
-msgstr "Oraș special"
+msgstr "Oraș special autonom"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Special self-governing province"
-msgstr ""
+msgstr "Provincie Autonomă Specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Special zone"
 msgstr "Zona specială"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "State"
@@ -986,53 +1020,59 @@
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Territory"
 msgstr "Teritoriu"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Town"
-msgstr ""
+msgstr "Oraș"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Town council"
-msgstr ""
+msgstr "Consiliul Local"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Two-tier county"
-msgstr ""
+msgstr "Județul cu două niveluri"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Union territory"
-msgstr ""
+msgstr "Teritoriul Uniunii"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority"
-msgstr ""
+msgstr "Autoritate unitară"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (england)"
-msgstr ""
+msgstr "Autoritate unitară (Anglia)"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Unitary authority (wales)"
-msgstr ""
+msgstr "Autoritate unitară (Țara Galilor)"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban community"
-msgstr "Comunitatea autonomă"
+msgstr "Comunitate urbană"
 
 #, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Urban municipality"
-msgstr "Municipalitatea specială"
+msgstr "Municipalitate urbană"
 
+#, fuzzy
 msgctxt "selection:country.subdivision,type:"
 msgid "Voivodship"
-msgstr ""
+msgstr "Voievodat"
 
 msgctxt "selection:country.subdivision,type:"
 msgid "Ward"
 msgstr ""
 
 msgctxt "selection:country.subdivision,type:"
 msgid "zone"
```

### Comparing `trytond_country-7.0.0/locale/ru.po` & `trytond_country-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/sl.po` & `trytond_country-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/tr.po` & `trytond_country-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/uk.po` & `trytond_country-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/locale/zh_CN.po` & `trytond_country-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/organization.xml` & `trytond_country-7.2.0/organization.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/region.xml` & `trytond_country-7.2.0/region.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/scripts/import_countries.py` & `trytond_country-7.2.0/scripts/import_countries.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/scripts/import_postal_codes.py` & `trytond_country-7.2.0/scripts/import_postal_codes.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/setup.py` & `trytond_country-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/modules-country/',
+        "Documentation": 'https://docs.tryton.org/modules-country/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton country',
     package_dir={'trytond.modules.country': '.'},
     packages=(
         ['trytond.modules.country']
```

### Comparing `trytond_country-7.0.0/tests/scenario_country_import.rst` & `trytond_country-7.2.0/tests/scenario_country_import.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ==============
 Country Import
 ==============
 
 Imports::
 
     >>> from proteus import Model
+    >>> from trytond.modules.country.scripts import (
+    ...     import_countries, import_postal_codes)
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.country.scripts import import_countries, import_postal_codes
 
 Activate modules::
 
     >>> config = activate_modules('country')
 
 Import countries::
```

### Comparing `trytond_country-7.0.0/tests/test_module.py` & `trytond_country-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/tox.ini` & `trytond_country-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/trytond_country.egg-info/PKG-INFO` & `trytond_country-7.2.0/trytond_country.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-country
-Version: 7.0.0
+Name: trytond_country
+Version: 7.2.0
 Summary: Tryton module with countries
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-country/
+Project-URL: Documentation, https://docs.tryton.org/modules-country/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton country
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: data
 Requires-Dist: pycountry; extra == "data"
-Requires-Dist: proteus<7.1,>=7.0; extra == "data"
+Requires-Dist: proteus<7.3,>=7.2; extra == "data"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 Requires-Dist: pycountry; extra == "test"
 Provides-Extra: geonames
-Requires-Dist: proteus<7.1,>=7.0; extra == "geonames"
+Requires-Dist: proteus<7.3,>=7.2; extra == "geonames"
 Provides-Extra: completion
 Requires-Dist: argcomplete; extra == "completion"
 
 ##############
 Country Module
 ##############
```

### Comparing `trytond_country-7.0.0/trytond_country.egg-info/SOURCES.txt` & `trytond_country-7.2.0/trytond_country.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 country.py
```

### Comparing `trytond_country-7.0.0/view/country_form.xml` & `trytond_country-7.2.0/view/country_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-7.0.0/view/subdivision_form.xml` & `trytond_country-7.2.0/view/subdivision_form.xml`

 * *Files identical despite different names*

