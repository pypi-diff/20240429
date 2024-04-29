# Comparing `tmp/decoutilities-0.1.4.tar.gz` & `tmp/decoutilities-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.4.tar", last modified: Mon Apr 29 10:39:34 2024, max compression
+gzip compressed data, was "decoutilities-0.1.5.tar", last modified: Mon Apr 29 10:48:12 2024, max compression
```

## Comparing `decoutilities-0.1.4.tar` & `decoutilities-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:39:33.986055 decoutilities-0.1.4/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     3053 2024-04-29 10:39:33.961012 decoutilities-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 10:39:33.817882 decoutilities-0.1.4/decoutilities/
--rw-rw-rw-   0        0        0      809 2024-04-29 10:39:04.000000 decoutilities-0.1.4/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:39:33.948012 decoutilities-0.1.4/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     3053 2024-04-29 10:39:33.000000 decoutilities-0.1.4/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-29 10:39:33.000000 decoutilities-0.1.4/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:39:33.000000 decoutilities-0.1.4/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 10:39:33.000000 decoutilities-0.1.4/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:39:33.986055 decoutilities-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-04-29 10:39:14.000000 decoutilities-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.490532 decoutilities-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3053 2024-04-29 10:48:12.472532 decoutilities-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.297532 decoutilities-0.1.5/decoutilities/
+-rw-rw-rw-   0        0        0      809 2024-04-29 10:39:04.000000 decoutilities-0.1.5/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.419532 decoutilities-0.1.5/decoutilities/config/
+-rw-rw-rw-   0        0        0       43 2024-04-29 10:47:46.000000 decoutilities-0.1.5/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.5/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.5/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.450531 decoutilities-0.1.5/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     3053 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:48:12.491531 decoutilities-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      680 2024-04-29 10:48:04.000000 decoutilities-0.1.5/setup.py
```

### Comparing `decoutilities-0.1.4/LICENSE` & `decoutilities-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.4/PKG-INFO` & `decoutilities-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.4
+Version: 0.1.5
 Summary: Enhance the readability of your code with decorators.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.1.4/README.md` & `decoutilities-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.4/decoutilities/__init__.py` & `decoutilities-0.1.5/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.4/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.1.5/decoutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.4
+Version: 0.1.5
 Summary: Enhance the readability of your code with decorators.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.1.4/setup.py` & `decoutilities-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.1.4',
+version='0.1.5',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators.',
-packages=find_packages(),
+packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
 'Operating System :: OS Independent',
 ],
 python_requires='>=3.6',
 long_description=long_description,
```

