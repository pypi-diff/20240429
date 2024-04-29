# Comparing `tmp/g3hardware-0.1.1.tar.gz` & `tmp/g3hardware-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3hardware-0.1.1.tar", last modified: Tue Feb  6 17:55:04 2024, max compression
+gzip compressed data, was "g3hardware-0.2.0.tar", last modified: Mon Apr 29 12:44:38 2024, max compression
```

## Comparing `g3hardware-0.1.1.tar` & `g3hardware-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 17:55:04.574826 g3hardware-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3hardware-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     1118 2024-02-06 17:55:04.571823 g3hardware-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      565 2024-02-05 22:32:18.000000 g3hardware-0.1.1/README.md
--rw-rw-rw-   0        0        0      835 2024-02-06 17:54:55.000000 g3hardware-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-06 17:55:04.575825 g3hardware-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-06 17:55:04.475276 g3hardware-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-06 17:55:04.516649 g3hardware-0.1.1/src/g3hardware/
--rw-rw-rw-   0        0        0      161 2024-01-17 13:17:13.000000 g3hardware-0.1.1/src/g3hardware/__init__.py
--rw-rw-rw-   0        0        0     8142 2024-01-17 13:27:23.000000 g3hardware-0.1.1/src/g3hardware/_hw_isle.py
--rw-rw-rw-   0        0        0    10144 2024-01-31 12:05:37.000000 g3hardware-0.1.1/src/g3hardware/_hw_module.py
--rw-rw-rw-   0        0        0     6802 2024-01-14 16:13:38.000000 g3hardware-0.1.1/src/g3hardware/_hw_module_data.py
--rw-rw-rw-   0        0        0        0 2023-09-26 20:40:57.000000 g3hardware-0.1.1/src/g3hardware/py.typed
--rw-rw-rw-   0        0        0    29488 2024-01-31 12:26:48.000000 g3hardware-0.1.1/src/g3hardware/settings.json
-drwxrwxrwx   0        0        0        0 2024-02-06 17:55:04.537262 g3hardware-0.1.1/src/g3hardware/utils/
--rw-rw-rw-   0        0        0        0 2024-01-14 15:59:46.000000 g3hardware-0.1.1/src/g3hardware/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:55:04.558172 g3hardware-0.1.1/src/g3hardware/utils/xmltemplate/
--rw-rw-rw-   0        0        0      315 2023-09-22 14:44:56.000000 g3hardware-0.1.1/src/g3hardware/utils/xmltemplate/__init__.py
--rw-rw-rw-   0        0        0     6545 2023-09-26 16:21:01.000000 g3hardware-0.1.1/src/g3hardware/utils/xmltemplate/_xml_element.py
--rw-rw-rw-   0        0        0     2175 2023-10-01 16:30:22.000000 g3hardware-0.1.1/src/g3hardware/utils/xmltemplate/_xml_file.py
--rw-rw-rw-   0        0        0     3204 2023-09-22 14:39:59.000000 g3hardware-0.1.1/src/g3hardware/utils/xmltemplate/_xml_prolog.py
--rw-rw-rw-   0        0        0      815 2023-09-26 13:59:36.000000 g3hardware-0.1.1/src/g3hardware/utils/xmltemplate/type_hinting.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:55:04.558172 g3hardware-0.1.1/src/g3hardware.egg-info/
--rw-rw-rw-   0        0        0     1118 2024-02-06 17:55:04.000000 g3hardware-0.1.1/src/g3hardware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2024-02-06 17:55:04.000000 g3hardware-0.1.1/src/g3hardware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 17:55:04.000000 g3hardware-0.1.1/src/g3hardware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-02-06 17:55:04.000000 g3hardware-0.1.1/src/g3hardware.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-06 17:55:04.000000 g3hardware-0.1.1/src/g3hardware.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:44:38.277454 g3hardware-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3hardware-0.2.0/LICENCE
+-rw-rw-rw-   0        0        0     1202 2024-04-29 12:44:38.274459 g3hardware-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-04-23 14:01:29.000000 g3hardware-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1262 2024-04-23 14:01:29.000000 g3hardware-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:44:38.278457 g3hardware-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 12:44:36.994954 g3hardware-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:44:37.053934 g3hardware-0.2.0/src/g3hardware/
+-rw-rw-rw-   0        0        0      410 2024-04-23 14:01:29.000000 g3hardware-0.2.0/src/g3hardware/__init__.py
+-rw-rw-rw-   0        0        0    54505 2024-04-23 14:01:29.000000 g3hardware-0.2.0/src/g3hardware/_g3hardware.py
+-rw-rw-rw-   0        0        0      949 2024-04-23 14:01:29.000000 g3hardware-0.2.0/src/g3hardware/api.py
+-rw-rw-rw-   0        0        0     9655 2024-04-23 14:03:01.000000 g3hardware-0.2.0/src/g3hardware/config.yaml
+-rw-rw-rw-   0        0        0        0 2023-09-26 20:40:57.000000 g3hardware-0.2.0/src/g3hardware/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-29 12:44:38.272464 g3hardware-0.2.0/src/g3hardware.egg-info/
+-rw-rw-rw-   0        0        0     1202 2024-04-29 12:44:36.000000 g3hardware-0.2.0/src/g3hardware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2024-04-29 12:44:36.000000 g3hardware-0.2.0/src/g3hardware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:44:36.000000 g3hardware-0.2.0/src/g3hardware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-29 12:44:36.000000 g3hardware-0.2.0/src/g3hardware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 12:44:36.000000 g3hardware-0.2.0/src/g3hardware.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:44:37.338935 g3hardware-0.2.0/tests/
+-rw-rw-rw-   0        0        0     2025 2024-04-23 10:25:50.000000 g3hardware-0.2.0/tests/test_module_config.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 10:25:50.000000 g3hardware-0.2.0/tests/test_module_factory.py
+-rw-rw-rw-   0        0        0     2491 2024-04-23 10:25:50.000000 g3hardware-0.2.0/tests/test_module_template_formatter.py
```

### Comparing `g3hardware-0.1.1/LICENCE` & `g3hardware-0.2.0/LICENCE`

 * *Files identical despite different names*

