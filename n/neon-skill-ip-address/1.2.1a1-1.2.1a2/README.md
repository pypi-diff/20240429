# Comparing `tmp/neon-skill-ip_address-1.2.1a1.tar.gz` & `tmp/neon-skill-ip_address-1.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-ip_address-1.2.1a1.tar", last modified: Mon Apr 22 15:16:41 2024, max compression
+gzip compressed data, was "neon-skill-ip_address-1.2.1a2.tar", last modified: Mon Apr 29 17:44:44 2024, max compression
```

## Comparing `neon-skill-ip_address-1.2.1a1.tar` & `neon-skill-ip_address-1.2.1a2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.470087 neon-skill-ip_address-1.2.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.474087 neon-skill-ip_address-1.2.1a1/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/ca-es/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/ca-es/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/ca-es/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/ca-es/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/ca-es/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/ca-es/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.474087 neon-skill-ip_address-1.2.1a1/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/cs-cz/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/cs-cz/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/cs-cz/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/cs-cz/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/cs-cz/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/cs-cz/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.474087 neon-skill-ip_address-1.2.1a1/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/de-de/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/de-de/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/de-de/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/de-de/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/de-de/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/de-de/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.478087 neon-skill-ip_address-1.2.1a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/public.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/word_local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/en-us/word_public.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.478087 neon-skill-ip_address-1.2.1a1/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/es-es/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/es-es/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/es-es/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/es-es/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/es-es/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/es-es/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.478087 neon-skill-ip_address-1.2.1a1/locale/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/eu-eu/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/eu-eu/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/eu-eu/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/eu-eu/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/eu-eu/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/eu-eu/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.478087 neon-skill-ip_address-1.2.1a1/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/it-it/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/it-it/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/it-it/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/it-it/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/it-it/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/it-it/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.482087 neon-skill-ip_address-1.2.1a1/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pl-pl/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pl-pl/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pl-pl/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pl-pl/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pl-pl/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pl-pl/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.482087 neon-skill-ip_address-1.2.1a1/locale/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pt-br/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pt-br/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pt-br/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pt-br/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pt-br/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/pt-br/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.482087 neon-skill-ip_address-1.2.1a1/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/sv-se/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/sv-se/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/sv-se/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/sv-se/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/sv-se/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/sv-se/query.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/locale/uk-ua/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/IP.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/dot.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/ethernet.connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/last digits device.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/last digits.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/my address is.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/my address on X is Y.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/no network connection.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/public.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/word_local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/locale/uk-ua/word_public.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-22 15:16:41.000000 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-22 15:16:41.000000 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:16:41.000000 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 15:16:41.000000 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-22 15:16:41.000000 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 15:16:41.000000 neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:16:41.486087 neon-skill-ip_address-1.2.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-22 15:16:35.000000 neon-skill-ip_address-1.2.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.392564 neon-skill-ip_address-1.2.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 17:44:44.392564 neon-skill-ip_address-1.2.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.376563 neon-skill-ip_address-1.2.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/ca-es/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/cs-cz/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/de-de/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.380563 neon-skill-ip_address-1.2.1a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/public.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/word_local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/en-us/word_public.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/es-es/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/eu-eu/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/it-it/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pl-pl/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.384564 neon-skill-ip_address-1.2.1a2/locale/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/pt-br/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/sv-se/query.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/locale/uk-ua/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/IP.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/dot.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/ethernet.connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/last digits device.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/last digits.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/my address is.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/my address on X is Y.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/no network connection.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/public.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/word_local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/locale/uk-ua/word_public.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 17:44:44.000000 neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:44:44.392564 neon-skill-ip_address-1.2.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:44:44.388563 neon-skill-ip_address-1.2.1a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-29 17:44:40.000000 neon-skill-ip_address-1.2.1a2/version.py
```

### Comparing `neon-skill-ip_address-1.2.1a1/LICENSE` & `neon-skill-ip_address-1.2.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/LICENSE.md` & `neon-skill-ip_address-1.2.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/PKG-INFO` & `neon-skill-ip_address-1.2.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-ip_address
-Version: 1.2.1a1
+Version: 1.2.1a2
 Summary: Neon IP Address Skill
 Home-page: https://github.com/NeonGeckoCom/skill-ip_address
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-ip_address-1.2.1a1/README.md` & `neon-skill-ip_address-1.2.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/__init__.py` & `neon-skill-ip_address-1.2.1a2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 from ifaddr import get_adapters
+from lingua_franca import load_language
 from neon_utils.user_utils import get_user_prefs
 from requests import get
 from adapt.intent import IntentBuilder
 from neon_utils.skills.neon_skill import NeonSkill
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_bus_client.message import Message
 from ovos_workshop.decorators import intent_handler
+from lingua_franca.format import pronounce_number
 
 
 # TODO: Add something equivalent to neon_utils.net_utils
 def get_ifaces(ignore_list: List[str] = None, message: Message = None) -> dict:
     """
     Build a dict with device names and their associated ip address.
     @param ignore_list: list of devices to ignore. Defaults to "lo"
@@ -97,37 +99,40 @@
     @intent_handler(IntentBuilder("IPIntent").require("query").require("IP")
                     .optionally("public"))
     def handle_query_ip(self, message):
         """
         Handle a user request for the IP Address
         :param message: Message associated with request
         """
+        load_language(self.lang)
         if message.data.get("public"):
             public = True
             addr = {'public': self._get_public_ip_address(message)}
         else:
             public = False
             addr = get_ifaces(message=message)
 
-        dot = self.dialog_renderer.render("dot")
-
         if len(addr) == 0:  # No IP Address found
             if not get_user_prefs(message)["response_mode"].get(
                     "limit_dialog"):
                 self.speak_dialog("no network connection", private=True)
             else:
                 self.speak("I'm not connected to a network", private=True)
             return
+
+        dot = self.resources.render_dialog("dot")
+
         if len(addr) == 1:  # Single IP Address to speak
             iface, ip = addr.popitem()
-            ip_spoken = ip.replace(".", f" {dot} ")
+            ip_spoken = f" {dot} ".join([pronounce_number(int(part))
+                                         for part in ip.split('.')])
             if public:
-                say_ip = self.translate("word_public")
+                say_ip = self.resources.render_dialog("word_public")
             else:
-                say_ip = self.translate("word_local")
+                say_ip = self.resources.render_dialog("word_local")
             self.speak_dialog("my address is",
                               {'ip': ip_spoken,
                                'pub': say_ip}, private=True)
 
             self.gui.show_text(ip, "IP Address")
             return
```

### Comparing `neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/PKG-INFO` & `neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-ip-address
-Version: 1.2.1a1
+Version: 1.2.1a2
 Summary: Neon IP Address Skill
 Home-page: https://github.com/NeonGeckoCom/skill-ip_address
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `neon-skill-ip_address-1.2.1a1/neon_skill_ip_address.egg-info/SOURCES.txt` & `neon-skill-ip_address-1.2.1a2/neon_skill_ip_address.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/setup.py` & `neon-skill-ip_address-1.2.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/skill.json` & `neon-skill-ip_address-1.2.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/test/test_skill.py` & `neon-skill-ip_address-1.2.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-ip_address-1.2.1a1/version.py` & `neon-skill-ip_address-1.2.1a2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.2.1a1"
+__version__ = "1.2.1a2"
```

