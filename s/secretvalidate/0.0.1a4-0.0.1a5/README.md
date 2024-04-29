# Comparing `tmp/secretvalidate-0.0.1a4.tar.gz` & `tmp/secretvalidate-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a4.tar", last modified: Mon Apr 29 11:45:49 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a5.tar", last modified: Mon Apr 29 11:52:24 2024, max compression
```

## Comparing `secretvalidate-0.0.1a4.tar` & `secretvalidate-0.0.1a5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.563034 secretvalidate-0.0.1a4/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a4/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 11:45:49.557032 secretvalidate-0.0.1a4/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.422035 secretvalidate-0.0.1a4/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a4/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a4/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.450032 secretvalidate-0.0.1a4/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a4/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     2719 2024-04-29 11:45:27.000000 secretvalidate-0.0.1a4/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.553032 secretvalidate-0.0.1a4/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:45:49.563034 secretvalidate-0.0.1a4/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-04-29 11:45:45.000000 secretvalidate-0.0.1a4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.546033 secretvalidate-0.0.1a4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a4/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a4/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:52:24.655145 secretvalidate-0.0.1a5/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a5/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:52:24.650146 secretvalidate-0.0.1a5/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 11:52:24.528146 secretvalidate-0.0.1a5/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a5/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a5/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:52:24.544146 secretvalidate-0.0.1a5/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a5/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     2229 2024-04-29 11:51:38.000000 secretvalidate-0.0.1a5/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:52:24.647147 secretvalidate-0.0.1a5/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:52:24.000000 secretvalidate-0.0.1a5/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 11:52:24.000000 secretvalidate-0.0.1a5/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:52:24.000000 secretvalidate-0.0.1a5/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-29 11:52:24.000000 secretvalidate-0.0.1a5/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 11:52:24.000000 secretvalidate-0.0.1a5/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 11:52:24.000000 secretvalidate-0.0.1a5/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:52:24.655145 secretvalidate-0.0.1a5/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-29 11:52:20.000000 secretvalidate-0.0.1a5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:52:24.640145 secretvalidate-0.0.1a5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a5/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a5/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a4/LICENSE` & `secretvalidate-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a4/setup.py` & `secretvalidate-0.0.1a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a4',
+    version='0.0.1a5',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

