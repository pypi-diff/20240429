# Comparing `tmp/secretvalidate-0.0.1a0.tar.gz` & `tmp/secretvalidate-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a0.tar", last modified: Mon Apr 29 11:12:14 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a1.tar", last modified: Mon Apr 29 11:18:31 2024, max compression
```

## Comparing `secretvalidate-0.0.1a0.tar` & `secretvalidate-0.0.1a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:12:14.527503 secretvalidate-0.0.1a0/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a0/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 11:12:14.522505 secretvalidate-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:12:14.412503 secretvalidate-0.0.1a0/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a0/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a0/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:12:14.427504 secretvalidate-0.0.1a0/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a0/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     1940 2024-04-29 10:59:30.000000 secretvalidate-0.0.1a0/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:12:14.517507 secretvalidate-0.0.1a0/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 11:12:13.000000 secretvalidate-0.0.1a0/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 11:12:14.000000 secretvalidate-0.0.1a0/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:12:13.000000 secretvalidate-0.0.1a0/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-29 11:12:13.000000 secretvalidate-0.0.1a0/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:12:13.000000 secretvalidate-0.0.1a0/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 11:12:13.000000 secretvalidate-0.0.1a0/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:12:14.528503 secretvalidate-0.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0      844 2024-04-29 11:10:54.000000 secretvalidate-0.0.1a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:12:14.510504 secretvalidate-0.0.1a0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a0/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a0/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.422631 secretvalidate-0.0.1a1/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a1/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:18:31.414632 secretvalidate-0.0.1a1/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.199636 secretvalidate-0.0.1a1/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a1/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a1/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.258633 secretvalidate-0.0.1a1/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a1/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-04-29 10:59:30.000000 secretvalidate-0.0.1a1/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.391632 secretvalidate-0.0.1a1/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:18:31.422631 secretvalidate-0.0.1a1/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-29 11:18:08.000000 secretvalidate-0.0.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.382633 secretvalidate-0.0.1a1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a1/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a1/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a0/LICENSE` & `secretvalidate-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a0/secretvalidate/validator.py` & `secretvalidate-0.0.1a1/secretvalidate/validator.py`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a0/setup.py` & `secretvalidate-0.0.1a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a',
+    version='0.0.1a1',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['*.txt', '../requirements.txt'],
     },
     install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'secretvalidate=secretvalidate.cli:main',
+            'secretvalidate=secretvalidate.validator:main',
         ],
     },
 )
```

