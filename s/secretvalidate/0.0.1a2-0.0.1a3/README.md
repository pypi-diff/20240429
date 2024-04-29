# Comparing `tmp/secretvalidate-0.0.1a2.tar.gz` & `tmp/secretvalidate-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a2.tar", last modified: Mon Apr 29 11:30:12 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a3.tar", last modified: Mon Apr 29 11:44:03 2024, max compression
```

## Comparing `secretvalidate-0.0.1a2.tar` & `secretvalidate-0.0.1a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.663238 secretvalidate-0.0.1a2/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a2/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 11:30:12.660236 secretvalidate-0.0.1a2/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.549238 secretvalidate-0.0.1a2/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a2/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a2/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.564239 secretvalidate-0.0.1a2/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a2/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     1952 2024-04-29 11:26:07.000000 secretvalidate-0.0.1a2/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.657234 secretvalidate-0.0.1a2/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 11:30:12.000000 secretvalidate-0.0.1a2/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:30:12.664235 secretvalidate-0.0.1a2/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-04-29 11:21:55.000000 secretvalidate-0.0.1a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:30:12.651236 secretvalidate-0.0.1a2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a2/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a2/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.541997 secretvalidate-0.0.1a3/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a3/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:44:03.530995 secretvalidate-0.0.1a3/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.383001 secretvalidate-0.0.1a3/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a3/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a3/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.415997 secretvalidate-0.0.1a3/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a3/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     2744 2024-04-29 11:43:09.000000 secretvalidate-0.0.1a3/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.524999 secretvalidate-0.0.1a3/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 11:44:02.000000 secretvalidate-0.0.1a3/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:44:03.541997 secretvalidate-0.0.1a3/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-29 11:43:43.000000 secretvalidate-0.0.1a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:44:03.515998 secretvalidate-0.0.1a3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a3/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a3/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a2/LICENSE` & `secretvalidate-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a2/secretvalidate/validator.py` & `secretvalidate-0.0.1a3/secretvalidate/validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 import json
 import requests
 import os
 
 # Reuse session for multiple requests
 session = requests.Session()
 
@@ -58,7 +59,25 @@
                     return "InActive"
         else:
             return e.response.text
     except requests.RequestException as e:
         return None
     pass
 
+def main(service, secret, response):
+    parser = argparse.ArgumentParser(description="Secret Validator Tool")
+    parser.add_argument("-service", choices=["snyk", "sonarcloud"], required=True, help="Service to validate secret for")
+    parser.add_argument("-secret", required=True, help="Secret to validate")
+    parser.add_argument('-r', '--response', action='store_true', help='Print simple response (status/true/false).')
+    
+    # Parse the command-line arguments
+    args = parser.parse_args()
+    
+    try:
+        # Call the validate function with provided arguments
+        result = main(args.service, args.secret, args.response)
+        print(result)
+    except Exception as e:
+        print(f"Error: {e}")
+
+if __name__ == "__main__":
+    main()
```

### Comparing `secretvalidate-0.0.1a2/setup.py` & `secretvalidate-0.0.1a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a2',
+    version='0.0.1a3',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

