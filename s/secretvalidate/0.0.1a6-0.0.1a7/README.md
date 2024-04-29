# Comparing `tmp/secretvalidate-0.0.1a6.tar.gz` & `tmp/secretvalidate-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a6.tar", last modified: Mon Apr 29 11:54:21 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a7.tar", last modified: Mon Apr 29 12:04:02 2024, max compression
```

## Comparing `secretvalidate-0.0.1a6.tar` & `secretvalidate-0.0.1a7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:54:21.784983 secretvalidate-0.0.1a6/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a6/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 11:54:21.775981 secretvalidate-0.0.1a6/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 11:54:21.665985 secretvalidate-0.0.1a6/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a6/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a6/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:54:21.684984 secretvalidate-0.0.1a6/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a6/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     2229 2024-04-29 11:51:38.000000 secretvalidate-0.0.1a6/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:54:21.771980 secretvalidate-0.0.1a6/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 11:54:21.000000 secretvalidate-0.0.1a6/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 11:54:21.000000 secretvalidate-0.0.1a6/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:54:21.000000 secretvalidate-0.0.1a6/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-29 11:54:21.000000 secretvalidate-0.0.1a6/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 11:54:21.000000 secretvalidate-0.0.1a6/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 11:54:21.000000 secretvalidate-0.0.1a6/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:54:21.784983 secretvalidate-0.0.1a6/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-04-29 11:54:17.000000 secretvalidate-0.0.1a6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:54:21.764982 secretvalidate-0.0.1a6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a6/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a6/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:04:02.102064 secretvalidate-0.0.1a7/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a7/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 12:04:02.097066 secretvalidate-0.0.1a7/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 12:04:02.003067 secretvalidate-0.0.1a7/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a7/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a7/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:04:02.022065 secretvalidate-0.0.1a7/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a7/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     2181 2024-04-29 12:02:56.000000 secretvalidate-0.0.1a7/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:04:02.094063 secretvalidate-0.0.1a7/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 12:04:01.000000 secretvalidate-0.0.1a7/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 12:04:01.000000 secretvalidate-0.0.1a7/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:04:01.000000 secretvalidate-0.0.1a7/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-29 12:04:01.000000 secretvalidate-0.0.1a7/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 12:04:01.000000 secretvalidate-0.0.1a7/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 12:04:01.000000 secretvalidate-0.0.1a7/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:04:02.103064 secretvalidate-0.0.1a7/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-29 12:03:41.000000 secretvalidate-0.0.1a7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:04:02.087064 secretvalidate-0.0.1a7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a7/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a7/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a6/LICENSE` & `secretvalidate-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a6/secretvalidate/validator.py` & `secretvalidate-0.0.1a7/secretvalidate/validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,19 +56,15 @@
     except requests.HTTPError as e:
         if response:
             return "InActive"
         else:
             return e.response.text
     except requests.RequestException as e:
         return None
-    pass
 
 def main(service, secret, response):  
     try:
         # Call the validate function with provided arguments
-        result = main(service, secret, response)
+        result = validate(service, secret, response)
         print(result)
     except Exception as e:
         print(f"Error: {e}")
-
-if __name__ == "__main__":
-    main()
```

### Comparing `secretvalidate-0.0.1a6/setup.py` & `secretvalidate-0.0.1a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a6',
+    version='0.0.1a7',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

