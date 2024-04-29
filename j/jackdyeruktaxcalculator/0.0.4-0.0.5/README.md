# Comparing `tmp/jackdyeruktaxcalculator-0.0.4.tar.gz` & `tmp/jackdyeruktaxcalculator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jackdyeruktaxcalculator-0.0.4.tar", last modified: Fri Apr 26 17:55:38 2024, max compression
+gzip compressed data, was "jackdyeruktaxcalculator-0.0.5.tar", last modified: Mon Apr 29 08:14:05 2024, max compression
```

## Comparing `jackdyeruktaxcalculator-0.0.4.tar` & `jackdyeruktaxcalculator-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 17:55:38.696341 jackdyeruktaxcalculator-0.0.4/
--rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      503 2024-04-26 17:55:38.695343 jackdyeruktaxcalculator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 17:55:38.695343 jackdyeruktaxcalculator-0.0.4/jackdyeruktaxcalculator.egg-info/
--rw-rw-rw-   0        0        0      503 2024-04-26 17:55:38.000000 jackdyeruktaxcalculator-0.0.4/jackdyeruktaxcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-26 17:55:38.000000 jackdyeruktaxcalculator-0.0.4/jackdyeruktaxcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 17:55:38.000000 jackdyeruktaxcalculator-0.0.4/jackdyeruktaxcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-26 17:55:38.000000 jackdyeruktaxcalculator-0.0.4/jackdyeruktaxcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 17:55:38.696341 jackdyeruktaxcalculator-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-04-26 17:55:30.000000 jackdyeruktaxcalculator-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:55:38.692351 jackdyeruktaxcalculator-0.0.4/source/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.4/source/__init__.py
--rw-rw-rw-   0        0        0     4605 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.4/source/income_calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:55:38.694346 jackdyeruktaxcalculator-0.0.4/test/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.4/test/__init__.py
--rw-rw-rw-   0        0        0     9566 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.4/test/test_income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.759761 jackdyeruktaxcalculator-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-04-29 08:14:05.758764 jackdyeruktaxcalculator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.758764 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/
+-rw-rw-rw-   0        0        0      503 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:14:05.759761 jackdyeruktaxcalculator-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-04-29 08:11:00.000000 jackdyeruktaxcalculator-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.755773 jackdyeruktaxcalculator-0.0.5/src/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.5/src/__init__.py
+-rw-rw-rw-   0        0        0     4605 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.5/src/income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.757767 jackdyeruktaxcalculator-0.0.5/test/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.5/test/__init__.py
+-rw-rw-rw-   0        0        0     9563 2024-04-29 08:10:34.000000 jackdyeruktaxcalculator-0.0.5/test/test_income_calculator.py
```

### Comparing `jackdyeruktaxcalculator-0.0.4/LICENSE` & `jackdyeruktaxcalculator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jackdyeruktaxcalculator-0.0.4/setup.py` & `jackdyeruktaxcalculator-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jackdyeruktaxcalculator",
-    version="0.0.4",
+    version="0.0.5",
     author="Jack Dyer",
     author_email="jack.dyer387@gmail.com",
     description="UK Tax Calculator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `jackdyeruktaxcalculator-0.0.4/source/income_calculator.py` & `jackdyeruktaxcalculator-0.0.5/src/income_calculator.py`

 * *Files identical despite different names*

### Comparing `jackdyeruktaxcalculator-0.0.4/test/test_income_calculator.py` & `jackdyeruktaxcalculator-0.0.5/test/test_income_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 import pytest
-from source.income_calculator import TakeHome
+from src.income_calculator import TakeHome
 
 
 class TestInit(TestCase):
 
     def test_negative_income(self):
         income = -100
         deductions = 0
```

