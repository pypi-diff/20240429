# Comparing `tmp/jdtaxcalculator-0.0.3.tar.gz` & `tmp/jdtaxcalculator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdtaxcalculator-0.0.3.tar", last modified: Mon Apr 29 10:29:15 2024, max compression
+gzip compressed data, was "jdtaxcalculator-0.0.4.tar", last modified: Mon Apr 29 10:34:43 2024, max compression
```

## Comparing `jdtaxcalculator-0.0.3.tar` & `jdtaxcalculator-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:29:15.478814 jdtaxcalculator-0.0.3/
--rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      495 2024-04-29 10:29:15.477816 jdtaxcalculator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 10:29:15.466363 jdtaxcalculator-0.0.3/jdtaxcalculator/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.3/jdtaxcalculator/__init__.py
--rw-rw-rw-   0        0        0     4612 2024-04-29 10:08:30.000000 jdtaxcalculator-0.0.3/jdtaxcalculator/jdtaxcalculator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:29:15.477816 jdtaxcalculator-0.0.3/jdtaxcalculator.egg-info/
--rw-rw-rw-   0        0        0      495 2024-04-29 10:29:15.000000 jdtaxcalculator-0.0.3/jdtaxcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-29 10:29:15.000000 jdtaxcalculator-0.0.3/jdtaxcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:29:15.000000 jdtaxcalculator-0.0.3/jdtaxcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-29 10:29:15.000000 jdtaxcalculator-0.0.3/jdtaxcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:29:15.479810 jdtaxcalculator-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      628 2024-04-29 10:29:10.000000 jdtaxcalculator-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:29:15.475821 jdtaxcalculator-0.0.3/test/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.3/test/__init__.py
--rw-rw-rw-   0        0        0     9788 2024-04-29 10:23:06.000000 jdtaxcalculator-0.0.3/test/test_income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:34:43.904453 jdtaxcalculator-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      495 2024-04-29 10:34:43.904453 jdtaxcalculator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jdtaxcalculator-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:34:43.903455 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/
+-rw-rw-rw-   0        0        0      495 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-29 10:34:43.000000 jdtaxcalculator-0.0.4/jdtaxcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:34:43.904453 jdtaxcalculator-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      628 2024-04-29 10:34:38.000000 jdtaxcalculator-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:34:43.902459 jdtaxcalculator-0.0.4/test/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jdtaxcalculator-0.0.4/test/__init__.py
+-rw-rw-rw-   0        0        0     9788 2024-04-29 10:23:06.000000 jdtaxcalculator-0.0.4/test/test_income_calculator.py
```

### Comparing `jdtaxcalculator-0.0.3/LICENSE` & `jdtaxcalculator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jdtaxcalculator-0.0.3/setup.py` & `jdtaxcalculator-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jdtaxcalculator",
-    version="0.0.3",
+    version="0.0.4",
     author="Jack Dyer",
     author_email="jack.dyer387@gmail.com",
     description="UK Tax Calculator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `jdtaxcalculator-0.0.3/test/test_income_calculator.py` & `jdtaxcalculator-0.0.4/test/test_income_calculator.py`

 * *Files identical despite different names*

