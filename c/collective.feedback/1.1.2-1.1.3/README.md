# Comparing `tmp/collective.feedback-1.1.2.tar.gz` & `tmp/collective.feedback-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.feedback-1.1.2.tar", last modified: Fri Mar 15 15:27:35 2024, max compression
+gzip compressed data, was "collective.feedback-1.1.3.tar", last modified: Mon Apr 29 09:16:12 2024, max compression
```

## Comparing `collective.feedback-1.1.2.tar` & `collective.feedback-1.1.3.tar`

### file list

```diff
@@ -1,81 +1,79 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.236606 collective.feedback-1.1.2/
--rw-r--r--   0 cekk       (501) staff       (20)      771 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       78 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      670 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      120 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     5766 2024-03-15 15:27:35.236654 collective.feedback-1.1.2/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3749 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.231582 collective.feedback-1.1.2/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     8003 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)      340 2024-03-15 15:27:35.236862 collective.feedback-1.1.2/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2538 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.229487 collective.feedback-1.1.2/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.231699 collective.feedback-1.1.2/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.233372 collective.feedback-1.1.2/src/collective/feedback/
--rw-r--r--   0 cekk       (501) staff       (20)      136 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1473 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      377 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.233859 collective.feedback-1.1.2/src/collective/feedback/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/collective.feedback.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.229719 collective.feedback-1.1.2/src/collective/feedback/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.234072 collective.feedback-1.1.2/src/collective/feedback/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)       28 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective/feedback/locales/en/LC_MESSAGES/collective.feedback.mo
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/en/LC_MESSAGES/collective.feedback.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.229825 collective.feedback-1.1.2/src/collective/feedback/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.234270 collective.feedback-1.1.2/src/collective/feedback/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)       28 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective/feedback/locales/it/LC_MESSAGES/collective.feedback.mo
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/it/LC_MESSAGES/collective.feedback.po
--rw-r--r--   0 cekk       (501) staff       (20)     1754 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      494 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      764 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.230120 collective.feedback-1.1.2/src/collective/feedback/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.234658 collective.feedback-1.1.2/src/collective/feedback/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      810 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/default/actions.xml
--rw-r--r--   0 cekk       (501) staff       (20)      176 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      240 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.234761 collective.feedback-1.1.2/src/collective/feedback/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      199 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      810 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.234866 collective.feedback-1.1.2/src/collective/feedback/profiles/default/to_1100/
--rw-r--r--   0 cekk       (501) staff       (20)      171 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/default/to_1100/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.234967 collective.feedback-1.1.2/src/collective/feedback/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      122 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.235155 collective.feedback-1.1.2/src/collective/feedback/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      197 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.235635 collective.feedback-1.1.2/src/collective/feedback/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2030 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/services/add.py
--rw-r--r--   0 cekk       (501) staff       (20)     1384 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/services/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1782 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/services/delete.py
--rw-r--r--   0 cekk       (501) staff       (20)     8106 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/restapi/services/get.py
--rw-r--r--   0 cekk       (501) staff       (20)      831 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/setuphandlers.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.236016 collective.feedback-1.1.2/src/collective/feedback/storage/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/storage/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      950 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/storage/catalog.py
--rw-r--r--   0 cekk       (501) staff       (20)      402 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/storage/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     4098 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/storage/store.py
--rw-r--r--   0 cekk       (501) staff       (20)     1562 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.236509 collective.feedback-1.1.2/src/collective/feedback/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3120 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/tests/test_delete_content.py
--rw-r--r--   0 cekk       (501) staff       (20)     4153 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/tests/test_feedbacks_add.py
--rw-r--r--   0 cekk       (501) staff       (20)     7925 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/tests/test_feedbacks_get.py
--rw-r--r--   0 cekk       (501) staff       (20)     3299 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/tests/test_store.py
--rw-r--r--   0 cekk       (501) staff       (20)     1147 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)     1079 2024-03-15 15:27:34.000000 collective.feedback-1.1.2/src/collective/feedback/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-15 15:27:35.232543 collective.feedback-1.1.2/src/collective.feedback.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     5766 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2521 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      124 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      242 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2024-03-15 15:27:35.000000 collective.feedback-1.1.2/src/collective.feedback.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.039282 collective.feedback-1.1.3/
+-rw-r--r--   0 lucabel    (501) staff       (20)      887 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       78 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)     1338 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      670 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      120 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)     5882 2024-04-29 09:16:12.039377 collective.feedback-1.1.3/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     3749 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/README.rst
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.026240 collective.feedback-1.1.3/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     8003 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      340 2024-04-29 09:16:12.039778 collective.feedback-1.1.3/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2538 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.021360 collective.feedback-1.1.3/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.026468 collective.feedback-1.1.3/src/collective/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.031209 collective.feedback-1.1.3/src/collective/feedback/
+-rw-r--r--   0 lucabel    (501) staff       (20)      136 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1473 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      377 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.032581 collective.feedback-1.1.3/src/collective/feedback/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/collective.feedback.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.021861 collective.feedback-1.1.3/src/collective/feedback/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.032830 collective.feedback-1.1.3/src/collective/feedback/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/en/LC_MESSAGES/collective.feedback.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.022094 collective.feedback-1.1.3/src/collective/feedback/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.033034 collective.feedback-1.1.3/src/collective/feedback/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/it/LC_MESSAGES/collective.feedback.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1754 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      494 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      764 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.022710 collective.feedback-1.1.3/src/collective/feedback/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.034350 collective.feedback-1.1.3/src/collective/feedback/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      810 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/default/actions.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      176 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      240 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.034659 collective.feedback-1.1.3/src/collective/feedback/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)      199 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/default/registry/main.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      810 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.034922 collective.feedback-1.1.3/src/collective/feedback/profiles/default/to_1100/
+-rw-r--r--   0 lucabel    (501) staff       (20)      171 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/default/to_1100/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.035174 collective.feedback-1.1.3/src/collective/feedback/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      122 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.035671 collective.feedback-1.1.3/src/collective/feedback/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      197 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.036932 collective.feedback-1.1.3/src/collective/feedback/restapi/services/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/services/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2030 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/services/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1384 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/services/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1782 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/services/delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8467 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/restapi/services/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      831 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/setuphandlers.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.037906 collective.feedback-1.1.3/src/collective/feedback/storage/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/storage/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      950 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/storage/catalog.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      402 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/storage/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4098 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/storage/store.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1562 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.039093 collective.feedback-1.1.3/src/collective/feedback/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3120 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/tests/test_delete_content.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4153 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/tests/test_feedbacks_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7925 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/tests/test_feedbacks_get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3299 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/tests/test_store.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1147 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1079 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective/feedback/upgrades.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-29 09:16:12.028885 collective.feedback-1.1.3/src/collective.feedback.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)     5882 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     2381 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      124 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       11 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       11 2024-04-29 09:16:11.000000 collective.feedback-1.1.3/src/collective.feedback.egg-info/top_level.txt
```

### Comparing `collective.feedback-1.1.2/CHANGES.rst` & `collective.feedback-1.1.3/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.3 (2024-04-29)
+------------------
+
+- add a plone2volto url conversion method on feedback download
+  [lucabel]
+
+
 1.1.2 (2024-03-15)
 ------------------
 
 - Fix typo in actions.xml permission.
   [cekk]
