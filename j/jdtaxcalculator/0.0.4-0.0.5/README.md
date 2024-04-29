# Comparing `tmp/jdtaxcalculator-0.0.4.tar.gz` & `tmp/jdtaxcalculator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdtaxcalculator-0.0.4.tar", last modified: Mon Apr 29 10:34:43 2024, max compression
+gzip compressed data, was "jdtaxcalculator-0.0.5.tar", last modified: Mon Apr 29 10:46:28 2024, max compression
```

## Comparing `jdtaxcalculator-0.0.4.tar` & `jdtaxcalculator-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:34:43.904453 jdtaxcalculator-0.0.4/
--rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      495 2024-04-29 10:34:43.904453 jdtaxcalculator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 10:34:43.903455 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/
--rw-rw-rw-   0        0        0      495 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:34:43.904453 jdtaxcalculator-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      628 2024-04-29 10:34:38.000000 jdtaxcalculator-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:34:43.902459 jdtaxcalculator-0.0.4/test/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.4/test/__init__.py
--rw-rw-rw-   0        0        0     9788 2024-04-29 10:23:06.000000 jdtaxcalculator-0.0.4/test/test_income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:46:28.062321 jdtaxcalculator-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      610 2024-04-29 10:46:28.061325 jdtaxcalculator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.5/README.md
+-rw-rw-rw-   0        0        0      603 2024-04-29 10:45:52.000000 jdtaxcalculator-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:46:28.062321 jdtaxcalculator-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 10:46:28.041375 jdtaxcalculator-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 10:46:28.046362 jdtaxcalculator-0.0.5/src/jdtaxcalculator/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.5/src/jdtaxcalculator/__init__.py
+-rw-rw-rw-   0        0        0     4612 2024-04-29 10:08:30.000000 jdtaxcalculator-0.0.5/src/jdtaxcalculator/uk_tax_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:46:28.061325 jdtaxcalculator-0.0.5/src/jdtaxcalculator.egg-info/
+-rw-rw-rw-   0        0        0      610 2024-04-29 10:46:28.000000 jdtaxcalculator-0.0.5/src/jdtaxcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-04-29 10:46:28.000000 jdtaxcalculator-0.0.5/src/jdtaxcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:46:28.000000 jdtaxcalculator-0.0.5/src/jdtaxcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 10:46:28.000000 jdtaxcalculator-0.0.5/src/jdtaxcalculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 10:46:28.059330 jdtaxcalculator-0.0.5/test/
+-rw-rw-rw-   0        0        0     9788 2024-04-29 10:23:06.000000 jdtaxcalculator-0.0.5/test/test_income_calculator.py
```

### Comparing `jdtaxcalculator-0.0.4/LICENSE` & `jdtaxcalculator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jdtaxcalculator-0.0.4/test/test_income_calculator.py` & `jdtaxcalculator-0.0.5/test/test_income_calculator.py`

 * *Files identical despite different names*

