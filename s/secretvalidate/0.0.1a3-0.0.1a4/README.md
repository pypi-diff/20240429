# Comparing `tmp/secretvalidate-0.0.1a3.tar.gz` & `tmp/secretvalidate-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a3.tar", last modified: Mon Apr 29 11:44:03 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a4.tar", last modified: Mon Apr 29 11:45:49 2024, max compression
```

## Comparing `secretvalidate-0.0.1a3.tar` & `secretvalidate-0.0.1a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.541997 secretvalidate-0.0.1a3/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a3/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 11:44:03.530995 secretvalidate-0.0.1a3/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.383001 secretvalidate-0.0.1a3/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a3/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a3/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.415997 secretvalidate-0.0.1a3/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a3/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     2744 2024-04-29 11:43:09.000000 secretvalidate-0.0.1a3/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.524999 secretvalidate-0.0.1a3/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:44:03.541997 secretvalidate-0.0.1a3/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-04-29 11:43:43.000000 secretvalidate-0.0.1a3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.515998 secretvalidate-0.0.1a3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a3/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a3/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.563034 secretvalidate-0.0.1a4/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a4/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:45:49.557032 secretvalidate-0.0.1a4/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.422035 secretvalidate-0.0.1a4/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a4/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a4/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.450032 secretvalidate-0.0.1a4/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a4/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     2719 2024-04-29 11:45:27.000000 secretvalidate-0.0.1a4/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.553032 secretvalidate-0.0.1a4/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 11:45:49.000000 secretvalidate-0.0.1a4/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:45:49.563034 secretvalidate-0.0.1a4/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-29 11:45:45.000000 secretvalidate-0.0.1a4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:45:49.546033 secretvalidate-0.0.1a4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a4/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a4/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a3/LICENSE` & `secretvalidate-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a3/secretvalidate/validator.py` & `secretvalidate-0.0.1a4/secretvalidate/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                     return "InActive"
         else:
             return e.response.text
     except requests.RequestException as e:
         return None
     pass
 
-def main(service, secret, response):
+def main():
     parser = argparse.ArgumentParser(description="Secret Validator Tool")
     parser.add_argument("-service", choices=["snyk", "sonarcloud"], required=True, help="Service to validate secret for")
     parser.add_argument("-secret", required=True, help="Secret to validate")
     parser.add_argument('-r', '--response', action='store_true', help='Print simple response (status/true/false).')
     
     # Parse the command-line arguments
     args = parser.parse_args()
```

### Comparing `secretvalidate-0.0.1a3/setup.py` & `secretvalidate-0.0.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a3',
+    version='0.0.1a4',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

