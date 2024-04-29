# Comparing `tmp/decoutilities-0.1.1.tar.gz` & `tmp/decoutilities-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.1.tar", last modified: Fri Apr 26 14:45:28 2024, max compression
+gzip compressed data, was "decoutilities-0.1.2.tar", last modified: Mon Apr 29 07:32:01 2024, max compression
```

## Comparing `decoutilities-0.1.1.tar` & `decoutilities-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 14:45:28.551296 decoutilities-0.1.1/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3053 2024-04-26 14:45:28.528297 decoutilities-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 14:45:28.389265 decoutilities-0.1.1/config/
--rw-rw-rw-   0        0        0       70 2024-04-26 13:18:54.000000 decoutilities-0.1.1/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.1/config/config.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.1/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:45:28.505293 decoutilities-0.1.1/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     3053 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 14:45:28.552295 decoutilities-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-04-26 14:44:49.000000 decoutilities-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:01.737159 decoutilities-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3053 2024-04-29 07:32:01.726160 decoutilities-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:01.619161 decoutilities-0.1.2/config/
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.2/config/config.py
+-rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.2/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:01.704160 decoutilities-0.1.2/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     3053 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:32:01.738159 decoutilities-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-04-29 07:31:50.000000 decoutilities-0.1.2/setup.py
```

### Comparing `decoutilities-0.1.1/LICENSE` & `decoutilities-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.1/PKG-INFO` & `decoutilities-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.1
+Version: 0.1.2
 Summary: Enhance the readability of your code with decorators.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.1.1/README.md` & `decoutilities-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.1/config/config.py` & `decoutilities-0.1.2/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.1/config/configContainer.py` & `decoutilities-0.1.2/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.1/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.1.2/decoutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.1
+Version: 0.1.2
 Summary: Enhance the readability of your code with decorators.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.1.1/setup.py` & `decoutilities-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.1.1',
+version='0.1.2',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators.',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

