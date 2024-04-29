# Comparing `tmp/jackdyeruktaxcalculator-0.0.5.tar.gz` & `tmp/jackdyeruktaxcalculator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jackdyeruktaxcalculator-0.0.5.tar", last modified: Mon Apr 29 08:14:05 2024, max compression
+gzip compressed data, was "jackdyeruktaxcalculator-0.0.6.tar", last modified: Mon Apr 29 08:16:56 2024, max compression
```

## Comparing `jackdyeruktaxcalculator-0.0.5.tar` & `jackdyeruktaxcalculator-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.759761 jackdyeruktaxcalculator-0.0.5/
--rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      503 2024-04-29 08:14:05.758764 jackdyeruktaxcalculator-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.758764 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/
--rw-rw-rw-   0        0        0      503 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 08:14:05.000000 jackdyeruktaxcalculator-0.0.5/jackdyeruktaxcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 08:14:05.759761 jackdyeruktaxcalculator-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-04-29 08:11:00.000000 jackdyeruktaxcalculator-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.755773 jackdyeruktaxcalculator-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.5/src/__init__.py
--rw-rw-rw-   0        0        0     4605 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.5/src/income_calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:14:05.757767 jackdyeruktaxcalculator-0.0.5/test/
--rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.5/test/__init__.py
--rw-rw-rw-   0        0        0     9563 2024-04-29 08:10:34.000000 jackdyeruktaxcalculator-0.0.5/test/test_income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:16:56.932306 jackdyeruktaxcalculator-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-04-29 08:16:56.931308 jackdyeruktaxcalculator-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-04-26 13:07:20.000000 jackdyeruktaxcalculator-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 08:16:56.920338 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator/__init__.py
+-rw-rw-rw-   0        0        0     4605 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator/income_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:16:56.930311 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator.egg-info/
+-rw-rw-rw-   0        0        0      503 2024-04-29 08:16:56.000000 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-29 08:16:56.000000 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:16:56.000000 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-29 08:16:56.000000 jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:16:56.932306 jackdyeruktaxcalculator-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-04-29 08:16:50.000000 jackdyeruktaxcalculator-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:16:56.929315 jackdyeruktaxcalculator-0.0.6/test/
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:54:48.000000 jackdyeruktaxcalculator-0.0.6/test/__init__.py
+-rw-rw-rw-   0        0        0     9563 2024-04-29 08:10:34.000000 jackdyeruktaxcalculator-0.0.6/test/test_income_calculator.py
```

### Comparing `jackdyeruktaxcalculator-0.0.5/LICENSE` & `jackdyeruktaxcalculator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jackdyeruktaxcalculator-0.0.5/setup.py` & `jackdyeruktaxcalculator-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jackdyeruktaxcalculator",
-    version="0.0.5",
+    version="0.0.6",
     author="Jack Dyer",
     author_email="jack.dyer387@gmail.com",
     description="UK Tax Calculator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `jackdyeruktaxcalculator-0.0.5/src/income_calculator.py` & `jackdyeruktaxcalculator-0.0.6/jackdyeruktaxcalculator/income_calculator.py`

 * *Files identical despite different names*

### Comparing `jackdyeruktaxcalculator-0.0.5/test/test_income_calculator.py` & `jackdyeruktaxcalculator-0.0.6/test/test_income_calculator.py`

 * *Files identical despite different names*

