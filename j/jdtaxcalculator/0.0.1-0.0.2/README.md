# Comparing `tmp/jdtaxcalculator-0.0.1.tar.gz` & `tmp/jdtaxcalculator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdtaxcalculator-0.0.1.tar", last modified: Mon Apr 29 10:22:41 2024, max compression
+gzip compressed data, was "jdtaxcalculator-0.0.2.tar", last modified: Mon Apr 29 10:26:38 2024, max compression
```

## Comparing `jdtaxcalculator-0.0.1.tar` & `jdtaxcalculator-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:22:41.924151 jdtaxcalculator-0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      495 2024-04-29 10:22:41.923154 jdtaxcalculator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 10:22:41.922157 jdtaxcalculator-0.0.1/jdtaxcalculator.egg-info/
--rw-rw-rw-   0        0        0      495 2024-04-29 10:22:41.000000 jdtaxcalculator-0.0.1/jdtaxcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-29 10:22:41.000000 jdtaxcalculator-0.0.1/jdtaxcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:22:41.000000 jdtaxcalculator-0.0.1/jdtaxcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 10:22:41.000000 jdtaxcalculator-0.0.1/jdtaxcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:22:41.924151 jdtaxcalculator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      628 2024-04-29 10:22:35.000000 jdtaxcalculator-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:22:41.921158 jdtaxcalculator-0.0.1/test/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     9814 2024-04-29 10:08:30.000000 jdtaxcalculator-0.0.1/test/test_income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:38.798346 jdtaxcalculator-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      495 2024-04-29 10:26:38.797348 jdtaxcalculator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:38.796353 jdtaxcalculator-0.0.2/jdtaxcalculator.egg-info/
+-rw-rw-rw-   0        0        0      495 2024-04-29 10:26:38.000000 jdtaxcalculator-0.0.2/jdtaxcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-29 10:26:38.000000 jdtaxcalculator-0.0.2/jdtaxcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:26:38.000000 jdtaxcalculator-0.0.2/jdtaxcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 10:26:38.000000 jdtaxcalculator-0.0.2/jdtaxcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:26:38.798346 jdtaxcalculator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      628 2024-04-29 10:26:31.000000 jdtaxcalculator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:38.793359 jdtaxcalculator-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     4612 2024-04-29 10:08:30.000000 jdtaxcalculator-0.0.2/src/jdtaxcalculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:38.794355 jdtaxcalculator-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     9788 2024-04-29 10:23:06.000000 jdtaxcalculator-0.0.2/test/test_income_calculator.py
```

### Comparing `jdtaxcalculator-0.0.1/LICENSE` & `jdtaxcalculator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jdtaxcalculator-0.0.1/setup.py` & `jdtaxcalculator-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jdtaxcalculator",
-    version="0.0.1",
+    version="0.0.2",
     author="Jack Dyer",
     author_email="jack.dyer387@gmail.com",
     description="UK Tax Calculator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `jdtaxcalculator-0.0.1/test/test_income_calculator.py` & `jdtaxcalculator-0.0.2/test/test_income_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 import pytest
-from jackdyeruktaxcalculator.uk_tax_calculator import UkTaxCalculator
+from jdtaxcalculator import UkTaxCalculator
 
 
 class TestInit(TestCase):
 
     def test_negative_income(self):
         income = -100
         deductions = 0
```

