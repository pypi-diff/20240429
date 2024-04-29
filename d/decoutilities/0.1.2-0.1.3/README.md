# Comparing `tmp/decoutilities-0.1.2.tar.gz` & `tmp/decoutilities-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.2.tar", last modified: Mon Apr 29 07:32:01 2024, max compression
+gzip compressed data, was "decoutilities-0.1.3.tar", last modified: Mon Apr 29 10:13:48 2024, max compression
```

## Comparing `decoutilities-0.1.2.tar` & `decoutilities-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:01.737159 decoutilities-0.1.2/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3053 2024-04-29 07:32:01.726160 decoutilities-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:01.619161 decoutilities-0.1.2/config/
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.2/config/config.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.2/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:01.704160 decoutilities-0.1.2/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     3053 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:32:01.000000 decoutilities-0.1.2/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 07:32:01.738159 decoutilities-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-04-29 07:31:50.000000 decoutilities-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:13:48.941108 decoutilities-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3053 2024-04-29 10:13:48.917109 decoutilities-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:13:48.805108 decoutilities-0.1.3/decoutilities/
+-rw-rw-rw-   0        0        0      424 2024-04-29 08:52:59.000000 decoutilities-0.1.3/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:13:48.902107 decoutilities-0.1.3/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     3053 2024-04-29 10:13:48.000000 decoutilities-0.1.3/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-29 10:13:48.000000 decoutilities-0.1.3/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:13:48.000000 decoutilities-0.1.3/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 10:13:48.000000 decoutilities-0.1.3/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:13:48.941108 decoutilities-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-04-29 10:11:21.000000 decoutilities-0.1.3/setup.py
```

### Comparing `decoutilities-0.1.2/LICENSE` & `decoutilities-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.2/PKG-INFO` & `decoutilities-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.2
+Version: 0.1.3
 Summary: Enhance the readability of your code with decorators.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.1.2/README.md` & `decoutilities-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.2/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.1.3/decoutilities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.2
+Version: 0.1.3
 Summary: Enhance the readability of your code with decorators.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.1.2/setup.py` & `decoutilities-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.1.2',
+version='0.1.3',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators.',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