```

### Comparing `collective.feedback-1.1.2/DEVELOP.rst` & `collective.feedback-1.1.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/LICENSE.GPL` & `collective.feedback-1.1.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/LICENSE.rst` & `collective.feedback-1.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/PKG-INFO` & `collective.feedback-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.feedback
-Version: 1.1.2
+Version: 1.1.3
 Summary: Feedback mechanism integration for io-comune
 Home-page: https://github.com/collective/collective.feedback
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.feedback/
 Project-URL: Source, https://github.com/collective/collective.feedback
@@ -158,14 +158,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+1.1.3 (2024-04-29)
+------------------
+
+- add a plone2volto url conversion method on feedback download
+  [lucabel]
+
+
 1.1.2 (2024-03-15)
 ------------------
 
 - Fix typo in actions.xml permission.
   [cekk]
```

### Comparing `collective.feedback-1.1.2/README.rst` & `collective.feedback-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/docs/conf.py` & `collective.feedback-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/setup.py` & `collective.feedback-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.feedback",
-    version="1.1.2",
+    version="1.1.3",
     description="Feedback mechanism integration for io-comune",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 1 - Planning",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.feedback-1.1.2/src/collective/feedback/configure.zcml` & `collective.feedback-1.1.3/src/collective/feedback/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/locales/README.rst` & `collective.feedback-1.1.3/src/collective/feedback/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/locales/update.py` & `collective.feedback-1.1.3/src/collective/feedback/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/permissions.zcml` & `collective.feedback-1.1.3/src/collective/feedback/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/profiles/default/actions.xml` & `collective.feedback-1.1.3/src/collective/feedback/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/profiles/default/rolemap.xml` & `collective.feedback-1.1.3/src/collective/feedback/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/restapi/services/add.py` & `collective.feedback-1.1.3/src/collective/feedback/restapi/services/add.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/restapi/services/configure.zcml` & `collective.feedback-1.1.3/src/collective/feedback/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/restapi/services/delete.py` & `collective.feedback-1.1.3/src/collective/feedback/restapi/services/delete.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/restapi/services/get.py` & `collective.feedback-1.1.3/src/collective/feedback/restapi/services/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -210,14 +210,23 @@
         now = datetime.now()
         self.request.response.setHeader(
             "Content-Disposition",
             f'attachment; filename="{self.type}_{now.strftime("%d%m%Y-%H%M%S")}.csv"',
         )
         self.request.response.write(data)
 
