# Comparing `tmp/secretvalidate-0.0.1a1.tar.gz` & `tmp/secretvalidate-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a1.tar", last modified: Mon Apr 29 11:18:31 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a2.tar", last modified: Mon Apr 29 11:30:12 2024, max compression
```

## Comparing `secretvalidate-0.0.1a1.tar` & `secretvalidate-0.0.1a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.422631 secretvalidate-0.0.1a1/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a1/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 11:18:31.414632 secretvalidate-0.0.1a1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.199636 secretvalidate-0.0.1a1/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a1/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a1/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.258633 secretvalidate-0.0.1a1/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a1/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     1940 2024-04-29 10:59:30.000000 secretvalidate-0.0.1a1/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.391632 secretvalidate-0.0.1a1/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 11:18:30.000000 secretvalidate-0.0.1a1/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:18:31.422631 secretvalidate-0.0.1a1/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-04-29 11:18:08.000000 secretvalidate-0.0.1a1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:18:31.382633 secretvalidate-0.0.1a1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a1/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a1/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.663238 secretvalidate-0.0.1a2/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a2/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:30:12.660236 secretvalidate-0.0.1a2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.549238 secretvalidate-0.0.1a2/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a2/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a2/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.564239 secretvalidate-0.0.1a2/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a2/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     1952 2024-04-29 11:26:07.000000 secretvalidate-0.0.1a2/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.657234 secretvalidate-0.0.1a2/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:30:12.664235 secretvalidate-0.0.1a2/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-29 11:21:55.000000 secretvalidate-0.0.1a2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.651236 secretvalidate-0.0.1a2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a2/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a2/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a1/LICENSE` & `secretvalidate-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a1/secretvalidate/validator.py` & `secretvalidate-0.0.1a2/secretvalidate/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,7 +56,9 @@
     except requests.HTTPError as e:
         if response:
                     return "InActive"
         else:
             return e.response.text
     except requests.RequestException as e:
         return None
+    pass
+
```

### Comparing `secretvalidate-0.0.1a1/setup.py` & `secretvalidate-0.0.1a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a1',
+    version='0.0.1a2',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