+    def plone2volto(self, url):
+        portal_url = api.portal.get().absolute_url()
+        frontend_domain = api.portal.get_registry_record(
+            "volto.frontend_domain", default=""
+        )
+        if frontend_domain and url.startswith(portal_url):
+            return url.replace(portal_url, frontend_domain, 1)
+        return url
+
     def get_data(self):
         tool = getUtility(ICollectiveFeedbackStore)
         sbuf = StringIO()
         rows = []
         columns = ["title", "url", "vote", "comment", "date", "answer"]
 
         for item in tool.search():
@@ -236,15 +245,15 @@
 
                 if isinstance(v, int):
                     v = str(v)
 
                 val = json_compatible(v)
                 data[k] = val
 
-            data["url"] = obj.absolute_url()
+            data["url"] = self.plone2volto(obj.absolute_url())
             rows.append(data)
 
         writer = csv.DictWriter(sbuf, fieldnames=columns, delimiter=",")
         writer.writeheader()
         for row in rows:
             try:
                 writer.writerow(row)
```

### Comparing `collective.feedback-1.1.2/src/collective/feedback/setuphandlers.py` & `collective.feedback-1.1.3/src/collective/feedback/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/storage/catalog.py` & `collective.feedback-1.1.3/src/collective/feedback/storage/catalog.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/storage/store.py` & `collective.feedback-1.1.3/src/collective/feedback/storage/store.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/testing.py` & `collective.feedback-1.1.3/src/collective/feedback/testing.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/tests/test_delete_content.py` & `collective.feedback-1.1.3/src/collective/feedback/tests/test_delete_content.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/tests/test_feedbacks_add.py` & `collective.feedback-1.1.3/src/collective/feedback/tests/test_feedbacks_add.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/tests/test_feedbacks_get.py` & `collective.feedback-1.1.3/src/collective/feedback/tests/test_feedbacks_get.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/tests/test_store.py` & `collective.feedback-1.1.3/src/collective/feedback/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/upgrades.py` & `collective.feedback-1.1.3/src/collective/feedback/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective/feedback/upgrades.zcml` & `collective.feedback-1.1.3/src/collective/feedback/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.feedback-1.1.2/src/collective.feedback.egg-info/PKG-INFO` & `collective.feedback-1.1.3/src/collective.feedback.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.feedback
-Version: 1.1.2
+Version: 1.1.3
 Summary: Feedback mechanism integration for io-comune
 Home-page: https://github.com/collective/collective.feedback
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.feedback/
 Project-URL: Source, https://github.com/collective/collective.feedback
@@ -158,14 +158,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+1.1.3 (2024-04-29)
+------------------
+
+- add a plone2volto url conversion method on feedback download
+  [lucabel]
+
+
 1.1.2 (2024-03-15)
 ------------------
 
 - Fix typo in actions.xml permission.
   [cekk]
```

### Comparing `collective.feedback-1.1.2/src/collective.feedback.egg-info/SOURCES.txt` & `collective.feedback-1.1.3/src/collective.feedback.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 src/collective/feedback/upgrades.py
 src/collective/feedback/upgrades.zcml
 src/collective/feedback/locales/README.rst
 src/collective/feedback/locales/__init__.py
 src/collective/feedback/locales/collective.feedback.pot
 src/collective/feedback/locales/update.py
 src/collective/feedback/locales/update.sh
-src/collective/feedback/locales/en/LC_MESSAGES/collective.feedback.mo
 src/collective/feedback/locales/en/LC_MESSAGES/collective.feedback.po
-src/collective/feedback/locales/it/LC_MESSAGES/collective.feedback.mo
 src/collective/feedback/locales/it/LC_MESSAGES/collective.feedback.po
 src/collective/feedback/profiles/default/actions.xml
 src/collective/feedback/profiles/default/browserlayer.xml
 src/collective/feedback/profiles/default/metadata.xml
 src/collective/feedback/profiles/default/rolemap.xml
 src/collective/feedback/profiles/default/registry/main.xml
 src/collective/feedback/profiles/default/to_1100/rolemap.xml
```

